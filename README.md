# My-Website
This is My Website.

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>sharea sobuj | Portfolio</title>
  <link rel="stylesheet" href="style.css" />
  <style>
    * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', sans-serif;
  line-height: 1.6;
  color: #333;
  background: #f4f4f4;
}

header {
  background: #222;
  color: #fff;
  padding: 1rem 2rem;
  position: sticky;
  top: 0;
  z-index: 1000;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
}

.nav-links a {
  color: #fff;
  text-decoration: none;
  transition: color 0.3s ease;
}

.nav-links a:hover {
  color: #00bcd4;
}

.hero {
  padding: 4rem 2rem;
  background: #00bcd4;
  color: white;
  text-align: center;
}

.hero h1 span {
  color: #fff700;
}

section {
  padding: 4rem 2rem;
}

.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.project {
  background: white;
  padding: 1.5rem;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  max-width: 500px;
  margin: auto;
}

form input,
form textarea {
  padding: 0.75rem;
  border: 1px solid #ccc;
  border-radius: 6px;
}

form button {
  background: #00bcd4;
  color: white;
  padding: 0.75rem;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

form button:hover {
  background: #0097a7;
}

footer {
  text-align: center;
  padding: 2rem;
  background: #222;
  color: #fff;
}

  </style>
</head>
<body>
  <header>
    <nav>
      <div class="logo">SHAREA SOBUJ</div>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="hero">
    <h1>Hello, I'm <span>SHAREA SOBUJ</span></h1>
    <p>Web Developer | Designer | Freelancer</p>
  </section>

  <section id="about">
    <h2>About Me</h2>
    <p>I'm a front-end web developer with a passion for crafting clean, responsive, and user-friendly websites. I specialize in turning designs into functional, high-performance code using HTML, CSS, JavaScript, and modern libraries like React. I focus on creating seamless user experiences and writing clean, maintainable code. Whether it's building from scratch or improving existing interfaces, I enjoy solving problems and bringing ideas to life in the browser. I'm always eager to learn new tools and technologies to stay ahead in the fast-evolving world of web development.

    </p>
    <section id="projects">
      <h2>Projects</h2>
      <div class="project-grid">
        
        <div class="project">
          <h3>Calculator</h3>
          <p>A responsive, JavaScript-powered calculator that supports basic arithmetic operations. Clean UI and keyboard support included.</p>
        </div>
        
        <div class="project">
          <h3>MindBridge</h3>
          <p>An interactive mental health and journaling web app designed to help users track emotions and build mindfulness habits.</p>
        </div>
        
        <div class="project">
          <h3>YouTube Music Player</h3>
          <p>A custom front-end for playing and managing YouTube music playlists. Built with the YouTube API and a dynamic, mobile-friendly interface.</p>
        </div>
        
        <div class="project">
          <h3>Portfolio Website</h3>
          <p>This website! Built to showcase my work, skills, and contact information. Fully responsive and optimized for performance and SEO.</p>
        </div>
        
      </div>
    </section>
    

  <section id="contact">
    <h2>Contact</h2>
    <form id="contact-form">
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <footer>
    <p>© 2025 SHAREA SOBUJ. All rights reserved.</p>
  </footer>

  <script src="script.js">
    document.getElementById('contact-form').addEventListener('submit', function (e) {
  e.preventDefault();
  alert('Thanks for reaching out! I will get back to you soon.');
  this.reset();
});

  </script>
</body>
</html>

