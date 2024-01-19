<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <!-- Add this in the head section of your HTML file -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css" integrity="sha384-l56Yi1QqZjKsTdymGBA0mOyxqoPkGyQ2vJ9+ZnGap3QvqR5e0vKDOh4u4kYhp4J0" crossorigin="anonymous">
    <style>
    
body {
  font-family: 'Arial', sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

nav {
  background-color: #5790AB;
  font-size: 15px;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  text-align: right;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-weight: bold;
}

li a:hover {
  background-color: gray;
}

header {
  background-color: #5790AB;
  color: #fff;
  text-align: center;
  padding: 1em;
}



section {
  margin: 2em;
}

h1 {
  color: #333;
  font-size: 40px;
}

}

p {
  line-height: 1.6;
}

button{
  border-radius: 7px;
}
#about {
  position: relative;
  background-color: #f4f4f4;
  padding: 40px;
}

#about::before {
  content: '';
  position: absolute;
  top: 0;
  left: 50%;
  width: 0;
  height: 0;
  border-left: 20px solid transparent;
  border-right: 20px solid transparent;
  border-bottom: 20px solid #f4f4f4;
  transform: translateX(-50%);
}

#about::after {
  content: '';
  position: absolute;
  top: 0;
  right: 50%;
  width: 0;
  height: 0;
  border-left: 20px solid transparent;
  border-right: 20px solid transparent;
  border-bottom: 20px solid #f4f4f4;
  transform: translateX(50%);
}

#about-background {
  position: absolute;
  top: 10%;
  right: 10%;
  width: 110px;
  height: 110px;
  background-color: #5790AB;
  border-radius: 30%;
}
#about-background2 {
  position: absolute;
  top: 20px;
  right: 20px;
  width: 80px;
  height: 80px;
  background-color: darkgray;
  border-radius: 30%;
  border: 6px solid #f4f4f4;
}
.more-button {
  display: inline-block;
  padding: 15px 20px;
  background-color: #5790AB;
  color: #fff;
  text-decoration: none;
  border-radius: 15px;
  transition: background-color 0.3s ease;
  box-shadow: 2px 2px lightgrey;
}

.more-button:hover {
  background-color: white;
  border: 2px solid #5790AB;
  color: #5790AB;
  
}
.project {
  border: 1px solid #ccc;
  padding: 15px;
  margin-bottom: 20px;
}

.project h3 {
  color: #333;
}

.project p {
  color: #555;
}

.project a {
  display: inline-block;
  padding: 10px;
  margin-top: 10px;
  background-color: #444;
  color: white;
  text-decoration: none;
}

.project {
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s;
  border-top: 10px solid #5790AB;
  border-bottom: 10px solid #5790AB;
}

.project:hover {
  transform: scale(1.05);
  border-top: 10px solid #5790AB;
  border-bottom: 10px solid #5790AB;
}

.project h3 {
  color: #5790AB;
}

.project p {
  color: #555;
}

.project a {
  display: inline-block;
  padding: 12px 20px;
  margin-top: 10px;
  background-color: #5790AB;
  color: white;
  text-decoration: none;
  border-radius: 5px;
  transition: background-color 0.3s;
}

.project a:hover {
  background-color: white;
  border: 2px solid #5790AB;
  color: #5790AB;
}
#submit{
  background-color: darkgray;
  border: 1px solid #ddd;
  padding: 1em 177px;
  margin-bottom: 1em;
  display: flex;
  align-items: center;
  transition: transform 0.3s ease-in-out;
  color: white;
  font-size: 15px;
}

#submit:hover {
  transform: scale(1.05);
  background-color: none;
  
}

 .services-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
}

.services {
  background-color: #f4f4f4;
  padding: 20px;
  border-radius: 8px;
  border: 1px solid #5790AB;
  border: 1px solid #ddd;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease-in-out;
}
.services h3{
  color: #5790AB;
}

.services:hover {
  transform: scale(1.05);
  border: 2px solid #5790AB;
}


.contact-item {
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  padding: 1em;
  margin-bottom: 1em;
  display: flex;
  align-items: center;
  transition: transform 0.3s ease-in-out;
  border-bottom: 5px solid #5790AB;
  border-right: 5px solid #5790AB;
}

.contact-item:hover {
  transform: scale(1.05);
  background-color: none;
  border-right: 5px solid #5790AB;
  border-bottom: 5px solid #5790AB;
}

