<script>
    import { count } from '../store.js';
    import Home from "./home.svelte";
    import Navbar from "./navbar.svelte";
    import About from './about.svelte';
    import Contact from './contact.svelte';
    /**
     * @type {number}
     */
    let countValue;

    count.subscribe((value) => {
        countValue = value;
    });
</script>

<div>
    <Navbar />
    {#if countValue == 0 }
    <Home />
    {/if}
    {#if countValue == 1 }
    <About />
    {/if}
    {#if countValue == 2 }
    <Contact />
    {/if}
    
</div>


