# portfolio
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content="Portfolio of Sanjana Reddy V - Full Stack Developer specializing in Java, Python Flask, and modern web technologies." />
  <title>Sanjana Reddy V | Full Stack Developer</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
  <link rel="icon" href="photo2.jpeg" type="image/jpeg">
  <script>
  document.addEventListener('DOMContentLoaded', () => {
    const menuBtn = document.querySelector('.md\\:hidden');
    const nav = document.querySelector('nav');

    menuBtn.addEventListener('click', () => {
      nav.classList.toggle('hidden');
    });

    document.querySelectorAll('nav a').forEach(link =>
      link.addEventListener('click', () => {
        if (!nav.classList.contains('md:flex')) {
          nav.classList.add('hidden');
        }
      })
    );
  });
</script>


  <script>
 

    tailwind.config = {
      theme: {
        extend: {
          colors: {
            primary: '#4F46E5',  // More vibrant indigo
            secondary: '#10B981', // Emerald green
            darkBg: '#1E293B',    // Dark blue-gray
            lightBg: '#F8FAFC',   // Very light gray
            textDark: '#1E293B',  // Dark blue-gray for text
            textLight: '#64748B'  // Gray for secondary text
          },
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
          },
        }
      }
    };
   

 
  </script>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
    
    html {
      scroll-behavior: smooth;
      font-family: 'Inter', sans-serif;
    }
    .typing::after {
      content: '|';
      animation: blink 0.7s infinite;
      animation-delay: 1s;
    }
    @keyframes blink {
      0%, 100% { opacity: 0 }
      50% { opacity: 1 }
    }
    .skill-card {
      transition: all 0.3s ease;
    }
    .skill-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
    }
    .project-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
      
    }
    footer a i {
  transition: transform 0.3s ease;
}
footer a:hover i {
  transform: scale(1.2);
  color: #10B981;
}
 </style>
</head>
<body class="bg-lightBg text-textDark">

  <!-- Navbar -->
  <header class="fixed top-0 w-full bg-white shadow-md z-50">
    <div class="max-w-7xl mx-auto px-4 py-4 flex justify-between items-center">
      <h1 class="text-2xl font-bold text-primary">Sanjana Reddy V</h1>
      <nav aria-label="Primary navigation" class="hidden md:flex space-x-8">
        <a href="#about" class="font-medium hover:text-primary transition">About</a>
        <a href="#projects" class="font-medium hover:text-primary transition">Projects</a>
        <a href="#skills" class="font-medium hover:text-primary transition">Skills</a>
        <a href="#contact" class="font-medium hover:text-primary transition">Contact</a>
      </nav>
      <button class="md:hidden text-primary focus:outline-none">
        <i class="fas fa-bars text-2xl"></i>
      </button>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="min-h-screen flex flex-col items-center justify-center bg-gradient-to-br from-darkBg to-gray-800 text-white pt-20 pb-20 px-4">
    <div class="mb-8">
      <img src="photo2.jpeg" alt="Sanjana Reddy V professional profile photo" 
           class="w-48 h-48 rounded-full object-cover border-4 border-primary shadow-xl" />
    </div>
    <div class="text-center max-w-2xl">
      <h2 class="text-4xl md:text-5xl font-bold mb-4">Hi, I'm Sanjana Reddy V</h2>
      <p class="text-xl md:text-2xl mb-8 typing">Full Stack Developer | Engineer</p>
      <div class="flex flex-col sm:flex-row justify-center gap-4">
        <a href="#" class="text-gray-400 hover:text-secondary transition">
  <i class="fab fa-twitter text-2xl"></i>
</a>
        <a href="#projects" class="bg-primary hover:bg-indigo-700 px-6 py-3 rounded-full text-white font-semibold transition shadow-md hover:shadow-lg">
          View My Work
        </a>
        <a href="#contact" class="bg-white text-primary hover:bg-gray-100 px-6 py-3 rounded-full font-semibold transition shadow-md hover:shadow-lg">
          Contact Me
        </a>
      </div>
    </div>
  </section>
  
  <!-- About -->
  <section id="about" class="py-20 px-4 max-w-4xl mx-auto">
    <h2 class="text-3xl font-bold mb-6 text-primary text-center">About Me</h2>
    <div class="bg-white p-8 rounded-xl shadow-md">
      <p class="text-lg leading-relaxed mb-6 text-textDark">
  I'm a 3rd-year Computer Science and Engineering (IoT) student passionate about full stack development and modern coding practices. I'm currently exploring technologies like JavaScript, Python Flask, and Java to build responsive and scalable web applications.
