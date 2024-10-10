<script>



    const projects = [
        {
            title: "Unfold",
            description: "A Portfolio template for students.",
            link: "https://example.com/project-one",
            image: "unfoldap.png" // Add the image property
        },
        {
            title: "Blog",
            description: "A blog website for everyone.",
            link: "https://example.com/project-one",
            image: "blog.png" // Add the image property
        },
    ];
</script>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />


<section class="bg-[#f5f5f5] py-0" id="cover">
    <div class="mx-0">
        <!-- Cover Photo Section -->
        <div class="relative mb-0 w-full h-[90vh]">
            <img src="/portfolioCover.jpg" alt="" class="absolute inset-0 w-full h-full object-cover" />
            <div class="absolute inset-0 flex flex-col justify-center items-start pl-8 sm:pl-16 md:pl-32 lg:pl-64 text-white">
                <h1 class="text-4xl sm:text-5xl md:text-6xl font-bold font-raleway text-[#04060f]">NIS CORPUZ</h1>
                <p class="mt-1 text-base sm:text-lg md:text-xl font-sans">I am a <span class="text-[#04060f]">BSIT</span> student, passionate about developing</p>
                <p class="text-base sm:text-lg md:text-xl font-sans">innovative solutions. Welcome to my <span class="text-[#04060f]">portfolio</span>!</p>
            </div>
        </div>

       <!-- About Section -->
<section id="about" class="bg-gradient-to-r  py-10">
    <div class="mx-auto px-4">
        <h2 class="text-3xl font-bold text-[#04060f] mb-4 text-center font-playfair">About Me</h2>
        <div class="flex flex-col sm:flex-row items-center justify-center">
            <img src="/cat.jpeg" alt="My Cat" class="w-32 h-32 rounded-full border-4 border-[#04060f] shadow-lg mr-4" />
            <div class="max-w-2xl p-4">
                <p class="text-lg font-sans mb-4 text-gray-800">
                    I am a dedicated BSIT student with a passion for technology and innovation. My journey has led me to explore various aspects of software development, including web and mobile applications. I thrive on challenges and enjoy creating solutions that enhance user experiences.
                </p>
                <p class="text-lg font-sans text-gray-800">
                    When I'm not coding, I love sketching and spending time with my cat Orin, who inspires my creativity and motivates me.
                </p>
            </div>
        </div>
    </div>
</section>

<section id="education" class="py-12 bg-gradient-to-r from-[#f5f5f5] to-[#ebebeb]">
    <h2 class="text-3xl font-bold text-[#04060f] mb-8 text-center font-playfair">Educational Background</h2>

    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6 px-6">
        <div class="bg-white shadow-sm rounded-lg p-4 flex flex-col items-center transition-transform transform hover:scale-105">
            <span class="text-3xl text-[#04060f]">🎓</span> <!-- Primary education icon -->
            <h3 class="text-xl font-semibold text-[#04060f] mt-2 font-playfair">Primary Education</h3>
            <p class="text-sm text-gray-700 text-center">Tabacuhan Elementary School</p>
            <p class="text-xs italic text-gray-500 text-center">Completed with honor and passion.</p>
        </div>

        <div class="bg-white shadow-sm rounded-lg p-4 flex flex-col items-center transition-transform transform hover:scale-105">
            <span class="text-3xl text-[#04060f]">🏫</span> <!-- Secondary education icon -->
            <h3 class="text-xl font-semibold text-[#04060f] mt-2 font-playfair">Secondary Education</h3>
            <p class="text-sm text-gray-700 text-center">Sta. Rita High School</p>
            <p class="text-xs italic text-gray-500 text-center">Explored various disciplines.</p>
        </div>

        <div class="bg-white shadow-sm rounded-lg p-4 flex flex-col items-center transition-transform transform hover:scale-105">
            <span class="text-3xl text-[#04060f]">💻</span> <!-- Senior High School icon -->
            <h3 class="text-xl font-semibold text-[#04060f] mt-2 font-playfair">Senior High School</h3>
            <p class="text-sm text-gray-700 text-center">Asian Institute of Computer Studies</p>
            <p class="text-xs italic text-gray-500 text-center">(TVL ICT STRAND)</p>
        </div>

        <div class="bg-white shadow-sm rounded-lg p-4 flex flex-col items-center transition-transform transform hover:scale-105">
            <span class="text-3xl text-[#04060f]">🎓</span> <!-- Tertiary education icon -->
            <h3 class="text-xl font-semibold text-[#04060f] mt-2 font-playfair">Tertiary Education</h3>
            <p class="text-sm text-gray-700 text-center">Gordon College</p>
            <p class="text-xs italic text-gray-500 text-center">3rd-year BSIT student.</p>
        </div>
        <!-- The updated "See More" button -->
        
    </div>
    <div class="flex justify-center mt-8">
        <a href="/about" class="text-white bg-[#04060f] hover:bg-blue-600 font-bold py-2 px-6 rounded transition-all duration-300">See More</a>
    </div>
