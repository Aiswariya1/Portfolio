# Portfolio
This is a portfolio website.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Portfolio</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      background-color: #f4f4f4;
      color: #333;
    }

    header {
      background: #333;
      color: #fff;
      padding: 20px 0;
      text-align: center;
    }

    header h1 {
      margin-bottom: 10px;
    }

    nav a {
      color: #fff;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }

    section {
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
    }

    #about, #projects, #contact {
      background: #fff;
      margin-top: 20px;
      border-radius: 8px;
      padding: 30px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    h2 {
      margin-bottom: 20px;
      color: #007bff;
    }

    .project {
      margin-bottom: 15px;
      padding: 10px;
      border: 1px solid #ddd;
      border-radius: 5px;
    }

    form input, form textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border-radius: 5px;
      border: 1px solid #ccc;
    }

    form button {
      padding: 10px 20px;
      border: none;
      background-color: #007bff;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }

    footer {
      background: #333;
      color: #fff;
      text-align: center;
      padding: 15px 0;
      margin-top: 40px;
    }
  </style>
</head>
<body>

  <header>
    <h1>John Doe</h1>
    <p>Web Developer | Designer | Coder</p>
    <nav>
      <a href="#about">About</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="about">
    <h2>About Me</h2>
    <p>Hello! I'm John, a passionate web developer with experience in creating dynamic and responsive websites using HTML, CSS, and JavaScript. I love solving problems and building clean user interfaces.</p>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="project">
      <h3>Portfolio Website</h3>
      <p>A personal website to showcase my projects, built with HTML, CSS, and JavaScript.</p>
    </div>
    <div class="project">
      <h3>To-Do List App</h3>
      <p>A simple to-do list app with add/remove functionality using vanilla JavaScript.</p>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <form id="contactForm">
      <input type="text" id="name" placeholder="Your Name" required />
      <input type="email" id="email" placeholder="Your Email" required />
      <textarea id="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
    <p id="formStatus" style="color: green; margin-top: 10px;"></p>
  </section>

  <footer>
    <p>&copy; 2025 John Doe. All Rights Reserved.</p>
  </footer>

  <script>
    const form = document.getElementById('contactForm');
    const status = document.getElementById('formStatus');

    form.addEventListener('submit', function(e) {
      e.preventDefault();
      status.textContent = "Thanks, your message has been sent!";
      form.reset();
    });
  </script>

</body>
</html>
