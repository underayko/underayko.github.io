<script>
    import { onMount } from 'svelte';

    export let year = new Date().getFullYear();

    let scrollAnimationClass = '';

    onMount(() => {
        const handleScroll = () => {
            scrollAnimationClass = window.scrollY > 0 ? 'bg-[#04060f] shadow-lg text-white' : 'bg-transparent text-black';
        };
        window.addEventListener('scroll', handleScroll);
        return () => window.removeEventListener('scroll', handleScroll);
    });

    const scrollToTop = () => {
        window.scrollTo({ top: 0, behavior: 'smooth' });
    };

    let projects = [
        {
            title: "Portfolio Website",
            image: "src/images/unfoldap.png",  // Image path
            description: "A portfolio website for students showcasing their skills and projects.",
            experience: "This project helped me to enhance my web development skills, especially in JavaScript and its framework, Angular. I learned how to create responsive layouts and improve user experience through clean design. I also learned how to communicate with other people since this project is by group.",
            link: "https://underayko.github.io/myportfolio/"
        },
        {
            title: "Blog Website",
            image: "src/images/blog.png",  // Image path
            description: "A blogging platform allowing users to create and share blog posts.",
            experience: "Working on this blog application expanded my knowledge in backend development and database management. I implemented user authentication, rich text editing, and more features and also learned to manage state effectively.",
            link: "https://github.com/yourusername/blog-application"
        },
        // Add more projects here
    ];
</script>

<!-- Fixed Header -->
<header class={`fixed top-0 left-0 w-full flex justify-between items-center p-2 transition-all duration-300 ${scrollAnimationClass} z-10`}>
    <div role="button" tabindex="0" on:click={scrollToTop} on:keydown={(e) => e.key === 'Enter' && scrollToTop()} class="text-2xl font-bold cursor-pointer">ELPZ</div>

    <div class="text-2xl">My Projects</div>
</header>

<!-- Projects Section -->
<section id="projects" class="pt-20 bg-[#f5f5f5] py-10">
    <div class="container mx-auto px-4">
        <h2 class="text-3xl text-center font-bold text-[#04060f] mb-10 font-playfair">My Projects</h2>
        <div class="flex flex-col gap-8">
            {#each projects as project}
                <div class="bg-white rounded-lg shadow-lg p-6 flex flex-col">
                    <h3 class="text-xl font-semibold text-[#04060f] font-playfair mb-2">{project.title}</h3>
                    <img src={project.image} alt={project.title} class="w-full h-100 object-cover rounded mb-4" /> <!-- Set a fixed height for consistency -->
                    <p class="text-gray-600 my-2 flex-grow">{project.description}</p>
                    <p class="text-gray-600 my-2">{project.experience}</p>
                    
                </div>
            {/each}
        </div>
    </div>
</section>

<footer class="bg-[#04060f] text-white text-center p-4 mt-auto">
    <div class="container mx-auto">
        <p class="font-playfair">&copy; {year} My Portfolio. All rights reserved.</p>
    </div>
</footer>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Raleway:wght@400;700&display=swap');


    header {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        z-index: 10;
        transform: translateY(0);
        transition: transform 0.3s ease;
    }
    
    section {
        padding-top: 6rem; /* Adjusting for fixed header */
    }
</style>
