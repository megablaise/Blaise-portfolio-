<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mega Blaise | Web Developer</title>
  <style>
    /* ===== Basic Reset ===== */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, sans-serif; }
    body { line-height: 1.6; color: #333; }

    /* ===== Header & Navigation ===== */
    header {
      background-color: #1e3a8a;
      color: white;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 { font-size: 1.5rem; }
    nav ul { list-style: none; display: flex; gap: 1.5rem; }
    nav a { color: white; text-decoration: none; font-weight: bold; transition: color 0.2s; }
    nav a:hover { color: #facc15; }

    /* ===== Hero Section ===== */
    .hero {
      text-align: center;
      padding: 4rem 2rem;
      background-color: #f3f4f6;
    }
    .hero h2 { font-size: 2.5rem; margin-bottom: 1rem; }
    .hero p { font-size: 1.2rem; margin-bottom: 2rem; }
    .hero a {
      display: inline-block;
      padding: 0.75rem 1.5rem;
      background-color: #1e3a8a;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
      transition: background-color 0.2s;
    }
    .hero a:hover { background-color: #3746b2; }

    /* ===== Sections ===== */
    section { padding: 3rem 2rem; max-width: 1000px; margin: 0 auto; }
    section h2 { font-size: 2rem; margin-bottom: 1.5rem; color: #1e3a8a; text-align: center; }

    /* ===== About Section ===== */
    #about { background-color: #e0f2fe; }
    #about .content { display: flex; flex-wrap: wrap; gap: 2rem; align-items: center; justify-content: center; }
    #about img { max-width: 300px; border-radius: 10px; }
    #about .text { max-width: 600px; }

    /* ===== Portfolio Section ===== */
    #portfolio { background-color: #fef3c7; }
    #portfolio .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
    }
    #portfolio .project {
      background-color: white;
      padding: 1rem;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      transition: transform 0.2s;
    }
    #portfolio .project:hover { transform: translateY(-5px); }
    #portfolio img { width: 100%; border-radius: 5px; }

    /* ===== Contact Section ===== */
    #contact { background-color: #d1fae5; text-align: center; }
    #contact form {
      max-width: 500px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }
    #contact input, #contact textarea {
      padding: 0.75rem;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 1rem;
    }
    #contact button {
      padding: 0.75rem;
      background-color: #1e3a8a;
      color: white;
      font-weight: bold;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.2s;
    }
    #contact button:hover { background-color: #3746b2; }

    /* ===== Footer ===== */
    footer {
      background-color: #1e3a8a;
      color: white;
      text-align: center;
      padding: 1rem;
      margin-top: 2rem;
    }

    /* ===== Responsive ===== */
    @media (max-width: 768px) {
      #about .content { flex-direction: column; text-align: center; }
    }
  </style>
</head>
<body>

  <!-- Header & Navigation -->
  <header>
    <h1>Mega Blaise</h1>
    <nav>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#portfolio">Portfolio</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <h2>Hi, I’m Mega Blaise!</h2>
    <p>Web developer building modern, responsive websites and applications.</p>
    <a href="#portfolio">View My Work</a>
  </section>

  <!-- About Section -->
  <section id="about">
    <h2>About Me</h2>
    <div class="content">
      <img src="https://i.imgur.com/EDdYICQ.jpg" alt="Profile Photo">
      <div class="text">
        <p>I am a web developer passionate about creating responsive, modern websites. I specialize in HTML, CSS, and JavaScript, and I enjoy building projects that solve real-world problems.</p>
      </div>
    </div>
  </section>

  <!-- Portfolio Section -->
  <section id="portfolio">
    <h2>My Portfolio</h2>
    <div class="projects">
      <div class="project">
        <img src="https://via.placeholder.com/300x200" alt="Project Screenshot">
        <h3>Project One</h3>
        <p>A responsive business website I built with HTML, CSS, and JS.</p>
      </div>
      <div class="project">
        <img src="https://via.placeholder.com/300x200" alt="Project Screenshot">
        <h3>Project Two</h3>
        <p>A landing page designed for a marketing campaign.</p>
      </div>
      <div class="project">
        <img src="https://via.placeholder.com/300x200" alt="Project Screenshot">
        <h3>Project Three</h3>
        <p>A portfolio showcase site for a creative professional.</p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h2>Contact Me</h2>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" value="megablaise44@gmail.com" required>
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
      <p>Or reach me via: 
        <a href="https://www.linkedin.com/in/mega-blaise-b736773b7#overlay_profile-image-modal" target="_blank">LinkedIn</a> | 
        <a href="https://github.com/megablaise" target="_blank">GitHub</a>
      </p>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2026 Mega Blaise | Web Developer | 
    <a href="https://www.linkedin.com/in/mega-blaise-b736773b7#overlay_profile-image-modal" target="_blank" style="color:white; text-decoration:underline;">LinkedIn</a> | 
    <a href="https://github.com/megablaise" target="_blank" style="color:white; text-decoration:underline;">GitHub</a>
  </footer>

</body>
</html>
