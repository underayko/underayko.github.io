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
</script>

<!-- Fixed Header -->
<header class={`fixed top-0 left-0 w-full flex justify-between items-center p-2 transition-all duration-300 ${scrollAnimationClass} z-10`}>
    <div class="text-2xl font-bold cursor-pointer" on:click={scrollToTop}>ELPZ</div>
    <div class="text-2xl">My Skills</div>
</header>

<!-- Skills Section -->
<section id="skills" class="pt-24 py-12 bg-[#f5f5f5]">
    <h2 class="text-4xl font-bold text-[#04060f] mb-10 text-center font-playfair">My Skills</h2>
    
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 px-4">
        <!-- Skill Item -->
        <div class="skill-item flex flex-col items-center bg-white p-6 rounded-lg shadow-md transition-transform duration-300 transform hover:scale-105">
            <span class="text-6xl mr-4">💻</span>
            <div class="flex-1 text-center">
                <h3 class="text-lg font-semibold font-playfair">Coding</h3>
                <p class="text-sm text-gray-600">Proficient in languages such as JavaScript, Python, and C++. Passionate about developing efficient and scalable applications.</p>
                <div class="relative mt-2">
                    <div class="progress-bar bg-gray-300 h-2 rounded"></div>
                    <div class="progress-indicator bg-[#04060f] h-2 rounded absolute top-0 left-0" style="width: 40%;"></div>
                </div>
            </div>
        </div>

        <div class="skill-item flex flex-col items-center bg-white p-6 rounded-lg shadow-md transition-transform duration-300 transform hover:scale-105">
            <span class="text-6xl mr-4">🖼️</span>
            <div class="flex-1 text-center">
                <h3 class="text-lg font-semibold font-playfair">Picture Editing</h3>
                <p class="text-sm text-gray-600">Skilled in using Adobe Photoshop and Illustrator for enhancing and creating visual content.</p>
                <div class="relative mt-2">
                    <div class="progress-bar bg-gray-300 h-2 rounded"></div>
                    <div class="progress-indicator bg-[#04060f] h-2 rounded absolute top-0 left-0" style="width: 70%;"></div>
                </div>
            </div>
        </div>

        <div class="skill-item flex flex-col items-center bg-white p-6 rounded-lg shadow-md transition-transform duration-300 transform hover:scale-105">
            <span class="text-6xl mr-4">🎥</span>
            <div class="flex-1 text-center">
                <h3 class="text-lg font-semibold font-playfair">Video Editing</h3>
                <p class="text-sm text-gray-600">Experienced with video editing software like Adobe Premiere Pro and Final Cut Pro.</p>
                <div class="relative mt-2">
                    <div class="progress-bar bg-gray-300 h-2 rounded"></div>
                    <div class="progress-indicator bg-[#04060f] h-2 rounded absolute top-0 left-0" style="width: 75%;"></div>
                </div>
            </div>
        </div>

        <div class="skill-item flex flex-col items-center bg-white p-6 rounded-lg shadow-md transition-transform duration-300 transform hover:scale-105">
            <span class="text-6xl mr-4">🎨</span>
            <div class="flex-1 text-center">
                <h3 class="text-lg font-semibold font-playfair">Sketching</h3>
                <p class="text-sm text-gray-600">Creative in various forms of traditional and digital sketching, with a strong sense of aesthetics.</p>
                <div class="relative mt-2">
                    <div class="progress-bar bg-gray-300 h-2 rounded"></div>
                    <div class="progress-indicator bg-[#04060f] h-2 rounded absolute top-0 left-0" style="width: 85%;"></div>
                </div>
            </div>
        </div>

        <div class="skill-item flex flex-col items-center bg-white p-6 rounded-lg shadow-md transition-transform duration-300 transform hover:scale-105">
            <span class="text-6xl mr-4">🔐</span>
            <div class="flex-1 text-center">
                <h3 class="text-lg font-semibold font-playfair">Cyber Security</h3>
                <p class="text-sm text-gray-600">Knowledgeable about data protection and secure coding practices to safeguard applications.</p>
                <div class="relative mt-2">
                    <div class="progress-bar bg-gray-300 h-2 rounded"></div>
                    <div class="progress-indicator bg-[#04060f] h-2 rounded absolute top-0 left-0" style="width: 40%;"></div>
                </div>
            </div>
        </div>

        <div class="skill-item flex flex-col items-center bg-white p-6 rounded-lg shadow-md transition-transform duration-300 transform hover:scale-105">
            <span class="text-6xl mr-4">✒️</span>
            <div class="flex-1 text-center">
                <h3 class="text-lg font-semibold font-playfair">Lettering</h3>
                <p class="text-sm text-gray-600">Talented in creating beautiful typography and lettering styles for digital and print media.</p>
                <div class="relative mt-2">
                    <div class="progress-bar bg-gray-300 h-2 rounded"></div>
                    <div class="progress-indicator bg-[#04060f] h-2 rounded absolute top-0 left-0" style="width: 70%;"></div>
                </div>
            </div>
        </div>

        <div class="skill-item flex flex-col items-center bg-white p-6 rounded-lg shadow-md transition-transform duration-300 transform hover:scale-105">
            <span class="text-6xl mr-4">🖍️</span>
            <div class="flex-1 text-center">
                <h3 class="text-lg font-semibold font-playfair">Illustrations</h3>
                <p class="text-sm text-gray-600">Proficient in creating vector and raster illustrations that communicate ideas effectively.</p>
                <div class="relative mt-2">
                    <div class="progress-bar bg-gray-300 h-2 rounded"></div>
                    <div class="progress-indicator bg-[#04060f] h-2 rounded absolute top-0 left-0" style="width: 80%;"></div>
                </div>
            </div>
        </div>

        <div class="skill-item flex flex-col items-center bg-white p-6 rounded-lg shadow-md transition-transform duration-300 transform hover:scale-105">
            <span class="text-6xl mr-4">🛠️</span>
            <div class="flex-1 text-center">
                <h3 class="text-lg font-semibold font-playfair">Audio Editing</h3>
                <p class="text-sm text-gray-600">Experience in sound design and audio editing, ensuring high-quality audio production.</p>
                <div class="relative mt-2">
                    <div class="progress-bar bg-gray-300 h-2 rounded"></div>
                    <div class="progress-indicator bg-[#04060f] h-2 rounded absolute top-0 left-0" style="width: 65%;"></div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Footer -->
<footer class="bg-[#04060f] text-white text-center p-4 mt-auto">
    <div class="container mx-auto">
        <p class="font-playfair">&copy; {year} My Portfolio. All rights reserved.</p>
    </div>
</footer>

<style>
    .progress-bar {
        width: 100%;
    }

    .progress-indicator {
        transition: width 0.5s ease;
    }
</style>
