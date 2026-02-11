<!DOCTYPE html>
<html lang="en">
    
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
    <link rel="stylesheet" href="style.css">
    <title>Portfolio Website</title>
</head>
<body>
    <header>
        <a href="#" class="logo">ANMOL MISHRA</a>

        <nav>
            <a href="#" class="active"> Home</a>
            <a href="#" >Services</a>
            <a href="#" >Skills</a>
            <a href="#" >Education</a>
            <a href="#" >Experience</a>
            <a href="#" >Contact</a>
        </nav>
    </header>
    <section class="home">
        <div class="home-img">
            <img src="logo.png" alt="">
        </div>
        <div class="home-content">
            <h1>Hi, It's <span>ANMOL</span></h1>
            <h3 class="typing-text">I'm a <span></span></h3>
            <p>B.Tech student and passionate coder focused on web development and problem-solving. I love building clean, efficient, and user-friendly projects while continuously learning new technologies..</p>
            <div class="social-icons">
                <a href="https://www.linkedin.com/in/anmol-mishra-39a648362"><i class="fa-brands fa-linkedin"></i></a>
                <a href="https://github.com/ANMOLMISHRA-GG?"><i class="fa-brands fa-github"></i></a>
                <a href="https://x.com/AnmolMishra52"><i class="fa-brands fa-x-twitter"></i></a>
                <a href="https://www.instagram.com/codefusionai"><i class="fa-brands fa-instagram"></i></a>
            </div>
          <a href="mailto: anmolmishra12103@gmail.com?subject=hello&body=Message"
            target="_blank" class="btn">Contact me</a>
            <div class="orb orb1"></div>
    <div class="orb orb2"></div>
    <div class="orb orb3"></div>

    <div class="container">

        <div class="skills-grid">
            <!-- Frontend -->
            <div class="skill-category frontend">
                <div class="category-header">
                    <div class="category-icon"></div>
                    <h2 class="category-title">Frontend</h2>
                </div>
                <div class="skills-list">
                    <span class="skill-tag">HTML5</span>
                    <span class="skill-tag">CSS3</span>
                    <span class="skill-tag">JavaScript</span>
                    <span class="skill-tag">TypeScript</span>
                    <span class="skill-tag">React</span>
                    <span class="skill-tag">Vue.js</span>
                    <span class="skill-tag">Next.js</span>
                </div>
            </div>
            
            <div class="skill-category backend">
                <div class="category-header">
                    <div class="category-icon"></div>
                    <h2 class="category-title">Backend</h2>
                </div>
                <div class="skills-list">
                    <span class="skill-tag">Node.js</span>
                    <span class="skill-tag">Express.js</span>
                    <span class="skill-tag">Python</span>
                </div>
            </div>

            <!-- Tools -->
            <div class="skill-category tools">
                <div class="category-header">
                    <div class="category-icon"></div>
                    <h2 class="category-title">Tools</h2>
                </div>
                <div class="skills-list">
                    <span class="skill-tag">Git</span>
                    <span class="skill-tag">GitHub</span>
                    <span class="skill-tag">VS Code</span>
                    <span class="skill-tag">AWS</span>
                    <span class="skill-tag">Linux</span>
                </div>
            </div>
        </div>
    </div>
        </div>
    </section>
</body>
</html>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    font-family: 'Poppins', sans-serif;
}

html{
    font-size: 62.5%;
}

body{
    width: 100%;
    height: 100vh;
    overflow-x: hidden;
    background-color: darkgray;
    color: black;
}

header{
    margin-top: 20px;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 1rem 9%;
    background-color: transparent;
    filter: drop-shadow(10px);
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}

.logo{
    font-size: 3rem;
    color: #00008b;
    font-weight: 800;
    cursor: pointer;
    transition: 0.5s ease;
}

.logo:hover{
    transform: scale(1.1);
}

nav a{
    font-size: 1.8rem;
    color: black;
    margin-left: 4rem;
    font-weight: 500;
    transition: 0.3s ease;
    border-bottom: 3px solid transparent;
}

nav a:hover,
nav a.active{
    color: #00008b;
    border-bottom: 3px solid #00008b;
}

@media(max-width:995px){
    nav{
        position: absolute;
        display: none;
        top: 0;
        right: 0;
        width: 40%;
        border-left: 3px solid #00008b;
        border-bottom: 3px solid #00008b;
        border-bottom-left-radius: 2rem;
        padding: 1rem solid;
        background-color: darkgray;
        border-top: 0.1rem solid rgba(0,0,0,0.1);
    }

    nav.active{
        display: block;
    }

    nav a{
        display: block;
        font-size: 2rem;
        margin: 3rem 0;
    }

    nav a:hover,
    nav a.active{
        padding: 1rem;
        border-radius: 0.5rem;
        border-bottom: 0.5rem solid #00008b;
    }
}

section{
    min-height: 100vh;
    padding: 5rem 9% 5rem;
}