.fancy-contact {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

.fancy-contact i {
  font-size: 36px;
  color: #3498db;
  margin-right: 20px;
}

.contact-details {
  flex-grow: 1;
}

.contact-details p {
  margin: 0;
  font-weight: bold;
  color: #333;
}

.contact-details a {
  color: #3498db;
  text-decoration: none;
}

.contact-details a:hover {
  text-decoration: underline;
}

.contact-item p {
  margin: 0;
  font-weight: bold;
}

.contact-item a {
  color: #333;
  text-decoration: none;
}

.contact-item a:hover {
  text-decoration: underline;
}

#feedback {
  margin-top: 2em;
}

form {
  max-width: 400px;
  margin: auto;
}

label {
  display: block;
  margin-bottom: 0.5em;
}

textarea {
  width: 100%;
  padding: 0.5em;
  margin-bottom: 1em;
  border-radius: 5px;
}

button {
  background-color: #333;
  color: #fff;
  padding: 7px 7px;
  border: none;
  cursor: pointer;
}

button:hover {
  background-color: #555;
}

#feedback {
  background-color: #f5f5f5;
  padding: 40px 20px;
  text-align: left;
}

.feedback-card {
  background-color: #fff;
  border: 2px solid #5790AB;
  border-radius: 8px;
  padding: 20px;
  margin-bottom: 20px;
  transition: transform 0.3s;
}

.feedback-card:hover {
  transform: scale(1.02);
}

.feedback-card p {
  color: #333;
  text-align: center;
}

.feedback-card span {
  display: block;
  color: #777;
  margin-top: 15px;
  font-style: italic;
}

.feedback-form {
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 20px;
  margin-top: 20px;
  box-shadow: 0 0 8px rgba(0, 0, 0, 0.1);
}

.feedback-form h3 {
  color: #333;
}

.feedback-form label {
  display: block;
  margin-top: 15px;
  color: #555;
}

.feedback-form textarea,
.feedback-form input {
  width: 100%;
  padding: 10px;
  margin-top: 5px;
  margin-bottom: 15px;
  box-sizing: border-box;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.feedback-form button {
  background-color: #5790AB;
  color: white;
  padding: 10px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.feedback-form button:hover {
  background-color: white;
  border: 2px solid #5790AB;
  color: #5790AB;
}

ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  text-align: center;
}

li {
  display: inline;
  margin: 0 10px;
}

a {
  text-decoration: none;
  color: white;
}

section {
  padding: 20px;
}

footer {
  background-color: #5790AB;
  color: white;
  text-align: center;
  padding: 10px;
}

form {
  display: grid;
  grid-gap: 10px;
  max-width: 400px;
  margin: auto;
}

button {
  background-color: #444;
  color: white;
  padding: 10px;
  cursor: pointer;
  border: none;
}

h2{
  color: #5790AB;
  font-size: 35px;
  line-height: 0.1;
  font-style: italic;
}
h4{
  font-size: 25px;
  line-height: 0.1;
}
#back-to-top {
  display: none;
  position: fixed;
  bottom: 50px;
  right: 20px;
  background-color: #333;
  color: #fff;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  opacity: 0.7;
}

    </style>
    <title>Your Name - Portfolio</title>
</head>
<body>
    <nav>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
            <li><a href="#feedback">Feedback</a></li>
        </ul>
    </nav>

    <section id="about">
      <h1>About Me?</h1>
      <div id="about-background"></div>
      <div id="about-background2"></div><br>
      <h4>Hi! I'm</h4>
      <h2>Jake clint Ballon.</h2>
      <p>
        I am a passionate web developer with a strong foundation in front-end and back-end technologies.
        My journey in web development started with a curiosity for creating interactive and user-friendly websites.
        I love to explore new technologies and apply them to solve real-world problems.
      </p>
      <p>
        In addition to my technical skills, I am a creative thinker and a team player. I enjoy collaborating with others
        to bring ideas to life and contribute to innovative projects.
      </p>
      <p> I am really looking forward to work and provide you with the service that I offer.</p>
