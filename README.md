Create two files in your GitHub repository: `index.html` and `style.css`. Paste these in.

`index.html`

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="Jordan Williams — student, builder, and future engineer." />
    <title>Jordan Williams | Portfolio</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <header class="site-header">
      <a class="brand" href="#home">JW<span>.</span></a>

      <nav>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <main>
      <section class="hero" id="home">
        <div class="hero-copy">
          <p class="eyebrow">STUDENT • BUILDER • FUTURE ENGINEER</p>
          <h1 class="moving-title">Hi, I’m <span>Jordan</span><br />Williams.</h1>
          <p class="intro">
            I’m a 9th-grade student at Henrico High School, learning to code
            and turning new ideas into projects.
          </p>
          <a class="button" href="#about">Get to know me <span>↓</span></a>
        </div>

        <div class="hero-art">
          <div class="orbit orbit-one"></div>
          <div class="orbit orbit-two"></div>

          <div class="gif-card">
            <img
              src="https://media.tenor.com/q89NzmL_UoAAAAAM/spike-touchdown.gif"
              alt="Football player celebrating a touchdown"
            />
          </div>

          <p class="play-call">PROJECTS<br /><strong>IN MOTION</strong></p>
        </div>
      </section>

      <section class="section about" id="about">
        <p class="section-label">01 / ABOUT ME</p>

        <div class="section-content">
          <h2 class="moving-title">
            Learning, building,<br /><span>leveling up.</span>
          </h2>

          <p>
            I’m currently learning how to code and make new projects. I enjoy
            exploring how technology works and using my skills to create things
            that solve problems and make a difference.
          </p>
        </div>
      </section>

      <section class="section skills" id="skills">
        <p class="section-label">02 / SKILLS</p>

        <div class="skill-grid">
          <article>
            <span>01</span>
            <h3 class="moving-title">Engineering</h3>
            <p>I like figuring out how things work and designing smart solutions.</p>
          </article>

          <article>
            <span>02</span>
            <h3 class="moving-title">Python</h3>
            <p>I’m learning to use Python to bring my ideas to life with code.</p>
          </article>

          <article>
            <span>03</span>
            <h3 class="moving-title">Project<br />Building</h3>
            <p>I’m always working on something new and growing with every project.</p>
          </article>
        </div>
      </section>

      <section class="contact" id="contact">
        <div>
          <p class="section-label">03 / CONNECT</p>
          <h2 class="moving-title">
            Let’s make<br /><span>something great.</span>
          </h2>

          <a class="email" href="mailto:jordanpnce@gmail.com">
            jordanpnce@gmail.com <span>↗</span>
          </a>
        </div>

        <img
          class="football-mini"
          src="https://media.tenor.com/m30E-XnZxHMAAAAm/football-dancing.webp"
          alt="Animated football player dancing"
        />
      </section>
    </main>

    <footer>
      <span>© 2026 Jordan Williams</span>
      <span>HENRICO HIGH SCHOOL</span>
    </footer>
  </body>
</html>
```

`style.css`

```css
:root {
  --navy: #061a40;
  --blue: #0b3a83;
  --ink: #07142e;
  --ice: #edf5ff;
  --white: #ffffff;
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  color: var(--ink);
  background: var(--white);
  font-family: "Space Grotesk", sans-serif;
}

