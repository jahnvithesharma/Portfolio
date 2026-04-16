<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jahnvi | Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navbar -->
    <nav>
        <h2>Jahnvi</h2>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <h1>Hello, I'm Jahnvi 👋</h1>
        <p>1st Year B.Tech CSE Student at Manav Rachna University</p>
        <button onclick="scrollToSection('contact')">Contact Me</button>
    </section>

    <!-- About -->
    <section id="about">
        <h2>About Me</h2>
        <p>
            I am a passionate Computer Science student currently in my first year at Manav Rachna University. 
            I am exploring programming, web development, and electronics projects using Raspberry Pi Pico. 
            I enjoy building real-world projects and continuously improving my technical skills.
        </p>
    </section>

    <!-- Skills -->
    <section id="skills">
        <h2>Skills</h2>
        <div class="skills-container">
            <div class="skill">C Programming</div>
            <div class="skill">Python (Basics)</div>
            <div class="skill">HTML</div>
            <div class="skill">CSS</div>
            <div class="skill">JavaScript (Basics)</div>
            <div class="skill">Problem Solving</div>
            <div class="skill">Data Structures (Basic)</div>
            <div class="skill">Electronics Basics</div>
            <div class="skill">Raspberry Pi Pico</div>
            <div class="skill">Git & GitHub</div>
        </div>
    </section>

    <!-- Projects -->
    <section id="projects">
        <h2>Projects</h2>
        <div class="project-card">
            <h3>Smart Waste Segregation System</h3>
            <p>Built using Raspberry Pi Pico to separate waste into wet, dry, and metal categories using sensors.</p>
        </div>

        <div class="project-card">
            <h3>Automated Dustbin</h3>
            <p>A touchless dustbin using ultrasonic sensor and servo motor.</p>
        </div>

        <div class="project-card">
            <h3>Dice Simulation (MATLAB)</h3>
            <p>Simulation project demonstrating probability concepts using MATLAB.</p>
        </div>
    </section>

    <!-- Contact -->
    <section id="contact">
        <h2>Contact Me</h2>
        <p>Email: jahnvi@example.com</p>
        <p>LinkedIn: linkedin.com/in/jahnvi</p>
        <p>GitHub: github.com/jahnvi</p>
    </section>

    <footer>
        <p>© 2026 Jahnvi | Portfolio</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background: #0f172a;
    color: #fff;
}

/* Navbar */
nav {
    display: flex;
    justify-content: space-between;
    padding: 20px 50px;
    background: #020617;
    position: sticky;
    top: 0;
}

nav ul {
    display: flex;
    list-style: none;
    gap: 20px;
}

nav a {
    text-decoration: none;
    color: #38bdf8;
    transition: 0.3s;
}

nav a:hover {
    color: white;
}

/* Hero */
.hero {
    text-align: center;
    padding: 100px 20px;
}

.hero h1 {
    font-size: 40px;
}

.hero p {
    margin: 15px 0;
    font-size: 18px;
}

.hero button {
    padding: 10px 20px;
    border: none;
    background: #38bdf8;
    color: black;
    cursor: pointer;
    border-radius: 5px;
}

/* Sections */
section {
    padding: 60px 40px;
    text-align: center;
}

h2 {
    margin-bottom: 20px;
    color: #38bdf8;
}

/* Skills */
.skills-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
}

.skill {
    padding: 10px 20px;
    background: #1e293b;
    border-radius: 20px;
}

/* Projects */
.project-card {
    background: #1e293b;
    padding: 20px;
    margin: 15px auto;
    width: 80%;
    border-radius: 10px;
}

/* Footer */
footer {
    text-align: center;
    padding: 20px;
    background: #020617;
}
function scrollToSection(sectionId) {
    document.getElementById(sectionId).scrollIntoView({
        behavior: "smooth"
    });
}