<br>
      
      <a href="#contact" class="more-button">Want to know more about me?</a>
    </section>
  
    <section id="projects">
    <h1>Projects >></h1>
    <h3>
      Welcome to my portfolio! Here's a glimpse of some projects I've worked on.</h3> 
    <p>Each project reflects my passion
      for creating innovative solutions and my dedication to delivering high-quality results.</p>
  
    <div class="project">
      <h3>Web Developing</h3>
      <p>Description of Project 1. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
      <a href="#" target="_blank">View Project</a>
    </div>
  
    <div class="project">
      <h3>Photography</h3>
      <p>Description of Project 2. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
      <a href="#" target="_blank">View Project</a>
    </div>
    
    <div class="project">
      <h3>Graphic Designing</h3>
      <p>Description of Project 3. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
      <a href="#" target="_blank">View Project</a>
    </div>
    
    <div class="project">
      <h3>Software Developing</h3>
      <p>Description of Project 4. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
      <a href="#" target="_blank">View Project</a>
    </div>
    <center>
  <button type="submit" id="submit">View more</button>
  </section>
  
  <section id="services">
    <h1>Services ✓</h1>
    <h3>Explore our services designed with you in mind. From tailored solutions to seamless experiences, we offer a range of offerings to meet your needs.</h3>
    <p>Discover how our expertise can elevate your projects and initiatives. Your goals are our focus, and we're here to provide the services that drive success.</p>
    <div class="services-grid">
    <div class="services">
    <h3>Portfolio Website ✓</h3>
    <p>Developed a personal portfolio website to showcase skills, projects, and contact information.</p>
    </div>
    <div class="services">
    <h3>E-commerce Platform ✓</h3>
    <p>Contributed to the development of an e-commerce platform with features such as product listings, cart, and checkout.</p>
    </div>
    <div class="services">
      <h3>Blog Application ✓</h3>
      <p>Built a blog application allowing users to create, edit, and delete blog posts with a user-friendly interface.</p>
    </div>
    <div class="services">
      <h3>Photography ✓</h3>
      <p>Capturing every moments, emotions, and stories through visual imagery with a very high quality images.</p>
    </div>
    <div class="services">
      <h3>Web Developing ✓</h3>
      <p>Web development is the creation and maintenance of websites, involving coding with languages like HTML, CSS, and JavaScript for functionality and design.</p>
    </div>
    <div class="services">
      <h3>Graphic Designing ✓</h3>
      <p>Graphic design is a creative and visual communication discipline that involves combining images, text, and other elements to convey a message or information.</p>
    </div>
  
  </section>


    <section id="contact">
      <h1>Contacts 📞</h1>
      <h3>Whether you have questions, feedback, or just want to say hello, we're here to hear from you</h3>
      <p>Feel free to reach out, and we'll get back to you as soon as possible. Your communication matters to us, and we look forward to connecting with you!</p>
      <div class="contact-item fancy-contact">
        <i class="fas fa-envelope"></i>
        <div class="contact-details">
          <p>Email Address</p>
          <a href="mailto:your.email@example.com">your.email@example.com</a>
          
        </div>
      </div>
      <div class="contact-item fancy-contact">
        <i class="fas fa-phone"></i>
        <div class="contact-details">
          <p>Phone Number</p>
          <p>(+63) 1234-567-8901</p>
        </div>
      </div>
      <div class="contact-item fancy-contact">
        <i class="fab fa-facebook"></i>
        <div class="contact-details">
          <p>Facebook Account</p>
          <a href="https://www.facebook.com/yourprofile" target="_blank">Your Facebook Profile</a>
        </div>
      </div>
      <div class="contact-item fancy-contact">
        <i class="fab fa-twitter"></i>
        <div class="contact-details">
          <p>Twitter Account</p>
          <a href="https://twitter.com/yourhandle" target="_blank">Your Twitter Profile</a>
        </div>
      </div>
    </section>
    
    <section id="feedback">
      <h1>Feedbacks 💬</h1>
      <p>Here are some of the feedbacks of some of our satisfied customers!</p>
    
      <div class="feedback-card">
        <p>"Your work is amazing! I love the attention to detail."</p>
        <span>- Happy Client</span>
      </div>
    
      <div class="feedback-card">
        <p>"Exceptional skills and timely delivery. Will definitely work again!"</p>
        <span>- Satisfied Customer</span>
      </div>
    
      <div class="feedback-form">
        <h3>Leave Your Feedback</h3>
        <p>Please do you send us some feedback regarding with your experience with our service!</p>
        <form id="user-feedback-form">
          <label for="feedback-message">Your Message:</label>
          <textarea id="feedback-message" name="feedback-message" required placeholder="Type your message here..."></textarea>
    
          <label for="user-name">Your Name:</label>
          <input type="text" id="user-name" name="user-name" required placeholder="Enter your name.">
    
          <button type="submit">Submit Feedback</button>
        </form>
      </div>
    </section>
    <button id="back-to-top" onclick="scrollToTop()">Back to Top</button>

    
    <footer>
      <p>&copy; 2024 My Portfolio. All rights reserved.</p>
    </footer>
    
    <script>
      // JavaScript function to scroll back to the top
      function scrollToTop() {
        document.body.scrollTop = 0; // For Safari
        document.documentElement.scrollTop = 0; // For Chrome, Firefox, IE, and Opera
      }
    
      // Show/hide the button based on scroll position
      window.onscroll = function() {
        showHideButton();
      };
    
      function showHideButton() {
        var button = document.getElementById("back-to-top");
        if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
          button.style.display = "block";
        } else {
          button.style.display = "none";
        }
      }
    </script>
</body>
</html>
