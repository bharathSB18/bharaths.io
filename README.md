<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Portfolio Website</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background: url('6eb0f442-4330-4666-af0d-82d496e4290a.png') no-repeat center center fixed;
      background-size: cover;
      color: #333;
    }

    .navbar {
      background-color: #1a1a2e;
      color: white;
      padding: 15px 0;
      display: flex;
      justify-content: center;
      gap: 30px;
      font-weight: 500;
    }

    .navbar a {
      color: white;
      text-decoration: none;
      font-size: 16px;
      transition: color 0.3s;
    }

    .navbar a:hover {
      color: #00bcd4;
    }

    .section {
      display: none;
      padding: 40px 20px;
      max-width: 800px;
      margin: 40px auto;
      background: rgba(255, 255, 255, 0.85);
      border-radius: 8px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }

    .active-section {
      display: block;
    }

    .header {
      text-align: center;
      padding: 40px 20px 0 20px;
      background: rgba(255, 255, 255, 0.85);
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }

    .header img {
      width: 140px;
      height: 140px;
      object-fit: cover;
      border-radius: 50%;
      border: 4px solid #1a1a2e;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }

    .header h1 {
      margin: 20px 0 10px 0;
      font-size: 32px;
      color: #1a1a2e;
    }

    .header button {
      padding: 10px 25px;
      font-size: 15px;
      background: #1a1a2e;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background 0.3s;
    }

    .header button:hover {
      background: #00bcd4;
    }

    h2 {
      color: #1a1a2e;
    }

    ul li {
      margin-bottom: 8px;
    }
  </style>
</head>
<body>
  <div class="header">
    <img src="https://uploads.onecompiler.io/433p8kja3/43sg3nyq9/for%20portfolio.JPG" alt="Profile Image" class="profile-image" />
    <h1>BHARATH S.</h1>
    <button onclick="downloadResume()">Download Resume</button>
  </div>

  <div class="navbar">
    <a onclick="showSection('Home')">Home</a>
    <a onclick="showSection('about')">About</a>
    <a onclick="showSection('skills')">Skills</a>
    <a onclick="showSection('projects')">Projects</a>
    <a onclick="showSection('certifications')">Certifications</a>
    <a onclick="showSection('contact')">Contact</a>
  </div>

  <div id="Home" class="section active-section">
    <h2>Welcome To My Profile</h2>
    <p>Hi, I am Bharath.S A dedicated learner with a fresh perspective. Explore my projects to see my technical skills and creative problem-solving in action.</p>
  </div>

  <div id="about" class="section">
    <h2>About Me</h2>
    <p>I am a passionate Computer Science Diploma student with interests in web development and cloud technologies...</p>
  </div>

  <div id="skills" class="section">
    <h2>Skills</h2>
    <ul>
      <li>HTML5, CSS3, JavaScript</li>
      <li>Git & GitHub</li>
      <li>Responsive Web Design</li>
      <li>AWS Cloud Fundamentals</li>
      <li>Basic Python & SQL</li>
    </ul>
  </div>

  <div id="projects" class="section">
    <h2>Projects</h2>
    <h4>Personal Portfolio Website</h4>
    <p>A fully responsive portfolio site built with HTML and CSS...</p>
    <h4>Student Result Management System</h4>
    <p>A mini project using HTML, CSS, and JS to manage marks and results...</p>
  </div>

  <div id="certifications" class="section">
    <h2>Certifications</h2>
    <ul>
      <li>Basic Computer Course</li>
      <li>TATA Data Analytics Virtual Internship</li>
    </ul>
  </div>

  <div id="contact" class="section">
    <h2>Contact</h2>
    <p>Email: bharathsahadeva2005@gmail.com</p>
    <p>Phone: +91 7022558340</p>
    <p>LinkedIn: linkedin.com/in/yourprofile</p>
  </div>

  <script>
    function showSection(id) {
      const sections = document.querySelectorAll('.section');
      sections.forEach(section => section.classList.remove('active-section'));
      document.getElementById(id).classList.add('active-section');
    }

    function downloadResume() {
      window.location.href = 'resume.pdf';
    }
  </script>
</body>
</html>
