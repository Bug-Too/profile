<script>
    /**
     * @type {string}
     */
    export let title;
    /**
     * @type {any}
     */
    export let img_src;

    /**
     * @type {string}
     */
    export let description;

    /**
     * @type {string}
     */
    export let link;

    /**
     * @type {string}
     */
    export let tech;
</script>

<div class="px-4 pt-4">
    <div class="grid-item card">
        <img src={img_src} alt="example" class="pt-2" />
        <a href={link}><h1 class="text-2xl text-center pt-14">🔗{title}</h1></a>
        <p class="cardp px-8 py-4">
            {description}
        </p>
        <p class="cardp px-8 pb-8 text-sky-500">
            {tech}
        </p>
    </div>
</div>

<style>
    .card {
        width: 20rem;
        /* height: 20rem; */
        background-color: #fff;
        border-radius: 0.5rem;
        box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.15);

        font-family: "Prompt", sans-serif;
        font-style: normal;
        font-weight: 700;
        font-size: 40px;
        line-height: 60px;
        text-align: center;

        color: #000000;
    }
    .cardp {
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 24px;
        text-align: left;
    }
</style>
