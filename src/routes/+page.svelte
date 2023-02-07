<script>
    import { count } from '../store.js';
    import Home_desktop from "./home_desktop.svelte";
    import Navbar from "./navbar.svelte";
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
    <Home_desktop />
    
</div>
