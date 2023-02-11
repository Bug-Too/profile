<script>
    import ExpCard from "./expCard.svelte";
</script>

<div class="background">
    <div class="max-w-screen-lg mx-auto px-8">
        <h1 class="main_header">About</h1>
        <p class="paragraph">
            I'm a computer engineering undergraduate student at Chiang Mai
            University with a passion for front-end web development, UX/UI
            design, and computational intelligence. With a commitment to
            excellence and a drive to stay ahead in my field, I deliver results
            -driven solutions for every project. Let's work together to bring
            your technology to the next level.
        </p>
        <h2 class="sub_header pt-14 py-2">Resume</h2>
        <iframe title="Resume" src="https://drive.google.com/file/d/1A-74kZS2Nhb0vQy_tp2fnsFKbNyXJjT_/preview" style="width:100%;height:50rem;" ></iframe>
        <h2 class="sub_header pt-14 py-2">Project</h2>
        <div class="flex flex-row flex-wrap justify-center">

            <ExpCard
                title="Plastic Model Online Shop"
                img_src="/online_model_shop.png"
                link="https://github.com/RiwEZ/Database-WebProject"
                description="My first project using Laravel and Sql. It features basic online shop functionalities - browsing, buying products, and check-out."
                tech="Website - React / Laravel / Sql"
            />
            <ExpCard
                title="CARIN"
                img_src="/carin.png"
                link="https://github.com/PutawanDE/ExpensivePigCARIN"
                description="It is a single-player online strategy game. It features genetic code parser and interpreter for game's characters, and multi-threaded server support for concurrent playing games."
                tech="Game - Java Spring WebSocket / React / TypeScript / CSS / HTML"
            />

            <ExpCard
                title="Multilayer Perceptron from Scratch"
                img_src="/mlp.png"
                link="https://github.com/Bug-Too/CI-Assignment-1-V2.git"
                description="I implemented an MLP from scratch using Python. I used Back Propagation,and Genetic Algorithms to train a network"
                tech="Computational Intelligence - Python"
            />
            <ExpCard
                title="Crown of Madness"
                img_src="/ggj.png"
                link="https://putawan-de.itch.io/crown-of-madness"
                description="My first Global Game Jam, The Global Game Jam (GGJ) is a unique free event held worldwide among game creators. Participants come together and work to develop original and innovative experimental video games based on a secret theme."
                tech="Game - C# / Unity"
            />

        </div>
        <h2 class="sub_header pt-14 py-2">Experience</h2>
        <div class="flex flex-row flex-wrap justify-center">
            <ExpCard
            title="IDC Robocon 2022"
            img_src="/IDC.png"
            link="http://www.idc-robocon.org/idc2022_eng/index.html"
            description="Due to COVID19, I collaborated online to develop a robot with people from China, South Korea, and Mexico. I learnt how to collaborate project's implementation with people from around the world over the course of 10 days, as well as how to use Unity's physics engine and 3D modelling tools to create a robot."
            tech="Competition - Unity C#"
        />
            <ExpCard
                title="PTT Young GENergy"
                img_src="/ptt_yg.jpg"
                link="https://www.nationtv.tv/pr-news/news/pr/378897483"
                description="Young GENergy is an camp held by PTT crop and I have learn about energy ,how to conserve and learn how to share knowledge effectively."
                tech="Energy Program"
            />
            <ExpCard
                title="Politics Hackathon"
                img_src="/ph.png"
                link=""
                description= "First place winner Hackathon in topic Participation of the people in amending the constitution and proposing policies online organized by King Prajadhipok's Institute CMU School of Lifelong Education Konrad-Adenauer-Stiftung Thailand Instiutute of Democratization Studies (iDS) OpenDream and Conlab"
                tech="Hackathon"
            />
            <ExpCard
                title="Thailand Energy Academy"
                img_src="/TEA.jpeg"
                link=""
                description="I have duly satisfied and fulfilled the requirements of the course in Energy Literacy for a Sustainable Future, which is a course organized by the Thailand Energy Academy, Ministry of Energy and PTT group, Thailand."
                tech="Energy Academy"
            />
            <ExpCard
                title="Smogathon"
                img_src="/Smogathon.png"
                link=""
                description="First place winner hackathon our team design an airship that can communicate each nodes and report when detect a fire."
                tech="Hackaton"
            />
            <ExpCard
            title="JALESEA"
            img_src="/JALESEA.jpg"
            link=""
            description="I have finished Japanese course JALESEA is Japanese 2 years course held by Language Institute, Chiang Mai University."
            tech="Japanese Course"
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
</style>
