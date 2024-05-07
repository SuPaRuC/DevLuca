<script>
    import Step from "../components/Step.svelte";

    let steps = [
        {name: 'Performance evaluation of a microcloud service of task oﬄoading in vehicular edge computing', icon: 'fa-solid fa-wifi', href: 'assets/progetto_tesi_luca_parenti.pdf'},
        {name: 'MeteoCity', icon: 'fa-solid fa-cloud', href: 'https://github.com/SuPaRuC/MeteoCity'}
    ];

    let benefits = [
        {name: 'a world and technologies explorer', description: 'Just as I have always had curiosity and aspiration to explore the world, so I also have a great desire to understand and learn how (new or unknown) technologies existing works. Curiosity, as Einstein used to say, has a purpose. One can only be amazed when the mysteries of eternity, of life and of the wonderful structure of reality are contemplated. It is enough if one tries to understand only a little of this mystery every day. That’s why I believe that at any age, anywhere and anytime, you can always learn something useful, that you will always carry in the baggage of your personal experience.'},
        {name: 'an hard worker and a perfectionist', description: 'In everything I’ve done so far, from my school education through university and my work experience, I’ve always tried to give 100% of myself. I’m of the opinion that if you want to do something you always have two options: do it right or not do it at all. We are not perfect, it is true, we are human beings, sometimes we can get lost, but the important thing is to always seek a solution to the different problems that can occur by facing them and not bypassing them.'},
        {name: 'a great teammate and motivator', description: 'If the first two points have not convinced you of the fact that I am a good motivator, let me explain my vision in this regard. I love working in a team, because being in contact with other people who have the same passion, allows me to discover and learn new things. Also, the presence of healthy competition always pushes me to show what I’m really capable of. Good teamwork always leads to great results, especially if the people who are part of it not only stimulate each other, but also manage to support and motivate each other to achieve their goals.'},
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
            <a href="#contacts" class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer">
                <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"/>
                <h4 class="relative z-9">Get in touch <i class="fa-solid fa-arrow-right ml-1 text-base"></i></h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <!-- svelte-ignore a11y-img-redundant-alt -->
            <img src={"images/profile.png"} alt="Profile image" class="object-cover z-[2] max-h-[70vh]">
        </div>
    </section>

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
                    This is my thesis project in which I was able to develop <strong class="text-violet-400">intermediate skills in vehicular edge computing</strong>. 
                    The project focuses on the design of a robust and reliable task offloading protocol and its implementation in <strong class="text-violet-400">C++</strong> using the <strong class="text-violet-400">OMNeT++</strong> simulator. 
                    Once the implementation was finished, its performance was <strong class="text-violet-400">analyzed</strong> using graphical <strong class="text-violet-400">python data analysis tools</strong>. 
                </p>
            </Step>

            <Step step={steps[1]}>
                <p class="mt-10">
                    In this university project I was able to develop different skills in <strong class="text-violet-400">web development</strong>. 
                    The site is very simple, but I was able to experiment with different technologies such as <strong class="text-violet-400">JavaScript</strong>, <strong class="text-violet-400">HTML5</strong>, <strong class="text-violet-400">CSS3</strong> and <strong class="text-violet-400">AJAX</strong> for front-end development, while <strong class="text-violet-400">NodeJS</strong> for back-end development. 
                    I was also able to develop the ability to create <strong class="text-violet-400">REST APIs</strong>. 
                    Finally, <strong class="text-violet-400">MongoDB</strong> was used, a non-relational database for saving the weather preferences of each individual user.
                </p>
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
            <div class="flex gap-6 sm:gap-8">
                <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
                    0..
                </p>
                <div class="flex flex-col gap-6 sm:gap-8">
                    <h3 class="text-2xl sm:text-3xl md:text-5xl">
                        a million other things 
                    </h3>
                </div>
            </div>
        </div>
        <h5 class="text-2xl sm:text-3xl font-semibold text-center poppins">
            The <span class="text-violet-400 poppins">complete</span> package.
        </h5>
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 lg:gap-10">
            <a href="assets/CV_Luca_Parenti_IT.pdf" target="_blank" class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-violet-700 text-center group cursor-pointer hover:border-violet-400 duration-200">
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
                            Download <i class="fa-solid fa-arrow-right ml-1 text-base"></i>
                        </p>
                    </div>
                </div>
            </a>

            <a href="assets/CV_Luca_Parenti_EN.pdf" target="_blank" class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-violet-700 text-center group cursor-pointer hover:border-violet-400 duration-200">
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
                            Download <i class="fa-solid fa-arrow-right ml-1 text-base"></i>
                        </p>
                    </div>
                </div>
            </a>
        </div>
    </section>
</main>