.site-header {
  max-width: 1200px;
  height: 82px;
  margin: auto;
  padding: 0 28px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.brand {
  color: var(--navy);
  text-decoration: none;
  font-size: 28px;
  font-weight: 700;
  letter-spacing: -2px;
}

.brand span {
  color: #2873d5;
}

nav {
  display: flex;
  gap: 26px;
}

nav a {
  color: var(--navy);
  font-size: 14px;
  font-weight: 600;
  text-decoration: none;
}

nav a:hover {
  color: #2873d5;
}

.hero {
  min-height: 610px;
  padding: 72px max(28px, calc((100vw - 1144px) / 2));
  display: grid;
  grid-template-columns: 1.08fr 0.92fr;
  gap: 40px;
  align-items: center;
  overflow: hidden;
  color: var(--white);
  background: var(--navy);
}

.eyebrow,
.section-label {
  font: 500 11px "DM Mono", monospace;
  letter-spacing: 1.4px;
}

.eyebrow {
  margin: 0 0 18px;
  color: #a9c9ff;
}

h1,
h2,
h3,
p {
  margin-top: 0;
}

.moving-title {
  letter-spacing: -0.065em;
  line-height: 0.9;
}

.hero h1 {
  margin-bottom: 27px;
  font-size: clamp(58px, 8.5vw, 105px);
}

.moving-title span {
  display: inline-block;
  color: #72a9ff;
  animation: float 3.6s ease-in-out infinite;
}

.intro {
  max-width: 520px;
  margin-bottom: 30px;
  color: #d6e5ff;
  font-size: 19px;
  line-height: 1.55;
}

.button {
  display: inline-flex;
  gap: 30px;
  align-items: center;
  padding: 14px 17px;
  color: var(--navy);
  background: var(--white);
  font-weight: 700;
  text-decoration: none;
}

.button span {
  font-size: 20px;
}

.hero-art {
  position: relative;
  height: 380px;
  display: grid;
  place-items: center;
}

.gif-card {
  z-index: 2;
  width: min(315px, 75vw);
  height: 315px;
  overflow: hidden;
  background: #0d3672;
  border: 10px solid var(--white);
  border-radius: 50%;
  box-shadow: 15px 16px 0 #2873d5;
}

.gif-card img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.orbit {
  position: absolute;
  width: 365px;
  height: 180px;
  border: 1px solid rgba(146, 190, 255, 0.5);
  border-radius: 50%;
  transform: rotate(-29deg);
}

.orbit-two {
  border-style: dashed;
  transform: rotate(45deg) scale(0.82);
  animation: spin 18s linear infinite;
}

.play-call {
  position: absolute;
  right: 0;
  bottom: 8px;
  z-index: 3;
  margin: 0;
  color: #bbd6ff;
  font: 500 11px "DM Mono", monospace;
  letter-spacing: 1px;
}

.play-call strong {
  color: white;
  font-size: 14px;
}

.section {
  max-width: 1144px;
  margin: auto;
  padding: 112px 28px;
  display: grid;
  grid-template-columns: 170px 1fr;
  gap: 30px;
}

.section-label {
  padding-top: 11px;
  color: #3067b9;
}

.section-content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 65px;
}

.section h2,
.contact h2 {
  margin-bottom: 0;
  color: var(--navy);
  font-size: clamp(42px, 5vw, 68px);
}

.section-content p {
  align-self: end;
  margin-bottom: 0;
  font-size: 19px;
  line-height: 1.6;
}

.skills {
  max-width: none;
  padding-right: max(28px, calc((100vw - 1144px) / 2));
  padding-left: max(28px, calc((100vw - 1144px) / 2));
  background: var(--ice);
}

.skill-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 18px;
}

.skill-grid article {
  min-height: 254px;
  padding: 25px;
  display: flex;
  flex-direction: column;
  background: var(--white);
  border-top: 4px solid var(--blue);
}

.skill-grid span {
  color: #3472cc;
  font: 500 11px "DM Mono", monospace;
}

.skill-grid h3 {
  margin: 35px 0 15px;
  color: var(--navy);
  font-size: 31px;
}

.skill-grid p {
  margin: 0;
  color: #4d5b74;
  line-height: 1.45;
}

.contact {
  max-width: 1144px;
  min-height: 430px;
  margin: auto;
  padding: 105px 28px 85px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 45px;
}

.contact h2 {
  margin: 14px 0 28px;
}

.email {
  color: var(--blue);
  font-size: clamp(17px, 2vw, 23px);
  font-weight: 700;
  text-underline-offset: 7px;
}

.football-mini {
  width: 160px;
  height: 160px;
  object-fit: cover;
  background: #b9d3ff;
  border: 7px solid var(--navy);
  border-radius: 50%;
}

footer {
  padding: 24px max(28px, calc((100vw - 1144px) / 2));
  display: flex;
  justify-content: space-between;
  color: #a9c9ff;
  background: var(--navy);
  font: 500 10px "DM Mono", monospace;
  letter-spacing: 1px;
}

