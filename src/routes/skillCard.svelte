<script>
    /**
     * @type {string}
     */
    export let title;
    /**
     * @type {any}
     */
    export let img_src;
</script>

<div class="px-4 pt-4">
    <div class="grid-item card">
        <img src={img_src} alt="example" class="pt-2" />
        <h1 class="text-2xl text-center pt-14">{title}</h1>
    </div>
</div>

<style>
    .card {
        width: 20rem;
        height: 20rem;
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
</style>
