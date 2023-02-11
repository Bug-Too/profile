<script>
    let name = "";
    let email = "";
    let message = "";

    async function handleSubmit() {
        alert("505 error");
        const response = await fetch(
            "",
            {
                method: "POST",
                headers: { "Content-Type": "application/json" },
                body: JSON.stringify({ name, email, message }),
            }
        );

        const result = await response.json();
        console.log(result);
    }
</script>

<div class="contact h-screen px-8">
    <div class="max-w-screen-lg mx-auto">
        <h1 class="main_header">Contact</h1>
        <form on:submit|preventDefault={handleSubmit}>
            <label for="name" class="text-white">Name</label>
            <div class="py-2">
                <input
                    type="text"
                    id="name"
                    bind:value={name}
                    placeholder="Your name"
                    class="w-full py-4 px-4 rounded-xl"
                />
            </div>
            <label for="email" class="text-white">Email</label>
            <div class="py-2">
                <input
                    type="email"
                    id="email"
                    bind:value={email}
                    placeholder="Your email"
                    class="w-full py-4 px-4 rounded-xl"
                />
            </div>
            <label for="message" class="text-white">Message</label>
            <div class="py-2">
                <textarea
                    bind:value={message}
                    rows="8"
                    placeholder="Your message"
                    class="w-full py-4 px-4 rounded-xl"
                />
            </div>
            <div class="text-center pt-8">
                <button type="submit" class="submit_btn px-12 py-2 rounded-2xl"
                    >Submit</button
                >
            </div>
        </form>

    </div>
    <div class="contact">
        <div class="pt-12 flex flex-row items-center max-w-screen-lg mx-auto">
            <div>
                <a href="https://github.com/Bug-Too"
                    ><img src="./github.svg" alt="github_white" /></a
                >
            </div>

            <div class="text-white pl-5">
                <a href="mailto:purichseenuallae@gmail.com"
                    >Email: purichseenuallae@gmail.com <br /></a
                >
                <a href="tel:0972791224">Tel: 0972791224</a>
            </div>
        </div>
    </div>
</div>

<style>
    .contact {
        background-color: #000000;
    }
    .main_header {
        font-style: normal;
        font-weight: 700;
        font-size: 5rem;
        line-height: 145px;

        background: linear-gradient(89.23deg, #696eff 0.36%, #f8acff 83.17%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
    }
    .submit_btn {
        background: #a9def9;
        font-style: normal;
        font-weight: 700;
        font-size: 32px;
        line-height: 48px;
        text-align: center;
    }
</style>
