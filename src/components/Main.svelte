<script>
    import Step from "../components/Step.svelte";

    let steps = [
        {name: 'Performance evaluation of a microcloud service of task oﬄoading in vehicular edge computing', icon: 'fa-solid fa-wifi', href: 'assets/task_offloading.zip'},
        {name: 'MeteoCity', icon: 'fa-solid fa-cloud', href: 'https://github.com/SuPaRuC/MeteoCity'}
    ];

    let benefits = [
        {name: 'a world and technologies explorer', description: 'description'},
        {name: 'an hard worker and details fanatic', description: 'description'},
        {name: 'a great teammate and motivator', description: 'description'},
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class="font-semibold text-4xl  sm:text-5xl md:text-6xl">
                Hi, I'm <span class="poppins text-violet-400">Luca</span> Parenti! <br>
                Software <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400">favourite tech</span> includes <b class="font-bold">Java</b>, <b class="font-bold">C/C++</b> and <b class="font-bold">Linux</b>! <br>
                Other technologies I have <span class="text-violet-400">interest</span> into:
            </p>
            <p class="text-4xl sm:text-5xl md:text-6xl">
                <i class="fa-brands fa-python"></i>
                <i class="fa-brands fa-php"></i>
                <i class="fa-brands fa-laravel"></i>
                <i class="fa-brands fa-html5"></i>
                <i class="fa-brands fa-css3"></i>
                <i class="fa-brands fa-js"></i>
                <i class="fa-brands fa-git-alt"></i>
            </p>
            <!-- svelte-ignore a11y-invalid-attribute -->
            <!-- TODO insert link to contacts -->
            <a href="#" target="_blank" class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer">
                <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"/>
                <h4 class="relative z-9">Get in touch <i class="fa-solid fa-arrow-right ml-1 text-base"></i></h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <!-- svelte-ignore a11y-img-redundant-alt -->
            <img src={"images/profile.png"} alt="Profile image" class="object-cover z-[2] max-h-[70vh]">
        </div>
    </section>

    <!-- TODO Finish description of projects -->
    <section id="projects" class="py-20 lg:py32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of my projects
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    This project focus on <strong class="text-violet-400">C++</strong>
                </p>
            </Step>

            <Step step={steps[1]}>
            </Step>
        </div>
    </section>

    <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . . 
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>
                            {benefit.description}
                        </p>
                    </div>
                </div>
            {/each}
        </div>
        <h5 class="text-2xl sm:text-3xl font-semibold text-center poppins">
            The <span class="text-violet-400 poppins">complete</span> package.
        </h5>
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 lg:gap-10">
            <a href="assets/cv_parenti_luca_it.pdf" target="_blank" class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-violet-700 text-center group cursor-pointer hover:border-violet-400 duration-200">
                <div class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200">
                    <i class="fa-solid fa-i"></i>
                </div>
                <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">
                    Curriculum Vitae - Italian version
                </h3>
                <slot/>
                <div class="flex-1 flex justify-between gap-4 items-center">
                    <div class="ml-auto cursor-pointer hover:text-slate-950 duration-200 relative after:absolute after:top-0 after:h-0 after:right-full after:w-full after:h-full after:bg-white after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden">
                        <p class="relative z-4">
                            Go to <i class="fa-solid fa-arrow-right ml-1 text-base"></i>
                        </p>
                    </div>
                </div>
            </a>

            <a href="assets/cv_parenti_luca_en.pdf" target="_blank" class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-violet-700 text-center group cursor-pointer hover:border-violet-400 duration-200">
                <div class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200">
                    <i class="fa-solid fa-e"></i>
                </div>
                <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">
                    Curriculum Vitae - English version
                </h3>
                <slot/>
                <div class="flex-1 flex justify-between gap-4 items-center">
                    <div class="ml-auto cursor-pointer hover:text-slate-950 duration-200 relative after:absolute after:top-0 after:h-0 after:right-full after:w-full after:h-full after:bg-white after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden">
                        <p class="relative z-4">
                            Go to <i class="fa-solid fa-arrow-right ml-1 text-base"></i>
                        </p>
                    </div>
                </div>
            </a>
        </div>
    </section>
</main>