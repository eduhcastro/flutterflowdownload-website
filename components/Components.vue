<style scoped>
    .alert.danger {
    --tw-border-opacity: 1;
    --tw-bg-opacity: .1;
    background-color: #f43f5e1a;
    background-color: rgb(244 63 94 / var(--tw-bg-opacity));
    border-color: #f43f5e;
    border-color: rgb(244 63 94 / var(--tw-border-opacity));
}

.alert.danger {
    --tw-border-opacity: 1;
    --tw-bg-opacity: 0.1;
    background-color: rgba(244, 63, 94, .1);
    background-color: rgb(244 63 94 / var(--tw-bg-opacity));
    border-color: #f43f5e;
    border-color: rgb(244 63 94 / var(--tw-border-opacity));
}
.p-4 {
    padding: 1rem;
}
.border-l-4 {
    border-left-width: 4px;
}
.rounded-bl-sm {
    border-bottom-left-radius: 0.125rem;
}
.rounded-lg {
    border-radius: 0.5rem;
}
.my-8 {
    margin-bottom: 2rem;
    margin-top: 2rem;
}
.relative {
    position: relative;
}
</style>

<template>
    <h1 style="text-align: center;font-size: medium;">Components</h1>

    <div style="height: 120px;margin-top: 15px;">
        <div style="display:flex;justify-content: center;align-items: center;">

            <div>
                <h3 style="font-size: 13px; color: #5e5d5d;">App</h3>
                <div style="display: flex; justify-content: center; align-items: center; height: 40px;">
                    <div>
                        <img style="width: 200px;"
                            src="https://assets-global.website-files.com/635ff61792c1c6ebf4e1edad/6364138a12ac6843f1c23412_flutterflow_logo_black-p-500.png">
                    </div>

                    <div>
                        <img src="https://cdn.icon-icons.com/icons2/2699/PNG/512/electronjs_logo_icon_169208.png"
                            style="width: 200px;">
                    </div>
                </div>
            </div>



            <div>
                <h3 style="font-size: 13px;
color: #5e5d5d;">Website</h3>
                <div style="display: flex; justify-content: center; align-items: center;  height: 40px;">
                    <div>
                        <img src="https://upload.wikimedia.org/wikipedia/commons/6/66/Nuxt_logo_%282021%29.svg"
                            style="width: 170px;">
                    </div>

                    <div>
                        <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5e/Vercel_logo_black.svg/2560px-Vercel_logo_black.svg.png"
                            style="width: 150px;">
                    </div>

                    <div>
                        <img src="/logo.png" style="margin-left: 5px; width: 50px;">
                    </div>
                </div>
            </div>



        </div>

       
    </div>


    <div class="relative p-4 border-l-4 my-8 rounded-lg rounded-bl-sm alert danger">
            <div>
                <h3>Can you help me?.</h3>
                <p>I currently have no computer/laptop to update this project, due to financial situations. Currently I cannot/can't program, due to this difficulty.
                </br>If you can help me, I promise that I will update this project again and do others, as I always have and always will.
                
                <br/> <br/>PayPal: eduh.castro19@gmail.com<br/><br/>

        <b>If you can't, that's okay, you're already helping me a lot by accessing this site, and I'm very grateful for that.</b></p>
    </div>
    </div>


   
</template>