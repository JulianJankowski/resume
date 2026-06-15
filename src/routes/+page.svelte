<script>
    // import { render } from 'svelte-email';
    // import nodemailer from 'nodemailer';

    function sendEmail(){
    //     const transporter = nodemailer.createTransport({
    //         host: 'smtp.ethereal.email',
    //         port: 587,
    //         secure: false,
    //         auth: {
    //             user: 'my_user',
    //             pass: 'my_password'
    //         }
    //     });

    //     const options = {
    //         from: 'you@example.com',
    //         to: 'user@gmail.com',
    //         subject: 'hello world',
    //         text: 'test'
    //     };

    //     transporter.sendMail(options);
    }
</script>

<div class="flex">
    <main class="w-full">
        <div class="split-background w-full h-screen text-slate-100">
            <div class="flex container mx-auto columns-1 text-center  size-full min-h-svh items-center">
                <div 
                    class="grid w-full">
                    <h1 class="leading-loose max-md:text-3xl text-5xl col-1">Julian Jankowski</h1>
                    <h2 class="leading-loose max-md:mt-32 max-md:text-3xl text-5xl col-1">Software Developer &#183; Salesforce Consultant</h2>
                </div>
            </div>
        </div>
        <div class="split-background-mirror w-full min-h-screen max-2xl:pt-96 max-2xl:pb-96 ">
            <div class="max-2xl:grid 2xl:flex mx-auto 2xl:columns-3 2xl:gap-[5%] max-2xl:columns-1 max-2xl:space-y-96 min-h-svh items-center justify-center justify-items-center">
                <div class=" p-10 border-solid border-4 border-slate-600 hover:border-teal-200 text-slate-50 max-md:h-max max-md:w-[20rem] h-[30rem] w-[30rem] rounded rounded-3xl bg-gradient-to-b from-teal-500 to-blue-600 h-1/3 transition duration-150 ease-out hover:scale-110">
                    <h3 class="leading-loose text-4xl">Developer</h3>
                    <p class="leading-loose text-xl min-md:text-2xl">Full Stack Developer, with skills in Python, JavaScript, TypeScript, Java, and more.</p>
                    <p class="leading-loose text-2xl">Agile team collaborator, and independant worker</p>
                </div>
                <div class="p-10 border-solid border-4 border-slate-600 hover:border-teal-200 text-slate-50 max-md:h-max max-md:w-[20rem] h-[30rem] w-[30rem] rounded rounded-3xl bg-gradient-to-b from-blue-600 to-fuchsia-600 h-1/3 transition duration-150 ease-out hover:scale-110">
                    <h3 class="leading-loose text-4xl">Collaborator</h3>
                    <p class="leading-loose text-2xl">Extensive use of git, Jira, and Confluence for development and documentation</p>
                    <p class="leading-loose text-2xl">Experience with developing devops processes with GitHub Actions and Bitbucket Pipelines</p>
                </div>
                <div class="p-10 border-solid border-4 border-slate-600 hover:border-teal-200 text-slate-50 max-md:h-max max-md:w-[20rem] h-[30rem] w-[30rem] rounded rounded-3xl bg-gradient-to-b from-fuchsia-600 to-rose-600 h-1/3 transition duration-150 ease-out hover:scale-110">
                    <h3 class="leading-loose text-4xl">Hobbyist</h3>
                    <p class="leading-loose text-2xl">Gym Enthusiast</p>
                    <p class="leading-loose text-2xl">Lawn Fanatic</p>
                    <p class="leading-loose text-2xl">Bouldering Amateur</p>
                </div>
            </div>
        </div>
        <div class="flex container w-screen h-screen text-slate-100 p-16">
            <div class="w-1/2 m-32">
                <h2 class="text-3xl pb-16">Contact</h2>
                <form>
                    <h3 class="text-2xl">Email</h3>
                    <input 
                        type="email" 
                        name="email" 
                        id="email"
                        autocomplete="email"
                        class="mt-4 block w-full rounded-md border-0 py-1.5 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6">

                    <h3 class="text-2xl pt-6">Body</h3>
                    <textarea
                        name="body" 
                        id="body"
                        class="mt-4 block w-full rounded-md border-0 py-1.5 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6"></textarea>
                    <button type="submit" on:click={sendEmail} class="mt-6 text-2xl bg-primary hover:text-teal-200">Send</button>
                </form>
            </div>
        </div>
    </main>
</div>
 


