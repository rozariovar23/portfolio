# portfolio
Portfolio has been created to enhance my skills and profile through personal website. It has been created using html and css
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ROZARIO A | AI & Data Analytics Engineer</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>
:root{
    --bg:#0b0f19;
    --card:#111827;
    --accent:#00e5ff;
    --accent2:#00ff9d;
    --text:#ffffff;
    --sub:#a8b2d1;
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    background:var(--bg);
    color:var(--text);
}

section{
    padding:90px 10%;
}

h2{
    font-size:2.5rem;
    margin-bottom:30px;
    color:var(--accent);
    text-align:center;
}

.navbar{
    position:fixed;
    width:100%;
    top:0;
    z-index:1000;
    background:rgba(0,0,0,0.8);
    backdrop-filter:blur(10px);
    padding:15px 10%;
}

.nav-container{
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    color:var(--accent);
    font-weight:700;
    font-size:1.4rem;
}

.nav-links{
    display:flex;
    gap:25px;
}

.nav-links a{
    color:white;
    text-decoration:none;
    transition:.3s;
}

.nav-links a:hover{
    color:var(--accent2);
}

.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:space-between;
    flex-wrap:wrap;
    gap:40px;
}

.hero-text{
    flex:1;
    animation:fadeIn 1.2s ease;
}

.quote{
    font-size:2rem;
    font-weight:700;
    color:var(--accent2);
    margin-bottom:20px;
}

.hero h1{
    font-size:3.5rem;
    margin-bottom:15px;
}

.highlight{
    color:var(--accent);
}

.hero p{
    color:var(--sub);
    line-height:1.8;
    max-width:650px;
}

.hero-image{
    flex:1;
    display:flex;
    justify-content:center;
}

.hero-image img{
    width:320px;
    height:320px;
    border-radius:50%;
    object-fit:cover;
    border:4px solid var(--accent);
    box-shadow:0 0 40px var(--accent);
}

.btn-group{
    margin-top:30px;
}

.btn{
    display:inline-block;
    padding:12px 25px;
    margin-right:15px;
    text-decoration:none;
    border-radius:8px;
    font-weight:600;
    transition:.3s;
}

.primary{
    background:var(--accent);
    color:black;
}

.secondary{
    border:2px solid var(--accent);
    color:var(--accent);
}

.btn:hover{
    transform:translateY(-4px);
}

.card{
    background:var(--card);
    padding:30px;
    border-radius:15px;
    border-left:4px solid var(--accent);
}

.about p,
.education p,
.experience p{
    color:var(--sub);
    line-height:1.9;
}

.education-card,
.exp-card{
    background:var(--card);
    padding:25px;
    border-radius:15px;
    border:1px solid var(--accent);
    text-align:center;
}

.skills-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
}

.skill{
    background:var(--card);
    padding:25px;
    text-align:center;
    border-radius:15px;
    transition:.4s;
}

.skill:hover{
    transform:translateY(-8px);
    box-shadow:0 0 20px rgba(8, 4, 202, 0.3);
}

.project-card{
    background:var(--card);
    border-radius:15px;
    padding:30px;
    transition:.4s;
}

.project-card:hover{
    transform:translateY(-8px);
    border:1px solid var(--accent);
}

.project-title{
    color:var(--accent2);
    margin-bottom:15px;
}

.contact-container{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:30px;
}

.contact-info{
    background:var(--card);
    padding:25px;
    border-radius:15px;
}

.contact-form{
    background:var(--card);
    padding:25px;
    border-radius:15px;
}

input, textarea{
    width:100%;
    padding:12px;
    margin-bottom:15px;
    border:none;
    border-radius:8px;
    background:#1f2937;
    color:white;
}

button{
    background:var(--accent);
    color:rgb(17, 16, 16);
    border:none;
    padding:12px 25px;
    border-radius:8px;
    cursor:pointer;
    font-weight:600;
}

footer{
    text-align:center;
    padding:25px;
    color:var(--sub);
}

@keyframes fadeIn{
    from{
        opacity:0;
        transform:translateY(20px);
    }
    to{
        opacity:1;
        transform:translateY(0);
    }
}

@media(max-width:768px){

    .hero{
        flex-direction:column-reverse;
        text-align:center;
    }

    .hero h1{
        font-size:2.5rem;
    }

    .quote{
        font-size:1.5rem;
    }

    .contact-container{
        grid-template-columns:1fr;
    }

    .nav-links{
        display:none;
    }
}
</style>
</head>

<body>

<nav class="navbar">
    <div class="nav-container">
        <div class="logo">ROZARIO A</div>

        <div class="nav-links">
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#education">Education</a>
            <a href="#experience">Experience</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </div>
    </div>
</nav>