.home{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 8rem;
    background-color: darkgray;
}

.home .home-content h1{
    font-size: 6rem;
    font-weight: 700;
    line-height: 1.3;
}

span{
    color: #00008b;
}

.home-content h3{
    font-size: 4rem;
    margin-bottom: 1rem;
    font-weight: 700;
}

.home-content p{
    font-size: 1.6rem;
}

.home-img{
    border-radius: 50%;
}

.home-img img{
    position: relative;
    width: 32vw;
    border-radius: 50%;
    box-shadow: 0 0 25px solid #00008b;
    cursor: pointer;
    transition: 0.2s linear;
}

.home-img img:hover{
    font-size: 1.8rem;
    font-weight: 500;
}

.social-icons a{
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 4rem;
    height: 4rem;
    background-color: transparent;
    border: 0.2rem solid #00008b;
    font-size: 2rem;
    border-radius: 50%;
    margin: 3rem 1.5rem 3rem 0;
    transition: 0.3s ease;
    color: #00008b;
}

.social-icons a:hover{
    color: white;
    transform: scale(1.3) translateY(-5px);
    background-color: #00008b;
    box-shadow: 0  0 25px #00008b;
}

.btn{
    display: inline-block;
    padding: 1rem 2.8rem;
    background-color: darkgray;
    border-radius: 4rem;
    font-size: 1.6rem;
    color: #00008b;
    letter-spacing: 0.3rem;
    font-weight: 600;
    border: 2px solid #00008b;
    transition: 0.3s ease;
    cursor: pointer;
}

.btn:hover{
    transform: scale3d(1.03);
    background-color: #00008b;
    color: darkgray;
    box-shadow: 0 0 25px #00008b;
}

.typing-text{
    font-size: 34px;
    font-weight: 600;
    min-width: 280px;
}

.typing-text span{
    position: relative;
}

.typing-text span::before{
    content: "software Developer";
    color: #00008b;
    animation: words 20s infinite;
}

.typing-text span::after{
    content: "";
    background-color: darkgray;
    position: absolute;
    width: calc(100% + 8px);
    height: 100%;
    border-left: 3px solid darkgray;
    right: -8;
    animation: cursor 0.6s infinite;
}

@keyframes cursor{
    to{
        border-left: 3px solid #00008b;
    }
}

@keyframes words{
    0%, 20%{
        content: "Web Developer";
    }
    21%, 40%{
        content: "Developer";
    }
    41%, 60%{
        content: "Web Designer";
    }
    61%, 80%{
        content: "Instagram Creator";
    }
    81%, 100%{
        content: "Graphic designer";
    }
}

@media (max-width: 1000px){
    .home{
        gap: 4rem;
    }
}

@media(max-width:995px){
    .home{
        flex-direction: column;
        margin: 5rem 4rem;
    }

    .home .home-content h3{
        font-size: 2.5rem;
    }

    .home-content h1{
        font-size: 5rem;
    }

    .home-img img{
        width: 70vw;
        margin-top: 4rem;
    }
}
:root {
  --bg-primary: darkgray;
  --bg-secondary: darkgray;
  --accent-blue: darkblue;
  --text-primary: #e5e5e5;
  --text-secondary: #a0a0a0;
  --card-bg: rgba(255, 255, 255, 0.08);
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Outfit', sans-serif;
  background: var(--bg-primary);
  color: var(--text-primary);
}

.container {
  max-width: 1200px;
  margin: auto;
  padding: 60px 20px;
}
header {
  text-align: center;
  margin-bottom: 60px;
}

h1 {
  font-size: 3rem;
  font-weight: 700;
  color: var(--accent-blue);
  margin-bottom: 10px;
}

.subtitle {
  color: var(--text-secondary);
  font-size: 1rem;
  letter-spacing: 1px;
}

.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 30px;
}

.skill-category {
  background: var(--card-bg);
  backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.15);
  border-radius: 20px;
  padding: 30px;
  transition: 0.3s ease;
}

.skill-category:hover {
  transform: translateY(-8px);
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
  border-color: var(--accent-blue);
}

.category-header {
  display: flex;
  align-items: center;
  gap: 12px;
  margin-bottom: 20px;
}

.category-icon {
  font-size: 2rem;
}

.category-title {
  font-size: 1.5rem;
  color: var(--accent-blue);
}

.skills-list {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.skill-tag {
  font-family: 'sans-serif', monospace;
  font-size: 0.85rem;
  padding: 8px 14px;
  background: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.15);
  border-radius: 6px;
  transition: 0.3s ease;
}

.skill-tag:hover {
  background: rgba(255, 255, 255, 0.12);
  border-color: var(--accent-blue);
  transform: scale(1.05);
}

@media (max-width: 768px) {
  h1 {
    font-size: 2.2rem;
  }

  .skill-category {
    padding: 25px;
  }
}


::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-thumb {
  background: var(--accent-blue);
  border-radius: 10px;
}