</section>


        <!-- Skills Section -->
        <section id="skills" class="py-12 bg-[#f5f5f5]">
            <h2 class="text-3xl font-bold text-[#04060f] mb-10 text-center font-playfair">My Skills</h2>
        
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8 px-4">
                <!-- Skill Item -->
                <div class="flex items-center">
                    <span class="text-4xl mr-4">💻</span>
                    <div class="flex-1">
                        <h3 class="text-lg font-semibold font-playfair">Coding</h3>
                        <div class="relative mt-1">
                            <div class="bg-[#04060f] h-1 w-full rounded"></div>
                            <div class="bg-blue-500 h-1 w-[40%] absolute top-0 left-0 rounded"></div> <!-- Indicator for proficiency -->
                        </div>
                    </div>
                </div>
        
                <div class="flex items-center">
                    <span class="text-4xl mr-4">🖼️</span>
                    <div class="flex-1">
                        <h3 class="text-lg font-semibold font-playfair">Picture Editing</h3>
                        <div class="relative mt-1">
                            <div class="bg-[#04060f] h-1 w-full rounded"></div>
                            <div class="bg-blue-500 h-1 w-[70%] absolute top-0 left-0 rounded"></div> <!-- Indicator for proficiency -->
                        </div>
                    </div>
                </div>
        
                <div class="flex items-center">
                    <span class="text-4xl mr-4">🎥</span>
                    <div class="flex-1">
                        <h3 class="text-lg font-semibold font-playfair">Video Editing</h3>
                        <div class="relative mt-1">
                            <div class="bg-[#04060f] h-1 w-full rounded"></div>
                            <div class="bg-blue-500 h-1 w-[75%] absolute top-0 left-0 rounded"></div> <!-- Indicator for proficiency -->
                        </div>
                    </div>
                </div>
        
                <div class="flex items-center">
                    <span class="text-4xl mr-4">🎨</span>
                    <div class="flex-1">
                        <h3 class="text-lg font-semibold font-playfair">Sketching</h3>
                        <div class="relative mt-1">
                            <div class="bg-[#04060f] h-1 w-full rounded"></div>
                            <div class="bg-blue-500 h-1 w-[85%] absolute top-0 left-0 rounded"></div> <!-- Indicator for proficiency -->
                        </div>
                    </div>
                </div>
        
                <div class="flex items-center">
                    <span class="text-4xl mr-4">🔐</span>
                    <div class="flex-1">
                        <h3 class="text-lg font-semibold font-playfair">Cyber Security</h3>
                        <div class="relative mt-1">
                            <div class="bg-[#04060f] h-1 w-full rounded"></div>
                            <div class="bg-blue-500 h-1 w-[40%] absolute top-0 left-0 rounded"></div> <!-- Indicator for proficiency -->
                        </div>
                    </div>
                </div>
        
                <div class="flex items-center">
                    <span class="text-4xl mr-4">✒️</span>
                    <div class="flex-1">
                        <h3 class="text-lg font-semibold font-playfair">Lettering</h3>
                        <div class="relative mt-1">
                            <div class="bg-[#04060f] h-1 w-full rounded"></div>
                            <div class="bg-blue-500 h-1 w-[70%] absolute top-0 left-0 rounded"></div> <!-- Indicator for proficiency -->
                        </div>
                    </div>
                </div>
        
                <div class="flex items-center">
                    <span class="text-4xl mr-4">🖍️</span>
                    <div class="flex-1">
                        <h3 class="text-lg font-semibold font-playfair">Illustrations</h3>
                        <div class="relative mt-1">
                            <div class="bg-[#04060f] h-1 w-full rounded"></div>
                            <div class="bg-blue-500 h-1 w-[75%] absolute top-0 left-0 rounded"></div> <!-- Indicator for proficiency -->
                        </div>
                    </div>
                </div>
        
                <div class="flex items-center">
                    <span class="text-4xl mr-4">🗂️</span>
                    <div class="flex-1">
                        <h3 class="text-lg font-semibold font-playfair">Microsoft</h3>
                        <div class="relative mt-1">
                            <div class="bg-[#04060f] h-1 w-full rounded"></div>
                            <div class="bg-blue-500 h-1 w-[80%] absolute top-0 left-0 rounded"></div> <!-- Indicator for proficiency -->
                        </div>
                    </div>
                </div>
            </div>
            <!-- See More Button -->
    <div class="flex justify-center mt-8">
        <a href="/skills" class="text-white bg-[#04060f] hover:bg-blue-600 font-bold py-2 px-6 rounded transition-all duration-300">See More</a>
    </div>
        </section>
        
        <!-- Projects Section -->
