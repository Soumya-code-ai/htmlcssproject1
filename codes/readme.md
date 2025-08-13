<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Soumya's Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

   
    <header>
        <nav>
            <div class="logo">Soumya <span>Ranjan</span></div>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <h1>Hi, I'm <span>Soumya</span></h1>
        <p>A Passionate Developer & Problem Solver</p>
        <a href="#projects" class="btn">View My Work</a>
    </section>

    <section id="about">
        <h2>About Me</h2>
        <div class="about-content">
            <img src="download.jpg" alt="Soumya's photo">
            <p>
                I am Soumya Ranjan, currently pursuing my undergraduate degree at Christ University. 
                I enjoy solving problems, building creative projects, and continuously learning new skills.
            </p>
        </div>
    </section>

   
    <section id="skills">
        <h2>Skills</h2>
        <ul class="skill-list">
            <li>HTML & CSS</li>
            <li>C Programming</li>
            <li>Java</li>
            <li>Problem Solving</li>
            <li>Team Collaboration</li>
        </ul>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2>Projects</h2>
        <div class="project-card">
            <h3>Firefighter Robot</h3>
            <p>A robot capable of detecting and extinguishing fires automatically.</p>
        </div>
        <div class="project-card">
            <h3>Operating System Simulation</h3>
            <p>Designed a simulation of OS-level process management techniques.</p>
        </div>
    </section>

   
    <section id="contact">
        <h2>Contact Me</h2>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" rows="5" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>@ 2025 Soumya Ranjan | All Rights Reserved</p>
    </footer>

</body>
</html>
css->
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background: #0f172a;
    color: #f8fafc;
}

/* Navigation */
header {
    background: rgba(15, 23, 42, 0.9);
    padding: 15px 50px;
    position: sticky;
    top: 0;
    backdrop-filter: blur(8px);
    z-index: 1000;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 26px;
    font-weight: bold;
}

.logo span {
    color: #38bdf8;
}

nav ul {
    display: flex;
    list-style: none;
}

nav ul li {
    margin-left: 25px;
}

nav ul li a {
    text-decoration: none;
    color: #f8fafc;
    transition: 0.3s;
}

nav ul li a:hover {
    color: #38bdf8;
}

/* Hero Section */
.hero {
    text-align: center;
    padding: 100px 20px;
    animation: fadeIn 1.5s ease-in-out;
}

.hero span {
    color: #38bdf8;
}

.btn {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 20px;
    background: #38bdf8;
    color: #0f172a;
    font-weight: bold;
    border-radius: 25px;
    text-decoration: none;
    transition: transform 0.3s, background 0.3s;
}

.btn:hover {
    transform: scale(1.1);
    background: #0ea5e9;
}

/* About */
#about {
    padding: 60px 20px;
    text-align: center;
}

.about-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 20px;
}

.about-content img {
    width: 220px;
    height: 280px;
    border-radius: 10px;
    margin-bottom: 15px;
    box-shadow: 0px 4px 12px rgba(0,0,0,0.5);
    transition: transform 0.3s;
}

.about-content img:hover {
    transform: scale(1.05);
}

.about-content p {
    max-width: 600px;
    line-height: 1.6;
}

/* Skills */
#skills {
    padding: 60px 20px;
    text-align: center;
}

.skill-list {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.skill-list li {
    background: #1e293b;
    margin: 8px;
    padding: 10px 15px;
    border-radius: 20px;
    transition: transform 0.3s, background 0.3s;
}

.skill-list li:hover {
    background: #38bdf8;
    color: #0f172a;
    transform: translateY(-5px);
}

/* Projects */
#projects {
    padding: 60px 20px;
    text-align: center;
}

.project-card {
    background: #1e293b;
    padding: 20px;
    margin: 15px auto;
    border-radius: 10px;
    max-width: 600px;
    transition: transform 0.3s, background 0.3s;
}

.project-card:hover {
    background: #38bdf8;
    color: #0f172a;
    transform: translateY(-5px);
}

/* Contact */
#contact {
    padding: 60px 20px;
    text-align: center;
}

form {
    display: flex;
    flex-direction: column;
    max-width: 400px;
    margin: auto;
}

form input, form textarea {
    margin: 8px 0;
    padding: 10px;
    border: none;
    border-radius: 8px;
    outline: none;
}

form button {
    padding: 10px;
    background: #38bdf8;
    color: #0f172a;
    font-weight: bold;
    border: none;
    border-radius: 25px;
    cursor: pointer;
    transition: transform 0.3s, background 0.3s;
}

form button:hover {
    background: #0ea5e9;
    transform: scale(1.05);
}

/* Footer */
footer {
    background: #1e293b;
    padding: 15px;
    text-align: center;
    margin-top: 40px;
}

/* Animations */
@keyframes fadeIn {
    0% { opacity: 0; transform: translateY(30px); }
    100% { opacity: 1; transform: translateY(0); }
}
