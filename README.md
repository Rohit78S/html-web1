<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Interactive Profile</title>
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-image: url('https://i.pinimg.com/originals/67/48/5a/67485aa4418c9f5980590ca090553050.gif');
      background-size: cover;
      background-repeat: no-repeat;
      background-attachment: fixed;
    }

    h2, h5 {
      text-align: center;
      color: white;
      text-shadow: 2px 2px 4px #000;
      margin: 5px;
    }

    h2 {
      font-size: 8vw;
      color: black;
    }

    h5 {
      font-size: 4vw;
      margin-top: -10px;
    }

    .profile-image {
      display: block;
      margin: 20px auto;
      width: 40vw;
      max-width: 180px;
      height: auto;
      border-radius: 50%;
      border: 4px solid white;
      box-shadow: 0 0 15px rgba(0,0,0,0.5);
      transition: transform 0.3s ease;
    }

    .profile-image:hover {
      transform: scale(1.05);
    }

    .nav {
      text-align: center;
      margin-top: 30px;
    }

    .nav h3 {
      display: inline-block;
      margin: 0 20px;
      color: black;
      cursor: pointer;
      transition: transform 0.3s ease, color 0.3s ease;
      animation: floatIn 2s ease forwards;
      font-size: 20px;
    }

    .nav h3:hover {
      transform: scale(1.2);
      color: darkblue;
    }

    .info-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      padding: 20px;
    }

    .info-box {
      width: 90%;
      max-width: 350px;
      background-color: rgba(255, 255, 255, 0.85);
      padding: 20px;
      border-radius: 15px;
      animation: slideIn 2s ease-out;
    }

    .info-box h4 {
      color: darkblue;
      font-size: 20px;
    }

    .info-box ul {
      padding-left: 20px;
    }

    .info-box li, .info-box p {
      color: black;
      font-size: 16px;
      line-height: 1.5;
    }

    .social-icons {
      text-align: center;
      margin-top: 30px;
    }

    .social-icons a {
      margin: 0 10px;
      display: inline-block;
    }

    .social-icons img {
      width: 35px;
      height: 35px;
      border-radius: 8px;
      transition: transform 0.3s;
    }

    .social-icons img:hover {
      transform: scale(1.2);
    }

    .gif-container {
      text-align: center;
      margin-top: 30px;
    }

    .gif-container img {
      width: 90%;
      max-width: 600px;
      border-radius: 20px;
    }

    #demo {
      color: white;
      font-size: 16px;
      margin-top: 10px;
      text-shadow: 1px 1px 2px #000;
    }

    .click-zone {
      position: absolute;
      z-index: 10;
      cursor: pointer;
    }

    .click-zone:hover {
      outline: 2px dashed rgba(255, 255, 255, 0.6);
    }

    @keyframes slideIn {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes floatIn {
      0% { opacity: 0; transform: translateY(-20px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    @media (max-width: 600px) {
      .nav h3 {
        display: block;
        margin: 10px 0;
      }

      .info-box {
        width: 100%;
        padding: 15px;
      }

      .profile-image {
        width: 60vw;
      }

      .gif-container img {
        width: 100%;
      }
      
    }
  </style>

  <script>
    const defaultBackground = "https://i.pinimg.com/originals/67/48/5a/67485aa4418c9f5980590ca090553050.gif";

    function changeBackground(url) {
      document.body.style.backgroundImage = `url('${url}')`;
      alert("The background image will change!");
    }

    function resetBackground() {
      document.body.style.backgroundImage = `url('${defaultBackground}')`;
      alert("Background reset to default!");
    }

    
  </script>
</head>

<body>
  <h2><i><b>HEY WELCOME</b></i></h2>
  <h5>Hey, I'm so happy you visited this website :)</h5>

  <div style="text-align: center; margin-top: 10px;">
    <button onclick="resetBackground()" style="padding: 10px 20px; font-size: 16px; border-radius: 8px; background-color: black; color: white; cursor: pointer;">
      Reset Background
    </button>
  </div>

 
    <img class="profile-image" src="https://uploads.onecompiler.io/43c8gtkh3/43rzxnhhb/profile.jpg" alt="Profile">
  

  <div class="nav">
    <h3>About Me</h3>
    <h3>Skills</h3>
  </div>

  <div class="info-container">
    <div class="info-box">
      <h4>About Me</h4>
      <p>Hi! I’m a Computer Science (Data Science) student passionate about web development, creative design, and problem-solving. I enjoy building clean, user-friendly interfaces and exploring how code can bring ideas to life. Currently learning full-stack development and working on personal projects to sharpen my skills.</p>
    </div>

    <div class="info-box">
      <h4>Skills</h4>
      <ul>
        <li>2nd year student</li>
        <li>Learning HTML</li>
        <li>Hands-on experience in HTML/CSS for responsive personal projects</li>
        <li>Skilled in user-friendly web design and clean layouts</li>
      </ul>
    </div>
  </div>

<div class="social-icons">
    <a href="https://www.instagram.com/rohityamauchi?igsh=MXdkd2NjZXRhOXcxaA==" target="_blank">
      <img src="https://www.transparentpng.com/thumb/logo-instagram/mrG45j-instagram-black-logo-free-download.png" alt="Instagram">
    </a>
    <a href="https://youtube.com/@rohityamauchi?si=8a81kYOLX0zS5YWu" target="_blank">
      <img src="https://www.transparentpng.com/thumb/youtube-icon/WoFzJU-youtube-symbol-svg-png-icon-free-download.png" alt="YouTube">
    </a>
    <a href="https://x.com/RohitYamauchi?s=09" target="_blank">
      <img src="https://img.freepik.com/free-vector/new-2023-twitter-logo-x-icon-design_1017-45418.jpg" alt="Twitter">
    </a>
    <a href="https://pin.it/5KutIk7P6" target="_blank">
      <img src="https://www.transparentpng.com/thumb/pinterest/logos-pinterest-icon-png-8.png" alt="Pinterest">
    </a>
  </div>


  <div class="click-zone" style="top: 16px; left: 6px; width: 196px; height: 144px;" onclick="changeBackground('https://uploads.onecompiler.io/43c8gtkh3/43rb8vygb/download%20(6).jpeg')"></div>
  <div class="click-zone" style="top: 10px; left: 619px; width: 273px; height: 233px;" onclick="changeBackground('https://i.pinimg.com/736x/d3/6e/45/d36e45153f2547f2ffb28612bac712c3.jpg')"></div>
  <div class="click-zone" style="top: 228px; left: 17px; width: 281px; height: 136px;" onclick="changeBackground('https://i.pinimg.com/1200x/6c/07/33/6c073337962113cfc88c43c41837f2a3.jpg')"></div>
  <div class="click-zone" style="top: 273px; left: 589px; width: 396px; height: 102px;" onclick="changeBackground('https://i.pinimg.com/1200x/66/67/2d/66672decb417ea948bfa10cef0bc68c5.jpg')"></div>



  <div class="gif-container">
    <img src="https://i.pinimg.com/originals/d8/ed/36/d8ed366ea4c2f96eb2013dd5022d5da7.gif" alt="anime gif">
  </div>






<footer style="background-color: #222; color: #fff; padding: 20px; text-align: center;
               font-family: 'Brush Script MT', cursive; font-size: 40px;
               box-shadow: 0 -4px 10px rgba(0, 0, 0, 0.6);">
  <p style="text-shadow: 2px 2px 4px rgba(40, 38, 38, 0.244);">
    Designed and coded by 
    <span style="color: red; font-weight: bold;">Rohit</span>
  </p>
</footer>


</body>
</html>
