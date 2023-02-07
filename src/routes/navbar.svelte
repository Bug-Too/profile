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
</script>

<div style="background-color: {bg_color}">
    <div
        class="pt-4 navbar text-right flex flex-row place-content-end place-item-center place-self-center max-w-screen-lg mx-auto"
    >
        <div class="px-2">
            <button on:click={home} class={home_selected}> Home </button>
        </div>
        <div class="px-2">
            <button on:click={about} class={about_selected}> About </button>
        </div>
        <div class="px-2">
            <button on:click={contact} class={contact_selected}>
                Contact
            </button>
        </div>
    </div>
</div>

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
