<script>
    import { count } from '../store.js';
    import Home_desktop from "./home_desktop.svelte";
    import Navbar from "./navbar.svelte";
    import About from './about.svelte';
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
    <Home_desktop />
    {/if}
    {#if countValue == 1 }
    <About />
    {/if}
    
</div>
