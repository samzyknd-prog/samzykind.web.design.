<style>
html{
  scroll-behavior: smooth;
}
  img{
    border: 3px solid white;
}
  img{
     border-radius: 50px;
}

</style>
<style> 
h1{
  border:3px solid blue;
  padding: 20px;
  margin: 20px;
}
h1{
  color:blue;
}
p{
  color:white;
}
body{
  background-color:orange;
}
h1{
  color:blue;
}
p{
  color:white;
  padding: 2px;
  margin: 5px;
}
body{
  background-color:orange;
}
button {
  background-color: purple;
  color: yellow;
  padding: 15px 30px;
  border: 3px solid blue;
  border-radius: 50px;
  transition: 0.3s;
  box-shadow: 0 4px 8px gray;
  cursor: pointer;
  align-items: center;
}
button:hover {
    color: red;
    transform: scale(1.1);
}
button:active {
   background-color: green;
   transform: scale(1.1);
}
nav {
   background-color: black;
   padding: 12px;
   text-align: center;
}
nav a {
   color: white;
   text-decoration: none;
   margin: 3px;
   font-size: 15px;
}
nav a:hover {
    color: yellow;
}
.hero {
  text-align: center;
  background-color: white;
  width: 300px;
  margin: 30px auto;
  padding: 20px;
  border-radius: 15px;
  box-shadow: 0 5px 15px gray;
}
.hero img{
  border-radius: 50%;
  border: 4px solid white;
}
.hero h1{
   border: none;
   color: black;
}
.hero p {
   color: black;
   font-size: 18px;
}
footer {
  background-color: #333;
  color: white;
  text-align: center;
  padding: 15px;
  margin-top: 30px;
}
footer p {
   color: white;
   margin: 0;
}
h2 {
  text-align: center;
  color: black;
  padding: 20px;
  margin: 10px;
}
ul {
  width: 250px;
  margin: auto;
  color: black;
  font-size: 18px;
}
.projects{
  display: flex;
  justify-content: flex-end;
  gap: 10px;
  flex-wrap: nowrap;
  margin: 20px;
}
.project-card{
  background: white;
  width: 200px;
  padding: 20px;
  border-radius: 15px;
  box-shadow: 0 5px 15px gray;
}
.project-card:hover{
  transform: translateY(-10px);
  transition: 0.3s;
  cursor: pointer;
  box-shadow: 0 10px 20px gray;
}
.project-card h3{
  color: blue;
}
.project-card p{
  color: black;
}
.loading{
  display: black;
  margin: 30px auto 80px auto;
}
.loading{
  margin-bottom: 250px;
  margin-top: 40px;
  text-align: center;
}
.about{
    width: 80%;
    margin: 30px auto;
    text-align: center;
    color: black;
    line-height: 1.6;
}
.about p{
  color: black;
  box-shadow: 0 5px 25px gray;
}
.contact{
  background: white;
  width: 300px;
  margin: 20px auto;
  padding: 20px;
  border-radius: 15px;
  text-align: center;
  line-height: 1.6;
}

.contact p{
  color: black;
  margin: 10px 0;
}
@media (max-width: 768px) {
  .projects{
    justify-content: center;
  }
}

  .hero{
    width: 90%;
  }

  .project-card{
    width: 90%;
  }
.social{
  text-align: center;
  margin: 30px 0;
}
.social a{
  color: white;
  text-decoration: none;
  background: blue;
  padding: 10px 15px;
  margin: 5px;
  border-radius: 10px;
  display: inline-block;
}

.social a:hover{
  background: purple;
}
.cv-btn{
  display: inline-block;
  background: purple;
  color: yellow;
  padding: 15px 30px;
  border: 3px solid blue;
  border-radius: 50px;
  text-decoration: none;
  margin-top: 15px;
  box-shadow: 0 4px 8px gray;
}
.cv-btn:hover{
  background: blue;
  color: white;
}
</style>
<!DOCTYPE html>
<html>
<head>
  <title>My First website</title>