<section class="hero" id="home">

    <div class="hero-text">

        <div class="quote">
            “I don’t just learn skills — I apply them.”
        </div>

        <h1>
            Hi, I'm <span class="highlight">ROZARIO A</span>
        </h1>

        <p>
            I am a graduate coder with a strong interest in
            <span class="highlight">Machine Learning</span>,
            <span class="highlight">Deep Learning</span>,
            <span class="highlight">SQL</span>, and
            <span class="highlight">Data Engineering</span>.
            My long-term goal is to become a versatile Full Stack Developer
            through continuous learning and hands-on training.
        </p>

        <div class="btn-group">
            <a href="#projects" class="btn primary">View Projects</a>
            <a href="#contact" class="btn secondary">Contact Me</a>
        </div>

    </div>

    <div class="hero-image">
        <!-- Replace image path -->
        <img src="c:\Users\Administrator\Pictures\WhatsApp Image 2026-04-30 at 6.47.20 PM.jpeg" alt="ROZARIO A">
    </div>

</section>

<section id="about">
    <h2>About Me</h2>

    <div class="card">
        <p>
            I am an aspiring AI and Data Analytics Engineer passionate about
            transforming knowledge into practical solutions. My interests span
            Machine Learning, Deep Learning, SQL, Data Engineering, and Data Analytics.
            I enjoy solving complex problems through logical thinking and analytical
            approaches. With a mindset focused on continuous learning and innovation,
            I aim to grow into a skilled Full Stack Developer capable of building
            impactful technology solutions.
        </p>
    </div>
</section>

<section id="education">
    <h2>Education</h2>

    <div class="education-card">
        <h3><span class="highlight">B.Tech in Artificial Intelligence and Data Science</span></h3>
        <br>
        <p>Saranathan College of Engineering and Technology</p>
        <p>2023 – 2027</p>
    </div>
</section>

<section id="experience">
    <h2>Experience & Training</h2>

    <div class="exp-card">
        <h3>Fresher</h3>
        <br>
        <p>
            Completed a 12-week Certified Machine Learning Course with
            hands-on exposure to model development, data preprocessing,
            machine learning workflows, practical implementation and 
            trained as a Data Analytic intern. 
        </p>
    </div>
</section>

<section id="skills">
    <h2>Skills & Expertise</h2>

    <div class="skills-grid">

        <div class="skill">🤖<br><br>Machine Learning</div>

        <div class="skill">🧠<br><br>Deep Learning</div>

        <div class="skill">🗄️<br><br>SQL</div>

        <div class="skill">⚙️<br><br>Data Engineering</div>

        <div class="skill">📊<br><br>Data Analytics</div>

        <div class="skill">💡<br><br>Logical Thinking</div>

        <div class="skill">🚀<br><br>Problem Solving</div>

    </div>
</section>

<section id="projects">

    <h2>Projects</h2>

    <div class="project-card">

        <h3 class="project-title">
            Lane Detection in Automated Vehicles using Deep Learning
        </h3>

        <p>
            Developed a deep learning-based system to detect road lanes
            for automated vehicles, enhancing safety and navigation
            accuracy through intelligent lane recognition and tracking.
        </p>
        
        

    </div>
<br>
<div class="project-card">

        <h3 class="project-title">
            Weather reporting application.
        </h3>

        <p>
           The application just created to know the weather reported in
           particular cities by searching in search bar. I have provided the
           necessary requirements with neat dashboard
        </p>
        
        

    </div>
    <br>
    <div class="project-card">

        <h3 class="project-title">
            Handwritten-digit-recognition.
        </h3>

        <p>
           Handwritten Digit Recognition (HDR) is an application of
            Artificial Intelligence, Machine Learning, and Computer Vision that 
            automatically identifies and classifies handwritten numbers (0–9) from images.
        </p>
        
        

    </div>
</section>

<section id="contact">

    <h2>Contact</h2>

    <div class="contact-container">

        <div class="contact-info">
            <h3>Email</h3>
            <br>
            <p>📧 rozariovar23@gmail.com </p>
            <br>

            <h3> Github💼</h3>
            <br>
            <p> https://github.com/rozariovar23</p>
        </div>



        <div class="contact-info">
            
            <h3>linkedIn🔗</h3>
            <br>
            <p> https://www.linkedin.com/in/rozarioa2005?utm_source=share_via&utm_content=profile&utm_medium=member_android</p>

        </div>

        <div class="contact-form">

            <form>

                <input type="text" placeholder="Your Name" required>

                <input type="email" placeholder="Your Email" required>

                <textarea rows="5" placeholder="Your Message"></textarea>

                <button type="submit">Send Message</button>

            </form>

        </div>

    </div>

</section>

<footer>
    © 2026 ROZARIO A | AI & Data Analytics Engineer
</footer>

</body>
</html>
