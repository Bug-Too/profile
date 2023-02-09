<script>
    import { count } from "../store.js";

    let bg_color = "#7209B7";
    let home_selected = "border-2 rounded-full px-2";
    let about_selected = "";
    let contact_selected = "";

    function home() {
        count.set(0);
        bg_color = "#7209B7";
        home_selected = "border-2 rounded-full px-2";
        about_selected = "";
        contact_selected = "";
    }
    function about() {
        count.set(1);
        bg_color = "#000000";
        about_selected = "border-2 rounded-full px-2";
        home_selected = "";
        contact_selected = "";
    }
    function contact() {
        count.set(2);
        bg_color = "#000000";
        contact_selected = "border-2 rounded-full px-2";
        home_selected = "";
        about_selected = "";
    }

    let width = 1920;
</script>

<svelte:window bind:innerWidth={width}/>
{#if width > 1024}
<div style="background-color: {bg_color}">
    <div
        class="pt-4 navbar text-right flex flex-row place-content-end place-item-center place-self-center max-w-screen-lg mx-auto"
    >
        <div class="px-2">
            <a href="/#"><button on:click={home} class={home_selected}> Home </button></a>
        </div>
        <div class="px-2">
            <a href="/#/about"><button on:click={about} class={about_selected}> About </button></a>
        </div>
        <div class="px-2">
            <a href="/#/contact">
                            <button on:click={contact} class={contact_selected}>
                Contact
            </button>
            </a>

        </div>
    </div>
</div>
{:else}
<div style="background-color: {bg_color}">
    <div
        class="pt-4 navbar text-right flex flex-row place-content-center place-item-center place-self-center max-w-screen-lg mx-auto"
    >
        <div class="px-2">
            <a href="/#"><button on:click={home} class={home_selected}> Home </button></a>
        </div>
        <div class="px-2">
            <a href="/#/about"><button on:click={about} class={about_selected}> About </button></a>
        </div>
        <div class="px-2">
            <a href="/#/contact">
                            <button on:click={contact} class={contact_selected}>
                Contact
            </button>
            </a>

        </div>
    </div>
</div>
{/if}

<style>
    .navbar {
        color: #fff;
        font-style: normal;
        font-weight: 700;
        font-size: 24px;
        line-height: 36px;
    }
    .nav_button {
        border-style: solid;
        border: 10px;
        border-color: black;
    }
</style>
