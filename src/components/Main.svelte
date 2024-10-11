<script>
    import Step from "./Step.svelte";

    let steps =[
        {name: 'Riaor restaurant', icon: 'fa-solid fa-utensils'},
        {name: 'Customer Churn Prediction', icon: 'fa-solid fa-house-circle-check'},
        
    ];
    let benefits = [
        {name: 'a self taught developer',description: 'I am a passionate web developer and Data Science Enthusiast,thrilled and a fanatic learner and adapting to new technology advancements'},
        {name: 'a web developer and Data scientist',description:'I love the challenge of learning new design concepts and enabling users with amazing online experiences'},
        {name: 'an excellent communicator',description: 'I believe in transparency and constructive communication above all else'},
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h1 class= "font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm<span class="poppins text-violet-400"> Victoria </span> Mwikali <br/> Data Scientist
                <span class="poppins text-violet-400">Web Developer</span>
            </h1>

            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400">Favorite tech</span> includes python,javascript(SvelteKit,Tailwindcss,node js)
                + Firebase
            </p>

            <a class="blueshadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 group rounded-full bg-white text-slate-950 cursor_position" href="#">
                <div class="absolute top-0 right-full w-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"></div>
                <h4 class="relative z-9">Get in touch</h4>
            </a>
                <div class="relative shadow-2xl grid place-items-center">

                </div>

                <img src={"images/profile.png.jpg"} alt="Profile image" class="object-cover z-[1] max-h-[80vh]">
        </div>
    </section>
    <section id="projects" class="py-20 lg:py-20 flex flex-col gap-10">
        <div class="flex flex-col gap-1 text-center">
            <h5 class="text-lg sm:text md:text-4xl">
                Sample projects worked on
            </h5>
        
            <h3 class="text-lg sm:text-xl md:text-3xl">
                Curious to <span class="poppins text-violet-400"> see </span> my work
            </h3>
            <a href="https://riaor-restaurant.vercel.app/"target ="_blank" class="mx-auto px-4 py-2 rounded-md border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -at-10 hover:border-violet-700 duration-200">
            <i class ="fa-regular fa-circle-play"></i>
            <p> click on me </p>
        </a>
            <div class="grid grid-cols lg:grid-cols-2 gap-15 lg:gap-20">
    
                <Step step={steps[0]}>
                    <p>Riaor Restaurant is a website created with
                     <strong class="text-violet-400">SCSS,Bootstrap,js,html</strong>
                    </p>
                </Step>
        
                <Step step={steps[1]}>
                    <p>Customer Churn Prediction is a data science project where
                        <strong class="text-violet-400"> a churning predictive model is created.</strong>
                    </p>
                </Step>
            </div>
        </div>
    </section>
    <section id="about" class="py-20 pt-10 lg:pt-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
    <div class="flex flex-col gap-2 text-center relative before:absolute before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
    >
        <h6 class ="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
        <h3 class="font-semibold text-3xl sm:text-5xl"> A bit <span class ="poppins text-violet-400">about</span> me.</h3>
    </div>
    <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">I am a passionate web developer and Data Science Enthusiast,thrilled and a fanatic of 
        learner and adapting to new technology advancements </p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
        {#each benefits as benefit, index}
            <div class="flex flex-col gap-6 sm:gap-8">
                <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-550 font-semibold">
                0{index+1}
                </p>
                <div class="flex flex-col gap-6 sm:gap-8">
                <h3 class="text-2xl sm:text-3xl md:text-5xl">
                    {benefit.name}
                </h3>
                <p>{benefit.description}</p>
                </div>
            </div>
        {/each}
    </div>
    <h5 class="text-2xl sm:text-3xl font-semibold text-center poppins"> The <span class="text-violet-400 poppins"> Complete </span> Package</h5>
    <div class = "flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
        <table class ="bg-white text-slate-700 rounded text-center">
            <thead class="border-b border-solid border-slate-200">
                <tr class="">
                    <th class = "whitespace-nowrap p-2 px-4">Candidate #1</th>
                    <th class = "whitespace-nowrap p-2 px-4">Candidate #2</th>
                    <th class = "whitespace-nowrap p-2 px-4">Candidate #3</th>
                    <th class = "whitespace-nowrap bg-violet-700 text-white p-4 px-8">Me</th>
                </tr>
            </thead>
            <tbody>
                <tr class="border-b border-solid border-slate-200">
                    <td class = "border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">Dedication</td>
                    <td><i class="fa-solid fa-check text-slate-500"></i></td>
                    <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                    <td><i class="fa-solid fa-check text-slate-500"></i></td>
                    <td><i class="fa-solid fa-check text-green-500"></i></td>
                </tr>
                <tr class="border-b border-solid border-slate-200">
                    <td class = "border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">Critical Thought</td>
                    <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                    <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                    <td><i class="fa-solid fa-check text-slate-500"></i></td>
                    <td><i class="fa-solid fa-check text-green-500"></i></td>
                </tr>
                <tr class="border-b border-solid border-slate-200">
                    <td class = "border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">Interpersonal skills</td>
                    <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                    <td><i class="fa-solid fa-check text-slate-500"></i></td>
                    <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                    <td><i class="fa-solid fa-check text-green-500"></i></td>
                </tr>
            </tbody>
        </table>
    </div>
    <div class = "mx-auto -mt-12 italic sm:hidden opacity-50">
        <p>Scroll to see more &rarr;</p>
    </div>
    <p class="mx-auto">So why not invest?
    </section>
</main>