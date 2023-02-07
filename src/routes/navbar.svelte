<script>
    import { count } from "../store.js";

    let bg_color = "#7209B7";

    function home() {
        count.set(0);
        bg_color = "#7209B7";
    }
    function about() {
        count.set(1);
        bg_color = "#000000";
    }
    function contact() {
        count.set(2);
        bg_color = "#000000";
    }
</script>

<div class="navbar" style="background-color: {bg_color}">
    <button on:click={home}> Home</button>
    <button on:click={about}> About </button>
    <button on:click={contact}> Contact </button>
</div>

<style>
    .navbar {
        color: #fff;
        font-style: normal;
        font-weight: 700;
        font-size: 24px;
        line-height: 36px;
        text-align: center;
    }
</style>
