<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Code Canvas: WS101 Creations</title>
  <style>
      
    * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    line-height: 1.6;}

body{
    background-color: #1E1E1E;
    color: #EAEAEA;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
}
nav ul {
    display: flex;
    justify-content: right;
    gap: 20px;
    list-style-type: none;
    background-color: #2A2A2A;
    padding: 10px 0;
    border-radius: 12px;
}

nav li a {
    color: #EAEAEA;
    text-decoration: none;
    padding: 10px 15px;
    transition: 0.3s;
}

nav li a:hover {
    background-color: #FF69B4;
    color: #ffffff;
    border-radius: 8px;
}

a {
    text-decoration: none;
    color: #D16D9E;
}
a:hover{
        color:#FF4FA3;
        transform: scale(1.05);     
    box-shadow: 0 0 15px #FF4FA3;
    }
.link {
    display: inline-block;
    padding: 8px 18px;
    border: 2px solid #FF69B4;
    border-radius: 8px;
    color: #FF69B4;
    font-weight: 500;
    transition: 0.3s;
    text-decoration: none;
}

.link:hover {
    background-color: #FF69B4;
    color: #ffffff;
    box-shadow: 0 0 10px rgba(255,105,180,0.4);
    transform: scale(1.05);
}
.img1 {
    border-radius: 50%;
    display: block;
    margin: 20px auto;
    width: 180px;
    border: 4px solid #FF69B4;
    box-shadow: 0 0 25px rgba(255,105,180,0.5);
}
.topics {
    border:none;
    padding: 20px;
    border-radius: 12px;
    margin: 20px auto;
    width: 80%;
    max-width: 900px;
    background-color: rgba(42,42,42,0.8); 
    transition: 0.3s;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.5);
    transition: transform 0.3s ease, box-shadow 0.3s ease, background 0.3s ease;
}
#Aboutme {
  padding-left: 30px;
}

#Aboutme li {
  margin-bottom: 3px;
  color: #EAEAEA;
 
}
#Aboutme li::marker{
  color: #ff66b2;
  display: inline-block;
  width: 1em; 
  margin-left: 2px; 
  font-size: 20px; 
  vertical-align: middle; 
}
.about-quote {
  border-left: 3px solid #FF69B4;
  padding-left: 15px;
  font-style: italic;
  margin-top: 20px;
  color: #FF69B4;
  text-align: left;
}
ul {
    padding-left: 20px;
}
h1{
            text-align: center;
            color: #D16D9E;
        }
h2{
    color: #D16D9E;
    margin-bottom: 5px;
}
footer{
    text-align:center; 
    color:#B0B0B0; 
    margin: 30px 0;
}
#Skills ul li {
    padding-left: 30px;
}
#Skills ul{
    margin-bottom: 5px;
}
.lt{
    padding: 15px 20px;
    margin-bottom: 20px;
    border-radius: 10px;
    background: rgba(252, 70, 161, 0.1); 
    border: 1px solid rgba(254, 61, 157, 0.2);
    color: #ffffff; 
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
    transition: transform 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94), 
                box-shadow 0.3s ease, 
                background 0.3s ease;
}
.lt:hover {
    transform: translateX(8px) translateY(-2px);
    
    
    box-shadow: 10px 10px 25px rgba(0, 0, 0, 0.5), 
                0 0 20px rgba(255, 105, 180, 0.4);
    
    background: rgba(255, 105, 180, 0.2); 
    border-color: rgba(255, 105, 180, 0.6);
}
#Projects{
    padding: 15px 20px;
    margin-bottom: 20px;
    border-radius: 10px;
    border: none; 
   background: rgba(255, 255, 255, 0.05); 
    color: #ffffff; 
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.5);
    
    transition: transform 0.3s ease, box-shadow 0.3s ease, background 0.3s ease;
}
#Skills{
     background: rgba(255, 77, 166, 0.08);
}
#tabi{
    display: flex; 
    gap: 20px; 
    margin: 0 auto;
    width: 900px;
}
.back2top {
  position: fixed;
  bottom: 30px;
  right: 30px;
  width: 50px;
  height: 50px;
  background-color: #1a1a1a; 
  color: #ff66b2; 
  border: 2px solid #ff66b2;
  border-radius: 50%;
  cursor: pointer;
  font-size: 24px;
  font-weight: bold;
  transition: all 0.3s ease;
  box-shadow: 0 0 10px rgba(255, 102, 178, 0.3);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1000;
}
.back2top:hover {
  background-color: #ff66b2;
  color: #ffffff;
  box-shadow: 0 0 20px rgba(255, 102, 178, 0.6);
  transform: translateY(-5px); /* Lift effect */
}
#Projects p {
  color:  #cccccc;
}
#Education ul li{
    margin-bottom: 10px;
}
#Portfolio {
   
    background-color:  #75475d;;
    padding: 40px 20px;
    border-radius: 20px;
    box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.8);
    backdrop-filter: blur(10px);
    max-width: 900px;
    margin: 20px auto;
}

