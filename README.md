<script>
function toggleTheme() {
    document.documentElement.classList.toggle('dark-mode');

    const button = document.querySelector('.theme-toggle');

    if (document.documentElement.classList.contains('dark-mode')) {
        button.innerHTML = '☀️ Light Mode';
        localStorage.setItem('theme', 'dark');
    } else {
        button.innerHTML = '🌙 Dark Mode';
        localStorage.setItem('theme', 'light');
    }
}

window.addEventListener('DOMContentLoaded', function () {
    const savedTheme = localStorage.getItem('theme');
    const button = document.querySelector('.theme-toggle');

    if (savedTheme === 'dark') {
        document.documentElement.classList.add('dark-mode');
        button.innerHTML = '☀️ Light Mode';
    }
});
</script>

<!-- Profile photo -->
<p>
  <img src="photo_2026-08-17_05-40-39.jpg"
       width="180"
       height="180"
       style="border-radius:50%; object-fit:cover;"
       alt="Mohammad Sefid">
</p>

<!-- Social links -->
<p>
  <!-- Gmail -->
  <a href="https://mail.google.com/mail/?view=cm&fs=1&to=mohammad.sefid74@gmail.com"
     target="_blank"
     rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"
         alt="Gmail">
  </a>

  <!-- LinkedIn -->
  <a href="https://www.linkedin.com/in/mohammad-sefid/"
     target="_blank"
     rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"
         alt="LinkedIn">
  </a>

  <!-- GitHub -->
  <a href="https://github.com/mohammad-sefid"
     target="_blank"
     rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"
         alt="GitHub">
  </a>
</p>
