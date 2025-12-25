# MyPortfolioWebsite
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Portfolio - [Your Name]</title>
    <!-- Load Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom scrollbar for aesthetics */
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }
        /* Style the scrollbar for webkit browsers */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        ::-webkit-scrollbar-thumb {
            background: #cbd5e1; /* slate-300 */
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #94a3b8; /* slate-400 */
        }
    </style>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        'primary-blue': '#0077b5', /* LinkedIn Blue */
                        'bg-light': '#f8fafc', /* slate-50 */
                        'text-dark': '#1e293b', /* slate-800 */
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-bg-light text-text-dark antialiased">

    <!-- Navigation (Sticky on scroll) -->
    <nav class="sticky top-0 z-50 bg-white shadow-lg">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <a href="#" class="text-2xl font-bold text-primary-blue hover:text-blue-700 transition duration-300">
                    DJ
                </a>
                <div class="flex space-x-4">
                    <a href="#projects" class="text-text-dark hover:text-primary-blue font-medium transition duration-300 p-2 rounded-lg">Projects</a>
                    <a href="#skills" class="text-text-dark hover:text-primary-blue font-medium transition duration-300 p-2 rounded-lg">Skills</a>
                    <a href="#contact" class="text-text-dark hover:text-primary-blue font-medium transition duration-300 p-2 rounded-lg">Contact</a>
                </div>
            </div>
        </div>
    </nav>

    <main class="max-w-4xl mx-auto px-4 py-8 sm:py-12 lg:py-16">

        <!-- 1. Hero Section (The first thing visitors see) -->
        <section class="text-center mb-16 p-6 sm:p-10 bg-white rounded-xl shadow-2xl">
            <img src="Dj casual pic.jpg" alt="Professional Headshot"
                 class="w-32 h-32 rounded-full mx-auto mb-6 object-cover border-4 border-primary-blue shadow-lg">
            
            <h1 class="text-4xl sm:text-5xl font-extrabold text-text-dark mb-2">
                Dheeraj Jangra
            </h1>
            <h2 class="text-xl sm:text-2xl font-semibold text-primary-blue mb-6">
                Senior Software Engineer | Data Visualization Specialist
            </h2>

            <p class="text-lg text-slate-600 max-w-2xl mx-auto mb-8">
                I transform complex data into actionable insights through robust, scalable, and user-friendly web applications. Focused on efficient development and clean architecture.
            </p>

            <div class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-4">
                <a href="#contact" class="inline-block px-8 py-3 bg-primary-blue text-white font-bold rounded-full shadow-lg hover:bg-blue-700 transition duration-300 transform hover:scale-105">
                    Get In Touch
                </a>
                <a href="Resume2.pdf" target="_blank" class="inline-block px-8 py-3 border-2 border-primary-blue text-primary-blue font-bold rounded-full shadow-lg hover:bg-blue-50 transition duration-300 transform hover:scale-105">
                    View Resume
                </a>
            </div>
        </section>

        <!-- 2. About Me/Summary -->
        <section id="about" class="mb-16 p-6 sm:p-8 bg-white rounded-xl shadow-lg">
            <h3 class="text-3xl font-bold text-text-dark border-b-4 border-primary-blue pb-2 mb-6">About Me</h3>
            <p class="text-slate-700 leading-relaxed">
                Motivated and detail-oriented Computer Science student seeking an internship opportunity 
