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
    <button type="button" class="text-2xl font-bold" on:click={scrollToTop}>ELPZ</button>
    <div class="text-2xl">About me</div>
</header>


<div class="container mt-16">
    <h1>About Me</h1>
    <p class="intro">
        Hello! I am <span class="highlight">ELPZ</span>, a passionate BSIT student at Gordon College, currently in my third year.
        I have a keen interest in technology and design, striving to develop innovative solutions to real-world problems.
    </p>

    <!-- Personal Background Section -->
    <div class="section">
        <h2>Personal Background</h2>
        <p>
            I was born and raised in Olongapo, and from a young age, I’ve always had a fascination with computers and how they work.
            Over the years, my curiosity led me to explore different aspects of technology, from programming to graphic design, which later shaped my decision to pursue a degree in Information Technology.
        </p>
        <p>
            As I continue my education at Gordon College, I’m always looking for new challenges and learning opportunities to sharpen my skills as a BSIT student.
        </p>
    </div>

    <!-- Hobbies & Interests Section -->
    <div class="section">
        <h2>Hobbies & Interests</h2>
        <ul class="hobbies-list">
            <li><strong>Programming:</strong> I enjoy coding and experimenting with new frameworks and languages.</li>
            <li><strong>Graphic Design:</strong> Creating digital art and website layouts is one of my favorite creative outlets.</li>
            <li><strong>Video Games:</strong> I’m a big fan of strategy and role-playing games, which often inspire my design ideas.</li>
            <li><strong>Traveling:</strong> Exploring new places and cultures broadens my perspective and inspires me creatively.</li>
        </ul>
    </div>

    <!-- Educational Attainment Section -->
    <div class="education">
        <h2>Educational Attainment</h2>
        <div class="timeline">
            <div class="institution">
                <span class="degree">Bachelor of Science in Information Technology</span>
                <div>Gordon College</div>
            </div>
            <div class="institution">
                <span class="degree">TVL ICT Strand</span>
                <div>Asian Institute of Computer Studies</div>
            </div>
            <div class="institution">
                <span class="degree">Senior High School</span>
                <div>Sta. Rita High School</div>
            </div>
            <div class="institution">
                <span class="degree">Elementary Education</span>
                <div>Tabacuhan Elementary School</div>
            </div>
        </div>
    </div>

    <!-- Career Aspirations Section -->
    <div class="section">
        <h2>Career Aspirations</h2>
        <p>
            My goal is to become a full-stack developer, working on both front-end and back-end development. I am excited about the endless possibilities technology offers and want to contribute to projects that make a meaningful impact in the world.
        </p>
        <p>
            Whether it's creating seamless user experiences or developing innovative backend solutions, I aim to be at the forefront of technology and continue learning throughout my career.
        </p>
    </div>
</div>

<footer class="bg-[#04060f] text-white text-center p-4 mt-auto">
    <div class="mx-auto">
        <p class="font-playfair">&copy; {year} My Portfolio. All rights reserved.</p>
    </div>
</footer>

<style>
    /* General container for page layout */
    .container {
        padding: 5rem 2rem;
        max-width: 900px;
        margin: auto;
        font-family: 'Raleway', sans-serif;
        color: #333;
        text-align: center;
    }

    h1 {
        font-size: 3rem;
        margin-bottom: 2rem;
        color: #04060f;
    }

    h2 {
        font-size: 2.5rem;
        margin: 2rem 0 1rem;
        color: #555;
        font-weight: normal; /* Reduced boldness */
    }

    p.intro {
        font-size: 1.2rem;
        line-height: 1.8;
        margin-bottom: 2rem;
        text-align: justify;
        max-width: 800px;
        margin-left: auto;
        margin-right: auto;
    }

    .highlight {
        color: #04060f;
        font-weight: bold;
    }

    /* Section styling for Personal Background, Hobbies, and Career Aspirations */
    .section {
        margin-top: 2rem;
        padding: 2rem;
        background-color: #f9f9f9;
        border-radius: 8px;
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    .section p {
        text-align: justify;
        line-height: 1.6;
        margin: 1rem 0;
    }

    /* Hobbies list styling */
    .hobbies-list {
        list-style: none;
        padding: 0;
    }

    .hobbies-list li {
        margin: 0.8rem 0;
        font-size: 1.1rem;
    }

    .education {
        margin-top: 2rem;
        border-top: 2px solid #04060f;
        padding-top: 1rem;
        width: 100%;
    }

    .timeline {
        display: flex;
        flex-direction: column;
        gap: 1.5rem;
    }

    .institution {
        background-color: #f5f5f5;
        padding: 1.5rem;
        border-radius: 8px;
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        text-align: left;
        max-width: 100%;
    }

    .institution div {
        margin-top: 0.5rem;
        font-size: 1rem;
        color: #333;
    }

    .degree {
        font-style: italic;
        font-weight: bold;
        color: #04060f;
        font-size: 1.2rem;
    }

</style>
