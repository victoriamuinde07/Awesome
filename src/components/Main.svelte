<script>
    import Step from "./Step.svelte";

    let steps =[
        {name: 'riaor restaurant', icon: 'fa-solid fa-utensils'},
        {name: 'riaor construction', icon: 'fa-solid fa-house-circle-check'},
        
    ]
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class= "font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm<span class="poppins text-violet-400">Victoria</span> Mwikali <br/> Data Scientist
                <span class="poppins text-violet-400">Web Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400">Favorite tech</span> includes python,javascript(SvelteKit,Tailwindcss,node js)
                + Firebase
            </p>
            <a class ="blueshadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 group rounded-full bg-white text-slate-950 cursor_position">
                <div class = "absolute top-0 right-full w-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                href ="#"
                target = "_blank"></div>
                <h4 class="relative z-9">Get in touch</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img src={"images/profile.png.jpg"} alt="Profile image" 
            class="object-cover z-[2] max-h-[100vh]"/>
        </div>
    </section>
    <section id="projects" class="py-20 lg:py-20 flex flex-col gap-10">
        <div class="flex flex-col gap-1 text-center">
            <h5 class="text-lg sm:text md:text-4xl">
                Sample projects worked on
            </h5><b></b>
            <h3 class="text-lg sm:text-xl md:text-3xl"><b></b>
                Curious to <span class="poppins text-violet-400"> see </span> my work
            </h3><b>

            </b>
            <a href="https://riaor-restaurant.vercel.app/"target ="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0
            -at-10 hover:border-violet-700 duration-200"><b></b>
            <i class ="fa-regular fa-circle-play"></i>
            <p> click on me </p>
        </a>
        <div class="grid grid-cols-2 lg:grid-cols-2 gap-15 lg:gap-20">
        <b>
            <Step step={steps[0]}>

            </Step></b>
        <b>
            <Step step={steps[1]}>
                
            </Step></b>
       
        </div>
        </div>
    </section>
</main>