</p>
<p class="text-lg leading-relaxed text-textDark">
  I love solving real-world problems through code and enjoy working on both frontend and backend development. I'm looking for internship opportunities in web development or software engineering to grow my skills and contribute to meaningful projects.
</p>
    </div>
  </section>

  <!-- Projects -->
  <section id="projects" class="py-20 px-4 bg-white">
    <div class="max-w-6xl mx-auto">
      <h2 class="text-3xl font-bold text-center mb-12 text-primary">Featured Projects</h2>
      <div class="grid md:grid-cols-2 gap-8">
        <!-- Project 1 -->
        <div class="project-card bg-lightBg p-6 rounded-xl shadow-md transition duration-300">
          <div class="mb-4 h-48 bg-gradient-to-r from-primary to-secondary rounded-lg flex items-center justify-center text-white">
            <i class="fas fa-graduation-cap text-6xl opacity-90"></i>
          </div>
          <h3 class="text-xl font-semibold mb-2 text-primary">College Connect</h3>
          <p class="mb-4 text-textLight">A comprehensive communication platform for educational institutions featuring real-time chat, announcements, and resource sharing.</p>
          <div class="flex flex-wrap gap-2 mb-4">
            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm text-textDark">Python Flask</span>
            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm text-textDark">WebSockets</span>
            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm text-textDark">SQLite</span>
            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm text-textDark">JavaScript</span>
          </div>
         <a href="https://github.com/sanjanareddy2706/college-connect" target="_blank" rel="noopener noreferrer">
  View Project <i class="fas fa-arrow-right ml-2"></i>
