

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ziad Profile</title>

<style>
  body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #0f0c29;
    color: white;
    transition: 0.5s;
    text-align: center;
  }

  .container {
    padding: 50px;
  }

  h1 {
    color: #00f5ff;
  }

  .typing {
    font-size: 18px;
    margin-top: 10px;
    min-height: 25px;
  }

  .card {
    background: rgba(255,255,255,0.1);
    padding: 20px;
    margin: 20px auto;
    width: 300px;
    border-radius: 15px;
    box-shadow: 0 0 10px #00f5ff;
  }

  ul {
    list-style: none;
    padding: 0;
  }

  button {
    padding: 10px 20px;
    border: none;
    background: #00f5ff;
    color: black;
    border-radius: 10px;
    cursor: pointer;
    margin-top: 20px;
  }

  button:hover {
    background: white;
  }

  /* Light mode */
  .light {
    background: white;
    color: black;
  }

  .light .card {
    box-shadow: 0 0 10px gray;
  }
</style>

</head>

<body>

<div class="container">

  <h1>Hi, I'm Ziad 👋</h1>

  <p class="typing" id="typing"></p>

  <div class="card">
    <h2>About Me</h2>
    <p>Name: Ziad Abdu Al-Asadi</p>
    <p>Age: 22</p>
    <p>Beginner Programmer 💻</p>
    <p>Goal: Software Engineer 🚀</p>
  </div>

  <div class="card">
    <h2>Skills</h2>
    <ul>
      <li>HTML 🌐</li>
      <li>CSS 🎨</li>
      <li>JavaScript ⚡</li>
      <li>C++ ⚙️</li>
    </ul>
  </div>

  <button onclick="changeTheme()">Change Theme 🎨</button>

</div>

<script>
  // typing animation
  const text = "Beginner Developer | Learning Web Development 🚀";
  let i = 0;

  function typingEffect() {
    if (i < text.length) {
      document.getElementById("typing").innerHTML += text.charAt(i);
      i++;
      setTimeout(typingEffect, 80);
    }
  }

  typingEffect();

  // theme toggle
  function changeTheme() {
    document.body.classList.toggle("light");
  }
</script>

</body>
</html>