to apply academic knowledge, gain practical experience, and contribute to real-world 
projects.
        </section>

        <!-- 3. Projects Showcase -->
        <section id="projects" class="mb-16">
            <h3 class="text-3xl font-bold text-text-dark border-b-4 border-primary-blue pb-2 mb-8 p-1">Key Projects</h3>
            
            <div class="space-y-8">
                <!-- Project Card 1 -->
                <div class="bg-white p-6 rounded-xl shadow-xl hover:shadow-2xl transition duration-300 transform hover:-translate-y-1">
                    <h4 class="text-2xl font-semibold text-primary-blue mb-2">Real-Time Traffic Management</h4>
                    <p class="text-sm font-medium text-slate-500 mb-4">Tech Stack: React, D3.js, Node.js, PostgreSQL</p>
                    <p class="text-slate-700 mb-4">
                        Developed a high-throughput real time traffic managing application. It uses YOLOv8 model in machine learning to detect number of vehicles in the lane and green signal timing is adjusted based on the rush. Resulted in a 40% reduction in rush.
                    </p>
                    <div class="flex space-x-4">
                        <a href="smarttrafficlight.py" target="_blank" class="text-text-dark hover:text-primary-blue font-medium underline">
                            Code &rarr;
                        </a>
                        <!-- <a href="[LINK_TO_PROJECT_GITHUB]" target="_blank" class="text-text-dark hover:text-primary-blue font-medium underline">
                            GitHub Code &rarr;
                        </a> -->
                    </div>
                </div>

                <!-- Project Card 2 -->
                <div class="bg-white p-6 rounded-xl shadow-xl hover:shadow-2xl transition duration-300 transform hover:-translate-y-1">
                    <h4 class="text-2xl font-semibold text-primary-blue mb-2">Real time captioning for deaf people</h4>
                    <p class="text-sm font-medium text-slate-500 mb-4">Tech Stack: Python (Django), AWS Lambda, DynamoDB</p>
                    <p class="text-slate-700 mb-4">
                        Designed to help deaf people to communicate by reading captions of the speaker in real time. Achieved 99.99% positive replies from deaf people.
                    </p>
                    <div class="flex space-x-4">
                        <a href="[LINK_TO_PROJECT_LIVE]" target="_blank" class="text-text-dark hover:text-primary-blue font-medium underline">
                            Live Demo &rarr;
                        </a>
                        <!-- <a href="[LINK_TO_PROJECT_GITHUB]" target="_blank" class="text-text-dark hover:text-primary-blue font-medium underline">
                            GitHub Code &rarr;
                        </a> -->
                    </div>
                </div>
            </div>
        </section>

        <!-- 4. Skills & Expertise -->
        <section id="skills" class="mb-16">
            <h3 class="text-3xl font-bold text-text-dark border-b-4 border-primary-blue pb-2 mb-8 p-1">Skills & Expertise</h3>
            <div class="bg-white p-6 rounded-xl shadow-lg">
                <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 gap-4">
                    <!-- Hard Skills -->
                    <span class="inline-block bg-primary-blue/10 text-primary-blue font-semibold px-4 py-2 rounded-full text-center transition duration-300 hover:bg-primary-blue/20">React.js</span>
                    <span class="inline-block bg-primary-blue/10 text-primary-blue font-semibold px-4 py-2 rounded-full text-center transition duration-300 hover:bg-primary-blue/20">Node.js / Express</span>
                    <span class="inline-block bg-primary-blue/10 text-primary-blue font-semibold px-4 py-2 rounded-full text-center transition duration-300 hover:bg-primary-blue/20">Python / Django</span>
                    <span class="inline-block bg-primary-blue/10 text-primary-blue font-semibold px-4 py-2 rounded-full text-center transition duration-300 hover:bg-primary-blue/20">AWS (S3, Lambda)</span>
                    <span class="inline-block bg-primary-blue/10 text-primary-blue font-semibold px-4 py-2 rounded-full text-center transition duration-300 hover:bg-primary-blue/20">SQL/NoSQL</span>
                    <span class="inline-block bg-primary-blue/10 text-primary-blue font-semibold px-4 py-2 rounded-full text-center transition duration-300 hover:bg-primary-blue/20">D3.js / Visualization</span>
                    <!-- Soft Skills -->
                    <span class="inline-block bg-slate-200 text-text-dark font-semibold px-4 py-2 rounded-full text-center transition duration-300 hover:bg-slate-300">Mentorship</span>
                    <span class="inline-block bg-slate-200 text-text-dark font-semibold px-4 py-2 rounded-full text-center transition duration-300 hover:bg-slate-300">Agile/Scrum</span>
                    <span class="inline-block bg-slate-200 text-text-dark font-semibold px-4 py-2 rounded-full text-center transition duration-300 hover:bg-slate-300">System Design</span>
                </div>
            </div>
        </section>

        <!-- 5. Contact Section -->
        <section id="contact" class="p-6 sm:p-8 bg-white rounded-xl shadow-lg text-center">
            <h3 class="text-3xl font-bold text-text-dark border-b-4 border-primary-blue pb-2 mb-6 inline-block">Connect With Me</h3>
            <p class="text-lg text-slate-700 mb-6">
                I'm currently open to new opportunities and collaborations. Feel free to reach out!
            </p>
            
            <div class="flex flex-col space-y-4 sm:space-y-0 sm:flex-row sm:justify-center sm:space-x-6">
                <!-- Email Button -->
                <a href="mailto:dheerajjangra3424@gmail.com" class="p-3 bg-red-600 text-white rounded-lg font-medium shadow-md hover:bg-red-700 transition duration-300 transform hover:scale-105 flex items-center justify-center">
                    <svg class="w-5 h-5 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8m-2 4v4a2 2 0 01-2 2H5a2 2 0 01-2-2v-4"></path></svg>
                    Email Me
                </a>
                
                <!-- LinkedIn Button -->
                <a href="https://www.linkedin.com/in/dheeraj-jangra-537a4b2b1" target="_blank" class="p-3 bg-primary-blue text-white rounded-lg font-medium shadow-md hover:bg-blue-700 transition duration-300 transform hover:scale-105 flex items-center justify-center">
                    <svg class="w-5 h-5 mr-2" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M20.447 20.452h-3.535v-5.603c0-1.339-.023-3.064-1.867-3.064-1.866 0-2.152 1.458-2.152 2.978v5.69h-3.536V9.248h3.398v1.56a3.78 3.78 0 013.398-1.868c3.626 0 4.296 2.373 4.296 5.467v6.075zM7.106 7.42c-1.164 0-2.096-.932-2.096-2.097 0-1.164.932-2.096 2.096-2.096 1.165 0 2.097.932 2.097 2.096 0 1.165-.932 2.097-2.097 2.097zM8.883 9.248H5.347v11.204h3.536V9.248z"/></svg>
                    LinkedIn
                </a>

                <!-- GitHub Button -->
                <a href="https://github.com/Dheeraj-Jangra" target="_blank" class="p-3 bg-gray-800 text-white rounded-lg font-medium shadow-md hover:bg-gray-900 transition duration-300 transform hover:scale-105 flex items-center justify-center">
                    <svg class="w-5 h-5 mr-2" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.163 6.83 9.48.5.087.683-.217.683-.487 0-.24-.008-1.018-.014-1.993-2.782.607-3.37-1.34-3.37-1.34-.455-1.15-.992-1.453-.992-1.453-.814-.555.06-.543.06-.543.797.056 1.216.822 1.216.822.708 1.216 1.85.864 2.305.66.072-.515.277-.864.504-1.062-1.769-.201-3.635-.884-3.635-3.95 0-.872.31-1.585.823-2.146-.083-.202-.358-1.012.078-2.112 0 0 .672-.215 2.204.82A7.838 7.838 0 0112 7.64c.548 0 1.096.074 1.624.218 1.532-1.035 2.204-.82 2.204-.82.436 1.1.162 1.91.08 2.112.513.56.823 1.274.823 2.146 0 3.074-1.868 3.748-3.645 3.945.285.247.54.735.54 1.48V21.5c0 .27.183.58.688.484C20.146 20.18 24 16.035 24 12.017 24 6.484 19.523 2 14 2z" clip-rule="evenodd"/></svg>
                    GitHub
                </a>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white mt-12 py-8">
        <div class="max-w-4xl mx-auto px-4 text-center">
            <p class="text-sm">
                &copy; <span id="currentYear"></span> Dheeraj Jangra. Built with a focus on professional presentation for LinkedIn visibility.
            </p>
            <p class="text-xs mt-2 text-gray-400">
                Designed to be fully responsive and load quickly.
            </p>
        </div>
    </footer>

    <script>
        // Set the current year in the footer
        document.getElementById('currentYear').textContent = new Date().getFullYear();

        // Optional: Simple JS for scrolling to sections
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
