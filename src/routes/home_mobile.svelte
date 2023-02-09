<script>
    /**
     * @type {any}
     */
    let y;

    import Skillset from "./skillset.svelte";
</script>

<svelte:window bind:innerWidth={y} />
<div class="mobile_bg">
    <div class="px-20">
        <h1 class="mobile_header pt-8">Hello 👋<br />I'm Pooh</h1>

        <img src="./profile_mobile.png" alt="profile" class="mx-auto pt-4" />

        <p class="mobile_p pt-4">
            I'm a computer engineering undergraduate student at Faculty of
            Engineering, Chiang Mai University. <br />
            I’m interested in front-end web development, UX/UI design, computational
            intelligence.
        </p>
        <div class="text-center py-4">
            <button
                class="text-center mobile_contact_button text-black px-8 py-4 rounded-full"
            >
                Contact Me
            </button>
        </div>
    </div>
</div>

<div class="max-w-screen-lg mx-auto pt-4 pb-8 bg-black">
    <div class="py-8">
    <span class="mobile_skill_header pl-20">Skill-Set </span>
    <span class="text-5xl"> ✨</span>
    </div>

    <div class="flex flex-row flex-wrap justify-center">
        <Skillset />
    </div>
</div>

<style>
    
    .mobile_bg {
        font-family: "Prompt", sans-serif;
        background: #7209b7;
        color: #fff;
    }
    .mobile_header {
        font-style: normal;
        font-weight: 700;
        font-size: 2rem;
        line-height: 3rem;
        text-align: center;
    }
    .mobile_p {
        font-style: normal;
        font-weight: 400;
        font-size: 1.125rem;
        line-height: 1.5rem;
    }

    .mobile_contact_button {
        background: #a9def9;
        font-style: normal;
        font-weight: 700;
        font-size: 1rem;
        line-height: 1.5rem;
    }
    .mobile_skill_header {
        font-style: normal;
        font-weight: 700;
        font-size: 3rem;
        line-height: 36px;

        background: linear-gradient(89.23deg, #696eff 0.36%, #f8acff 83.17%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
    }
</style>