@keyframes float {
  50% {
    transform: translateY(-8px) rotate(-1deg);
  }
}

@keyframes spin {
  to {
    transform: rotate(405deg) scale(0.82);
  }
}

@media (max-width: 720px) {
  .site-header {
    height: 68px;
  }

  .hero {
    padding-top: 58px;
    padding-bottom: 58px;
    grid-template-columns: 1fr;
  }

  .hero-art {
    height: 300px;
  }

  .orbit {
    width: 300px;
  }

  .gif-card {
    width: 240px;
    height: 240px;
  }

  .section {
    padding-top: 75px;
    padding-bottom: 75px;
    grid-template-columns: 1fr;
    gap: 8px;
  }

  .section-content,
  .skill-grid {
    grid-template-columns: 1fr;
  }

  .section-content {
    gap: 26px;
  }

  .skill-grid article {
    min-height: 200px;
  }

  .contact {
    min-height: 360px;
    padding-top: 75px;
  }

  .football-mini {
    width: 105px;
    height: 105px;
  }

  nav {
    gap: 14px;
  }

  nav a {
    font-size: 12px;
  }

  footer {
    font-size: 8px;
  }
}
```
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="Jordan Williams — student, builder, and future engineer." />
    <title>Jordan Williams | Portfolio</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <header class="site-header">
      <a class="brand" href="#home">JW<span>.</span></a>

      <nav>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <main>
      <section class="hero" id="home">
        <div class="hero-copy">
          <p class="eyebrow">STUDENT • BUILDER • FUTURE ENGINEER</p>
          <h1 class="moving-title">Hi, I’m <span>Jordan</span><br />Williams.</h1>
          <p class="intro">
            I’m a 9th-grade student at Henrico High School, learning to code
            and turning new ideas into projects.
          </p>
          <a class="button" href="#about">Get to know me <span>↓</span></a>
        </div>

        <div class="hero-art">
          <div class="orbit orbit-one"></div>
          <div class="orbit orbit-two"></div>

          <div class="gif-card">
            <img
              src="https://media.tenor.com/q89NzmL_UoAAAAAM/spike-touchdown.gif"
              alt="Football player celebrating a touchdown"
            />
          </div>

          <p class="play-call">PROJECTS<br /><strong>IN MOTION</strong></p>
        </div>
      </section>

      <section class="section about" id="about">
        <p class="section-label">01 / ABOUT ME</p>

        <div class="section-content">
          <h2 class="moving-title">
            Learning, building,<br /><span>leveling up.</span>
          </h2>

          <p>
            I’m currently learning how to code and make new projects. I enjoy
            exploring how technology works and using my skills to create things
            that solve problems and make a difference.
          </p>
        </div>
      </section>

      <section class="section skills" id="skills">
        <p class="section-label">02 / SKILLS</p>

        <div class="skill-grid">
          <article>
            <span>01</span>
            <h3 class="moving-title">Engineering</h3>
            <p>I like figuring out how things work and designing smart solutions.</p>
          </article>

          <article>
            <span>02</span>
            <h3 class="moving-title">Python</h3>
            <p>I’m learning to use Python to bring my ideas to life with code.</p>
          </article>

          <article>
            <span>03</span>
            <h3 class="moving-title">Project<br />Building</h3>
            <p>I’m always working on something new and growing with every project.</p>
          </article>
        </div>
      </section>

      <section class="contact" id="contact">
        <div>
          <p class="section-label">03 / CONNECT</p>
          <h2 class="moving-title">
            Let’s make<br /><span>something great.</span>
          </h2>

          <a class="email" href="mailto:jordanpnce@gmail.com">
            jordanpnce@gmail.com <span>↗</span>
          </a>
        </div>

        <img
          class="football-mini"
          src="https://media.tenor.com/m30E-XnZxHMAAAAm/football-dancing.webp"
          alt="Animated football player dancing"
        />
      </section>
    </main>

    <footer>
      <span>© 2026 Jordan Williams</span>
      <span>HENRICO HIGH SCHOOL</span>
    </footer>
  </body>
</html>