#Portfolio h2 {
    text-align: center;
    font-style: italic;
    font-weight: 900;
    font-size: 3em;
    margin: 0 0 15px 0;
    background: linear-gradient(to right, #ff69b4, #ffffff, #ff1493);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    filter: drop-shadow(0px 0px 8px rgba(255, 105, 180, 0.5));
    letter-spacing: 1px;
}

#Portfolio p {
    text-align: center;
    color: #e0e0e0; 
    max-width: 700px;
    margin: 0 auto;
    font-size: 1.1em;
}


#Contacts {
    background-color: rgb(65, 61, 61);
    border: 1px solid rgba(255, 105, 180, 0.2);
    position: relative;
    overflow: hidden;
    padding: 15px; 
}

#Contacts::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 3px;
    background: linear-gradient(90deg, transparent, #FF69B4, #FF1493, transparent);
}

.contact-container {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 10px; 
    margin: 10px 0; 
    padding: 10px; 
}

.contact-card {
    display: flex;
    align-items: center;
    padding: 10px 10px;
    background: rgba(42, 42, 42, 0.8);
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 105, 180, 0.2);
    border-radius: 10px;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
}

.contact-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 105, 180, 0.08), transparent);
    opacity: 0;
    transition: opacity 0.3s ease;
}

.contact-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.4), 0 0 15px rgba(255, 105, 180, 0.2);
    border-color: rgba(255, 105, 180, 0.4);
}

.contact-card:hover::before { opacity: 1; }

.contact-icon {
    font-size: 1.6em; 
    margin-right: 12px;
    filter: drop-shadow(0 0 6px rgba(255, 105, 180, 0.4));
    transition: all 0.3s ease;
    flex-shrink: 0;
}

.contact-card:hover .contact-icon {
    transform: scale(1.05);
    filter: drop-shadow(0 0 12px rgba(255, 105, 180, 0.6));
}

.contact-info h3 {
    color: #FF69B4;
    font-size: 0.9em;
    margin-bottom: 2px;
    font-weight: 600;
    text-transform: uppercase;
}

.contact-link, .phone-number {
    color: #EAEAEA;
    font-size: 0.85em; 
    font-weight: 500;
    display: block;
    transition: all 0.3s ease;
    line-height: 1.3;
}

.contact-link:hover, .phone-number:hover {
    color: #FF69B4;
    text-shadow: 0 0 6px rgba(255, 105, 180, 0.4);
    transform: translateX(2px);
}

