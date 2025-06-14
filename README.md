# devorbit404.github.io
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Warshan | Front-End Developer</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #0d1117;
      --fg: #c9d1d9;
      --accent: #58a6ff;
      --light: #161b22;
      --transition: all 0.3s ease;
    }
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      background-color: var(--bg);
      color: var(--fg);
      font-family: 'Poppins', sans-serif;
      line-height: 1.6;
    }
    header {
      background-color: var(--light);
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 2px 5px #00000033;
    }
    .logo {
      font-size: 1.5rem;
      color: var(--accent);
      font-weight: bold;
    }
    nav a {
      color: var(--fg);
      text-decoration: none;
      margin-left: 1.5rem;
      transition: var(--transition);
    }
    nav a:hover {
      color: var(--accent);
    }
    .section {
      padding: 4rem 2rem;
      max-width: 1000px;
      margin: auto;
    }
    .section h2 {
      color: var(--accent);
      font-size: 2rem;
      margin-bottom: 1rem;
    }
    .about p, .languages ul, .projects .project, .contact p {
      margin-bottom: 1rem;
    }
    .languages ul {
      list-style: none;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
      gap: 1rem;
    }
    .languages li {
      background-color: var(--light);
      padding: 0.75rem 1rem;
      border-radius: 5px;
      text-align: center;
      transition: var(--transition);
    }
    .languages li:hover {
      background-color: var(--accent);
      color: #fff;
    }
    .projects .project {
      background-color: var(--light);
      padding: 1rem;
      border-radius: 5px;
      transition: var(--transition);
    }
    .projects .project:hover {
      background-color: var(--accent);
      color: #fff;
    }
    footer {
      text-align: center;
      padding: 2rem;
      background-color: #0b0f17;
      color: #666;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">Warshan</div>
    <nav>
      <a href="#about">About</a>
      <a href="#languages">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header> <section class="section about" id="about">
    <h2>About Me</h2>
    <p>Hi, I'm <strong>Warshan</strong>, a Front-End Developer with 3 years of hands-on experience building responsive and user-centric websites using HTML, CSS, JavaScript, and frameworks like React.</p>
    <p>No formal degree, just pure skills and projects that speak louder than paper.</p>
  </section> <section class="section languages" id="languages">
    <h2>Front-End Languages & Tools</h2>
    <ul>
      <li>HTML5</li>
      <li>CSS3</li>
      <li>JavaScript</li>
      <li>React</li>
      <li>Tailwind</li>
      <li>Bootstrap</li>
      <li>TypeScript</li>
      <li>Git</li>
      <li>GSAP</li>
      <li>Figma</li>
    </ul>
  </section> <section class="section projects" id="projects">
    <h2>Featured Projects</h2>
    <div class="project">
      <h3>Modern Portfolio Site</h3>
      <p>A responsive, animated portfolio website built with HTML, CSS, JS & GSAP.</p>
    </div>
    <div class="project">
      <h3>E-commerce UI</h3>
      <p>Built using React and TailwindCSS. Mobile-first and fully interactive.</p>
    </div>
  </section> <section class="section contact" id="contact">
    <h2>Contact</h2>
    <p>Email: <a href="mailto:warshankakar69@gmail.com">warshankakar69@gmail.com</a></p>
    <p>Let's build something amazing together!</p>
  </section> <footer>
    &copy; 2025 Warshan. Built with love &lt;/&gt;
  </footer> <script>
    // Simple fade animation
    const sections = document.querySelectorAll('.section');
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.style.opacity = 1;
          entry.target.style.transform = 'translateY(0)';
        }
      });
    }, { threshold: 0.1 });

    sections.forEach(section => {
      section.style.opacity = 0;
      section.style.transform = 'translateY(50px)';
      section.style.transition = 'all 0.8s ease-out';
      observer.observe(section);
    });
  </script></body>
</html>
