<script>
    import SkillCard from "./skillCard.svelte";
    import Skillset from "./skillset.svelte";
</script>

<div class="">
    <div class="home-header ">
        <div class="grid-container max-w-screen-lg mx-auto pt-4">
            <div class="pr-4">
                <h1 class="greeting">Hello 👋 <br />I'm Pooh</h1>
                <p class="sub-greeting">
                    I'm a computer engineering undergraduate student at Faculty
                    of Engineering, Chiang Mai University.<br />
                    -------------------------------- <br />I’m interested in
                    front-end web development, UX/UI design, computational
                    intelligence.
                </p>
            </div>
            <div class=" profile-img">
                <img
                    src="/profile_img.png"
                    alt="profile_image"
                    class="profile-img pt-24"
                />
            </div>
            <div class=" pl-4 pt-16">
                <h1 class="greeting"><br /><br /></h1>
                <p class="quote">
                    " Empowering the digital world, one line of code at a time.
                    "
                </p>
                <div class="pt-8">
                    <a href="mailto:purichseenuallae@gmail.com"><button
                        class="contact_button text-black px-8 py-6 rounded-full "
                    >
                        Contact Me
                    </button></a>
                    
                </div>
            </div>
        </div>
    </div>
    <div class="home-body pb-8">
        <div class="max-w-screen-lg mx-auto pt-4">
            <span class="gradient-header">Skill-Set </span>
            <span class="text-5xl"> ✨</span>
            <div class="grid-container justify-center">
                <Skillset />
            </div>
        </div>
    </div>
</div>

<style>
    .contact_button {
        background: #a9def9;
        font-style: normal;
        font-weight: 700;
        font-size: 32px;
        line-height: 48px;
        text-align: center;
    }
    .gradient-header {
        font-style: normal;
        font-weight: 700;
        font-size: 48px;
        line-height: 73px;

        /* identical to box height */

        background: linear-gradient(89.23deg, #696eff 0.36%, #f8acff 83.17%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
    }
    .greeting {
        color: #fff;
        font-style: normal;
        font-weight: 700;
        font-size: 64px;
        line-height: 97px;
        text-align: left;
    }

    .sub-greeting {
        color: #fff;
        font-style: normal;
        font-weight: 400;
        font-size: 24px;
        line-height: 36px;
        text-align: left;
        padding-top: 80px;
    }

    .grid-container {
        display: grid;
        grid-template-columns: auto auto auto;
    }
    .home-header {
        background-color: #7209b7;
        color: #fff;
    }
    * {
        font-family: "Prompt", sans-serif;
        box-sizing: border-box;
    }

    .profile-img {
        width: 20.6rem;
    }
    .quote {
        font-size: 2rem;
        /* font-weight: 500; */
        font-style: normal;
        font-weight: 700;
        line-height: 54px;

        text-align: center;
    }
    .home-body {
        background-color: #000;
    }
    /* card in rem */
</style>
