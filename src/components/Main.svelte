<script>

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
                Other technologies I have <span class="text-violet-400">interest</span> into 
                <i class="fa-brands fa-python"></i>
                <i class="fa-brands fa-php"></i>
                <i class="fa-brands fa-laravel"></i>
                <i class="fa-brands fa-html5"></i>
                <i class="fa-brands fa-css3"></i>
                <i class="fa-brands fa-js"></i>
                <i class="fa-brands fa-git-alt"></i>
            </p>
            <!-- svelte-ignore a11y-invalid-attribute -->
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
</main>