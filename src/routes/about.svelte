<script>
    import ExpCard from "./expCard.svelte";
</script>

<div class="background">
    <div class="max-w-screen-lg mx-auto">
        <h1 class="main_header">About</h1>
        <p class="paragraph">
            I'm a computer engineering undergraduate student at Chiang Mai
            University with a passion for front-end web development, UX/UI
            design, and computational intelligence. With a commitment to
            excellence and a drive to stay ahead in my field, I deliver results
            -driven solutions for every project. Let's work together to bring
            your technology to the next level.
        </p>
        <h2 class="sub_header pt-14 py-2">Project</h2>
        <div class="grid-container">
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
        </div>
        <h2 class="sub_header pt-14 py-2">Experience</h2>
        <div class="grid-container">
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="UI/UX Designer"
                img_src="/paint_icon.png"
                link="https://www.google.com"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
        </div>
    </div>
</div>

<style>
    .background {
        background-color: #000000;
    }
    .main_header {
        font-style: normal;
        font-weight: 700;
        font-size: 96px;
        line-height: 145px;

        background: linear-gradient(89.23deg, #696eff 0.36%, #f8acff 83.17%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
    }
    .sub_header {
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
    .paragraph {
        font-style: normal;
        font-weight: 400;
        font-size: 24px;
        line-height: 36px;

        color: #ffffff;
    }
    .grid-container {
        display: grid;
        grid-template-columns: auto auto auto;
    }
</style>