</head>
<style> 
.box {
  width: 100px;
  height: 100px;
  border-radius: 50px;
  background: orange;
  animation: moveBox 3s
infinite;
}
@keyframes moveBox {
  0% {
    transform: translateX(0);
    background: blue;
  }
  25% {
    background: red;
  }
  50% {
    transform: translateX(200px);
    background: yellow;
  }
  75% {
    transform: translateX(200px);
    background: yellow;
  }
  100% {
    transform: translateX(0);
    background: purple;
  }
}
</style>
<body>
 <nav>
  <a href="#">HOME</a>
  <a href="#about">ABOUT</a>
  <a href="#skills">SKILLS</a>
  <a href="#projects">PROJECTS</a>
  <a href="#contact">CONTACT</a>
</nav>
  <h1 onclick="changeColor()"> WELCOME TO SAMZYKIND.OG WEBSITE</h1>
  <p>"I'm Samzy Kind, a web developer learning to build amazing websites."</p>
  <p>
      I'm passionate about creating beautiful, responsive websites and learning new web technologies every day. Welcome to my portfolio! 
      Thank you for visiting my website, and I hope you enjoy exploring my work.</p>
<div class="box"></div>
  <script>
    let colors = ["red", "green","blue", "white"]
    let index = 0;
    function changeColor() {
      document.querySelector("h1").style.color = colors[index];
      index++;
      
      if (index >= colors.length) {
        index = 0;
      }
    }

  </script>
<button>CLICK ME</button>
  <div class="hero">
  <img src="Samzy.jpg" alt="Samzy" width="180"><br> 
  <h1>Hi, I'm Samzy Kind.OG </h1>
  <p id="typing"></p>
 <button onclick="contactMe()">Contact Me
 </button>
 <br></br>
<a href="Cv.pdf" download class="cv-btn">Download My CV</a>
 <script>
  function contactMe() {
  alert("Thanks for visiting my portfolio! You can contact me at:samzyknd@gmail.com +234 7076849480");}
  </script>
<div class="about">
    <h2 id="about">About Me</h2>
    <p>
        Hello! I'm Samzy Kind.OG, an aspiring web developer from Nigeria.
        I enjoy building websites with HTML and CSS, and I'm currently learning JavaScript.
        My goal is to become a professional full-stack web developer.
    </p>
</div>
<h2 id="skills">My Skills</h2>
<ul>
  <li>HTML⭐⭐⭐⭐⭐</li>
  <li>CSS⭐⭐⭐⭐⭐</li>
  <li> JAVASCRIPT⭐⭐⭐⭐⭐</li>
  </ul>
<h2 id="projects">My Project</h2>
<div class="projects">
  <div class="project-card">
  <h3>Portfolio Website</h3>
  <p>MY PERSONAL PORTFOLIO BUILT WITH HTML AND CSS.</p>
</div>
<div class="project-card">
  <h3>COMING SOON</h3>
  <p>MORE AMAZING PROJECT WILL BE ADDED HERE.</p>
</div>
</div>
</div>

 <img src="loading.JPG" alt="loading" width="100" class="loading"><br>
<h2 id="contact">Contact Me</h2>
<div class="contact">
  <p>Email: samzyknd@gmail.com</p>
  <p>Phone: +234 7076849480</p>
  <p>Location: Nigeria</p>
</div>
<h2>Follow Me</h2>
<div class="social">
  <a href="https://facebook.com">Facebook</a>
  <a href="https://instagram.com">Instagram</a>
  <a href="https://x.com">X (Twitter)</a>
  <a href="https://github.com">GitHub
  </a>
  <a href="https://tiktok.com">Tiktok</a>
</div>
</div>
<footer> 
<p> ©2026 SAMZYKIND.OG. All Right Reserved</p>
</footer>
<script>
const text = "ASPIRING WEB DEVELOPER.";
let i = 0;

function typeText() {
  if (i < text.length) {
    document.getElementById("typing").innerHTML += text.charAt(i);
    i++;
    setTimeout(typeText, 100);
  }
}

typeText();
</script>
</body>
</html>
