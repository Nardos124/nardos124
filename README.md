<p align="center">
  <img src="https://media.giphy.com/media/3oEjI6SIIHBdRxXI40/giphy.gif" width="120"/>
</p>

<h1 align="center">
  Hi 👋, I'm <strong>Nardos Behailu</strong>
</h1>

<h3 align="center">
  <em>
    <span id="typing"></span>
  </em>
</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/your-linkedin" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://t.me/your-telegram" target="_blank">
    <img src="https://img.shields.io/badge/Telegram-0088cc?style=for-the-badge&logo=telegram&logoColor=white"/>
  </a>
  <a href="mailto:your.email@example.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
</p>

---

## 🌐 Skills & Technologies

<p align="center">
  ![HTML5](https://img.shields.io/badge/HTML5-90%25-orange?style=for-the-badge)
  ![CSS3](https://img.shields.io/badge/CSS3-85%25-blue?style=for-the-badge)
  ![JavaScript](https://img.shields.io/badge/JavaScript-90%25-yellow?style=for-the-badge)
  ![React](https://img.shields.io/badge/React-80%25-61DAFB?style=for-the-badge&logo=react&logoColor=black)
  ![Node.js](https://img.shields.io/badge/Node.js-75%25-green?style=for-the-badge&logo=node.js&logoColor=white)
  ![Cybersecurity](https://img.shields.io/badge/Cybersecurity-70%25-red?style=for-the-badge)
  ![IT Technician](https://img.shields.io/badge/IT%20Technician-80%25-blue?style=for-the-badge)
</p>

---

## ⚡ Fun / Animated Section

<p align="center">
  <img src="https://media.giphy.com/media/l0Exk8EUzSLsrErEQ/giphy.gif" width="300"/>
</p>

---

<!-- Typing Animation Script -->
<script>
const messages = ["Full-Stack Developer", "Cybersecurity Enthusiast", "IT Technician"];
let i = 0, j = 0;
let currentMessage = "";
let isDeleting = false;
const speed = 100;

function typeEffect() {
  const typingElement = document.getElementById("typing");
  if (!typingElement) return;

  if (!isDeleting && j <= messages[i].length) {
    currentMessage = messages[i].substring(0, j++);
    typingElement.innerHTML = currentMessage;
  } else if (isDeleting && j >= 0) {
    currentMessage = messages[i].substring(0, j--);
    typingElement.innerHTML = currentMessage;
  }

  if (j === messages[i].length) {
    isDeleting = true;
    setTimeout(typeEffect, 1000);
  } else if (j === 0 && isDeleting) {
    isDeleting = false;
    i = (i + 1) % messages.length;
  }
  setTimeout(typeEffect, speed);
}

typeEffect();
</script>