.email-card .contact-icon { color: #FF6B9D; }
.phone-card .contact-icon { color: #FF8E53; }
.fb-card .contact-icon { color: #4267B2; }
.location-card .contact-icon { color: #4ECDC4; }

.contact-cta {
    text-align: center;
    margin-top: 12px; 
    padding: 8px; 
    background: rgba(255, 105, 180, 0.06);
    border-radius: 6px;
    border: 1px solid rgba(255, 105, 180, 0.15);
}

.contact-cta p {
    color: #FF69B4;
    font-size: 0.9em; 
    font-weight: 500;
    margin: 0;
}

.contact-link {
    pointer-events: auto;
    z-index: 10;
    position: relative;
}

.contact-card:hover .contact-link {
    pointer-events: auto;
    z-index: 20;
}
@media (max-width: 768px) {
    .contact-container { grid-template-columns: 1fr; }
    #Contacts { padding: 12px; }
    .contact-card { padding: 10px 8px; flex-direction: column; text-align: center; }
    .contact-icon { margin-right: 0; margin-bottom: 8px; font-size: 2em; }
}

   @media (max-width: 768px) {
    nav ul {
        display: flex;
        flex-direction: column;
    }
    nav li {
        float: none;
        width: 100%;
    }
}
        
  </style>
        
</head>
<body>
<div id="top"></div>
  <nav>
    <ul>
     <li><a href="#Aboutme">About Me</a></li>
     <li><a href="#Skills">Skills</a></li>
     <li><a href="#Education">Education</a></li>
     <li><a href="#Projects">Projects</a></li>
     <li><a href="#Contacts">Contacts</a></li>
    </ul>
  </nav>  

  <img class="img1" src="MIDTERMS TASKS/portfolio/pic.jpg" >
  <h1>Francine Jayde S. Delfina</h1>
<div class="topics"  id="Portfolio">
  <h2 style="text-align: center;">Code Canvas: WS101 Creations</h2>
  <p style="text-align: center;"> Welcome to my WS 101 Portfolio!<br> This portfolio is a glimpse of my learning journey, featuring my lab tasks and the creativity I explored throughout the course.</p>
</div>

  <div  class="topics"  id="Aboutme">
  <h2>👤 About me</h2>
  <ul>
        <li>🏫 BSIT student at Pampanga State Agricultural University</li>
        <li>🎯 Passionate about technology and problem-solving</li>
        <li>💻 Knowledge in computer systems and software applications</li>
        <li>🛠️ Experience in Python and Java</li>
        <li>🎨 Loves designing websites using HTML and CSS</li>
        <li>🚀 Continuously learning and improving in IT</li>
      </ul>
      <p class="about-quote">
        “I aim to grow as a developer and create impactful digital solutions.”
      </p>
  </div>

  <div id="tabi">
  <div class="topics" id="Skills">
<h2>🧠 Skills</h2>
<h3>🌐 Web Development</h3>
      <ul style="list-style: none; padding: 0;">
        <li>HTML</li>
        <li>CSS</li>
        <li>Responsive Design</li>
      </ul>
<h3>⚙️ Programming</h3>
      <ul style="list-style: none; padding: 0;">
        <li>Python</li>
        <li>Java</li>
      </ul>
<h3>🤝 Soft Skills</h3>
      <ul style="list-style: none; padding: 0;">
        <li>Time Management</li>
        <li>Flexible & Adaptable</li>
        <li>Fast Learner</li>
        <li>Good at Collaboration</li>
        <li>Problem Solving</li>
        <li>Eager to Learn</li>
      </ul>
  </div>
<div class="topics"  id="Education">
<h2>🎓 Education</h2>
  <ul type="round">
   <li><strong>Currently:</strong> Bachelors of Science in Information Technology<br>
        <em>Pampanga State Agricultural University • Expected 2029</em></li>
    <li>STEM<br><em>Andres M. Luciano High School • 2025</em></li>
    <li>Junior High School<br><em>Andres M. Luciano High School • 2023</em></li> 
    <li>Elementary School<br><em>San Miguel Elementary School • 2017</em></li>
  </ul>
</div>
  </div>

<div class="topics" id="Projects">
<h2 >📂 Projects</h2>
<p>Hands-on projects from my Web Systems 101. Progressive <strong>HTML & CSS</strong> exercises. From basic layouts to responsive designs—my learning journey in web development.</p><br>
<h2 style="text-align: center; color: #FF69B4; margin-bottom: 20px;">📚 Midterms</h2>

<div class="lt">
<h3>Lab Task 1: </h3>
<p>Created a personal resume using basic HTML structure and formatting. This task helped me understand how to organize content using headings, paragraphs, and lists.</p>
<a href="MIDTERMS TASKS/portfolio/labtask1.html" target="_blank" class="link">MidTerm Task 1: Resume Writing using HTML</a>
</div>

<div class="lt">
<h3>Lab Task 2:</h3>
<p>Developed a webpage using ordered and unordered lists, as well as tables. This activity improved my understanding of structuring data and presenting information clearly.</p>
<a href="MIDTERMS TASKS/portfolio/labtask2.html" target="_blank" class="link">Midterm Task 2: HTML List and Tables</a>
</div>

<div class="lt">
<h3>Lab Task 3:</h3>
<p>Created an interactive image map with clickable areas that link to different sections or pages. This task enhanced my knowledge of image mapping and user interaction.</p>
<a href="MIDTERMS TASKS/portfolio/labtask3.html" target="_blank" class="link">Midterm Task 3: Image Maps</a>
</div>

<div class="lt">
<h3>Lab Task 4:</h3>
<p>Built a form that collects user input such as text, selections, and buttons. This helped me learn how forms work and how to structure input fields properly.</p>
<a href="MIDTERMS TASKS/portfolio/labtask4.html" target="_blank" class="link">Midterm Task 4: HTML Forms</a>
</div>

<div class="lt">
<h3>Lab Task 5:</h3>
<p>Applied styling using both inline and internal CSS. This task helped me understand how to design webpages and control layout, colors, and fonts.</p>
<a href="MIDTERMS TASKS/portfolio/labtask5.html" target="_blank" class="link">Midterm Task 5: Using Inline and Internal CSS</a>
</div>

<div class="lt">
<h3>Lab Task 6:</h3>
<p>Explored different display properties in CSS to control how elements appear on a webpage. This improved my understanding of layout and element positioning.</p>
<a href="MIDTERMS TASKS/portfolio/labtask6.html" target="_blank" class="link">Midterm Task 6: Using Display Property (Block Level, Inline-Block, Inline) </a>
</div>

<div class="lt">
<h3>Lab Task 7:</h3>
<p>Explored CSS and HTML skills for designing responsive webpage layouts, element positioning, and modern visual styling techniques.</p>
<a href="MIDTERMS TASKS/portfolio/labtask7.html" target="_blank" class="link">Midterm Final Task 7: GitHub Portfolio</a>
</div>

<h2 style="text-align: center; color: #FF69B4; margin-bottom: 20px;">📚 Finals</h2>

<div class="lt">
<h3>Lab Task 1:</h3>
<p>Applied Flexbox layout techniques for creating responsive webpage designs with multiple breakpoints, implementing desktop, tablet, and mobile displays while maintaining consistent color schemes and modern visual styling.</p>
<a href="MIDTERMS TASKS/portfolio/labtaskf1.html" target="_blank" class="link">Finals Task 1:Creating Responsive Layout using Flex Display Property</a>
</div>
</div>
<div class="topics" id="Contacts">
  <h2>💬 Contact Me</h2>
  
  <div class="contact-container">
    <div class="contact-card email-card">
      <div class="contact-icon">📧</div>
      <div class="contact-info">
        <h3>Email</h3>
        <a href="mailto:fjdelfina0892@iskwela.psau.edu.ph" target="_blank" class="contact-link">fjdelfina0892@iskwela.psau.edu.ph</a>
      </div>
    </div>
    <div class="contact-card phone-card">
      <div class="contact-icon">📞</div>
      <div class="contact-info">
        <h3>Phone</h3>
        <p class="phone-number">0926 930 0072</p>
      </div>
    </div>
    <div class="contact-card fb-card">
      <div class="contact-icon">ⓕ</div>
      <div class="contact-info">
        <h3>Facebook</h3>
        <a href="https://www.facebook.com/chin.delfina/" target="_blank" class="contact-link">Chin Delfina</a>
      </div>
    </div>
    <div class="contact-card location-card">
      <div class="contact-icon">📍</div>
      <div class="contact-info">
        <h3>Location</h3>
        <p>Magalang, Pampanga, Philippines</p>
      </div>
    </div>
</div>
  <div class="contact-cta">
  <p>Explore my WS101 journey! More exciting projects coming soon! 🚀📚</p>
  </div>
</div>
<button class="back2top"><a href="#top"><b>↑</b></a></button>
<footer>
  <p>© 2026 Francine Delfina | WS101 Portfolio</p>
</footer>
</body>
</html>
