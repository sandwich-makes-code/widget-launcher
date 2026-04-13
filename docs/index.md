<style>
  /* Light mode */
  body {
    background: #ffffff;
    color: #000000;
    font-family: "Segoe UI", sans-serif;
  }

  /* Dark mode */
  @media (prefers-color-scheme: dark) {
    body {
      background: #0d1117;
      color: #c9d1d9;
    }
  }
</style>


# Widget Launcher


<img src="icon-shortcut.ico" style="
  width: 600px;
  border-radius: 10px;
  box-shadow: 0 0 20px #0005;
">


Welcome to the official home of the Widget Launcher project.

Download from here: [Download Releases](releases.md)

UPDATE REPORT 4/12/2026 to 4/13/2026:

The Major Drop: I have added lots of pre-made widgets and they do stuff. v2.0

Spelling issue fix v1.1

<button class="theme-toggle" onclick="toggleTheme()">Toggle Theme</button>
<script>
  // Load saved theme OR default to auto (device-based)
  const saved = localStorage.getItem('theme') || 'auto';
  document.body.className = saved;

  function toggleTheme() {
    let current = document.body.className;

    // Cycle through: auto → light → dark → auto
    let next = current === 'auto' ? 'light' :
               current === 'light' ? 'dark' : 'auto';

    document.body.className = next;
    localStorage.setItem('theme', next);
  }
</script>

