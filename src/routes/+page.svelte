<script>
    import { count } from '../store.js';
    import Home from "./home.svelte";
    import Navbar from "./navbar.svelte";
    import About from './about.svelte';
    import Contact from './contact.svelte';
    import Home_mobile from "./home_mobile.svelte";
    /**
     * @type {number}
     */
    let countValue;

    let width = 1920;
    count.subscribe((value) => {
        countValue = value;
    });
</script>

<svelte:window bind:innerWidth={width}/>
<div>
    <Navbar />
    {#if countValue == 0 }
        {#if width > 1024}
        <Home />
        {:else}
        <Home_mobile />
        {/if}
    {/if}
    {#if countValue == 1 }
    <About />
    {/if}
    {#if countValue == 2 }
    <Contact />
    {/if}
    
</div>