</a>
        </div>
        
        <!-- Project 2 -->
        <div class="project-card bg-lightBg p-6 rounded-xl shadow-md transition duration-300">
          <div class="mb-4 h-48 bg-gradient-to-r from-secondary to-primary rounded-lg flex items-center justify-center text-white">
            <i class="fas fa-utensils text-6xl opacity-90"></i>
          </div>
          <h3 class="text-xl font-semibold mb-2 text-primary">Food Market Web App</h3>
          <p class="mb-4 text-textLight">Modern food ordering platform with intuitive browsing, cart management, and seamless checkout experience.</p>
          <div class="flex flex-wrap gap-2 mb-4">
            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm text-textDark">HTML/CSS</span>
            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm text-textDark">JavaScript</span>
            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm text-textDark">Responsive Design</span>
            <span class="bg-gray-100 px-3 py-1 rounded-full text-sm text-textDark">Tailwind CSS</span>
          </div>
          <a href="#" class="text-primary hover:text-indigo-700 font-medium inline-flex items-center">
            View Project <i class="fas fa-arrow-right ml-2"></i>
          </a>
        </div>
      </div>
    </div>
  </section>

  <!-- Skills -->
  <section id="skills" class="py-20 px-4 max-w-5xl mx-auto bg-lightBg">
    <h2 class="text-3xl font-bold mb-12 text-primary text-center">Technical Skills</h2>
    <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 gap-6">
      <div class="skill-card bg-white p-6 rounded-xl shadow text-center flex flex-col items-center">
        <i class="fab fa-html5 text-4xl text-primary mb-3"></i>
        <div class="font-medium">HTML/CSS</div>
        <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
          <div class="bg-primary h-2 rounded-full" style="width: 90%"></div>
        </div>
      </div>
      <div class="skill-card bg-white p-6 rounded-xl shadow text-center flex flex-col items-center">
        <i class="fab fa-js-square text-4xl text-primary mb-3"></i>
        <div class="font-medium">JavaScript</div>
        <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
          <div class="bg-primary h-2 rounded-full" style="width: 85%"></div>
        </div>
      </div>
      <div class="skill-card bg-white p-6 rounded-xl shadow text-center flex flex-col items-center">
        <i class="fab fa-python text-4xl text-primary mb-3"></i>
        <div class="font-medium">Python </div>
        <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
          <div class="bg-primary h-2 rounded-full" style="width: 80%"></div>
        </div>
      </div>
      <div class="skill-card bg-white p-6 rounded-xl shadow text-center flex flex-col items-center">
        <i class="fab fa-java text-4xl text-primary mb-3"></i>
        <div class="font-medium">Java</div>
        <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
          <div class="bg-primary h-2 rounded-full" style="width: 75%"></div>
        </div>
      </div>
     
    
      <div class="skill-card bg-white p-6 rounded-xl shadow text-center flex flex-col items-center">
        <i class="fab fa-git-alt text-4xl text-primary mb-3"></i>
        <div class="font-medium">Git & GitHub</div>
        <div class="w-full bg-gray-200 rounded-full h-2 mt-3">
          <div class="bg-primary h-2 rounded-full" style="width: 90%"></div>
        </div>
      </div>
     
    </div>
  </section>

  <!-- Contact -->
  <section id="contact" class="py-20 px-4 max-w-3xl mx-auto bg-white">
    <div class="bg-gradient-to-br from-primary to-secondary p-8 rounded-xl shadow-lg text-white">
      <h2 class="text-3xl font-bold mb-8 text-center">Let's Work Together</h2>
      <p class="text-lg mb-8 text-center opacity-90">
        I'm currently looking for new opportunities. Whether you have a project to discuss or just want to connect, I'd love to hear from you!
      </p>
      
      <div class="flex flex-col md:flex-row justify-center gap-6 mb-8">
        <a href="mailto:sanjanareddy2706@gmail.com" class="flex items-center justify-center space-x-2 hover:opacity-80 transition">
          <i class="fas fa-envelope text-xl"></i>
          <span class="font-medium">sanjanareddy2706@gmail.com</span>
        </a>
        <a href="tel:+918985941988" class="flex items-center justify-center space-x-2 hover:opacity-80 transition">
          <i class="fas fa-phone text-xl"></i>
          <span class="font-medium">+91 8985941988</span>
        </a>
      </div>
      
      <div class="flex justify-center space-x-6">
        <a href="https://linkedin.com/in/sanjana-reddy-vasipalli-789668343" class="text-2xl hover:opacity-80 transition" target="_blank" rel="noopener noreferrer">
          <i class="fab fa-linkedin-in"></i>
        </a>
        <a href="https://github.com/sanjanareddy2706" class="text-2xl hover:opacity-80 transition" target="_blank" rel="noopener noreferrer">
          <i class="fab fa-github"></i>
        </a>
        <a href="#" class="text-2xl hover:opacity-80 transition" target="_blank" rel="noopener noreferrer">
          <i class="fab fa-twitter"></i>
        </a>
        <a href="#" class="text-2xl hover:opacity-80 transition" target="_blank" rel="noopener noreferrer">
          <i class="fab fa-instagram"></i>
        </a>
      </div>
    </div>
  </section>

 <footer class="bg-darkBg text-white py-8">
  <div class="max-w-7xl mx-auto px-4 text-center">
    <p>&copy; 2025 Sanjana Reddy V. All rights reserved.</p>
    <p class="mt-2 text-gray-400">Built with passion using modern web technologies</p>
    
 <div class="mt-4 flex justify-center space-x-6">
  <a href="https://linkedin.com/in/..." target="_blank" rel="noopener noreferrer">
    <i class="fab fa-linkedin-in text-2xl"></i>
  </a>
  <a href="https://github.com/..." target="_blank" rel="noopener noreferrer">
    <i class="fab fa-github text-2xl"></i>
  </a>
  <a href="#" target="_blank" rel="noopener noreferrer">
    <i class="fab fa-twitter text-2xl"></i>
  </a>
  <a href="#" target="_blank" rel="noopener noreferrer">
    <i class="fab fa-instagram text-2xl"></i>
  </a>
</div>

  </div>
</footer>


  <!-- Mobile Menu Script -->
  <script>
    document.querySelector('.md\\:hidden').addEventListener('click', function() {
      const nav = document.querySelector('nav');
      nav.classList.toggle('hidden');
      nav.classList.toggle('flex');
      nav.classList.toggle('flex-col');
      nav.classList.toggle('absolute');
      nav.classList.toggle('top-16');
      nav.classList.toggle('right-4');
      nav.classList.toggle('bg-white');
      nav.classList.toggle('p-4');
      nav.classList.toggle('rounded-lg');
      nav.classList.toggle('shadow-lg');
    });

    // Smooth scrolling for all browsers
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