<section id="projects" class="bg-[#f5f5f5] py-10">
    <div class="container mx-auto px-4">
        <h2 class="text-3xl text-center font-bold text-[#04060f] mb-10 font-playfair">My Projects</h2>
        <div class="flex justify-center gap-8 flex-wrap">
            {#each projects as project}
                <div class="bg-white rounded-lg shadow-lg p-6 transition-transform transform hover:scale-105 font-sans w-full max-w-xs flex flex-col">
                    <h3 class="text-xl font-semibold text-[#04060f] font-playfair mb-2">{project.title}</h3>
                    {#if project.image} <!-- Check if the project has an image -->
                        <img src={project.image} alt={project.title} class="w-full h-40 object-cover mb-4 rounded" />
                    {/if}
                    <p class="text-gray-600 my-2 flex-grow">{project.description}</p>
                    <a href={project.link} target="_blank" class="text-blue-600 hover:underline">View Project</a>
                </div>
            {/each}
        </div>
    </div>
    <!-- See More Button -->
    <div class="flex justify-center mt-8">
        <a href="/projects" class="text-white bg-[#04060f] hover:bg-blue-600 font-bold py-2 px-6 rounded transition-all duration-300">See More</a>
    </div>
</section>


        <section id="contact" class="bg-[#f5f5f5] py-10 text-center scroll-section">
            <div class="container mx-auto px-4">
                <h2 class="text-3xl font-bold text-[#04060f] mb-4 font-playfair">Contact Me</h2>
                <p class="text-lg font-sans mb-6">Feel free to reach out for collaboration or inquiries!</p>
                
                <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-6">
                    <div class="flex flex-col items-center">
                        <a href="mailto:202210168@gordoncollege.edu.ph" class="text-blue-600 hover:text-blue-800 flex flex-col items-center">
                            <i class="fas fa-envelope text-4xl"></i> <!-- Email icon -->
                            <p class="text-lg font-sans">Email</p>
                        </a>
                    </div>
                    <div class="flex flex-col items-center">
                        <a href="https://www.facebook.com/nis.corpuz" class="text-blue-600 hover:text-blue-800 flex flex-col items-center">
                            <i class="fab fa-facebook-f text-4xl"></i> <!-- Facebook icon -->
                            <p class="text-lg font-sans">Facebook</p>
                        </a>
                    </div>
                    <div class="flex flex-col items-center">
                        <a href="https://www.instagram.com/its.nisdre" class="text-blue-600 hover:text-blue-800 flex flex-col items-center">
                            <i class="fab fa-instagram text-4xl"></i> <!-- Instagram icon -->
                            <p class="text-lg font-sans">Instagram</p>
                        </a>
                    </div>
                    <div class="flex flex-col items-center">
                        <a href="https://github.com/underayko" class="text-blue-600 hover:text-blue-800 flex flex-col items-center">
                            <i class="fab fa-github text-4xl"></i> <!-- GitHub icon -->
                            <p class="text-lg font-sans">GitHub</p>
                        </a>
                    </div>
                </div>
            </div>
        </section>
        
    </div>
</section>