<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <meta name="description" content="Aleesha Fathima PK - Data Scientist Portfolio">
  <meta name="author" content="Aleesha Fathima PK">

  <title>Aleesha Fathima PK | Data Scientist</title>

  <style>
    :root {
      --bg: #f7f9fc;
      --white: #ffffff;
      --text: #172033;
      --muted: #667085;
      --primary: #4f46e5;
      --primary-dark: #3730a3;
      --border: #e5e7eb;
      --soft: #f1f5f9;
      --shadow: 0 18px 50px rgba(15, 23, 42, 0.08);
      --radius: 18px;
      --max-width: 1120px;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Inter, -apple-system, BlinkMacSystemFont, "Segoe UI",
        Roboto, Arial, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.7;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    .container {
      width: min(92%, var(--max-width));
      margin: auto;
    }

    /* ================= NAVBAR ================= */

    header {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: rgba(255, 255, 255, 0.92);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border);
    }

    nav {
      min-height: 72px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-size: 1.2rem;
      font-weight: 800;
    }

    .logo span {
      color: var(--primary);
    }

    .nav-links {
      display: flex;
      gap: 28px;
      list-style: none;
      font-size: 0.94rem;
      font-weight: 600;
      color: #475467;
    }

    .nav-links a:hover {
      color: var(--primary);
    }

    .nav-button {
      background: var(--text);
      color: white !important;
      padding: 9px 17px;
      border-radius: 10px;
    }

    /* ================= HERO ================= */

    .hero {
      min-height: calc(100vh - 72px);
      display: flex;
      align-items: center;
      padding: 80px 0;
      background:
        radial-gradient(circle at 85% 15%, rgba(79, 70, 229, 0.11), transparent 28%),
        radial-gradient(circle at 10% 80%, rgba(99, 102, 241, 0.08), transparent 25%);
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.3fr 0.7fr;
      gap: 70px;
      align-items: center;
    }

    .eyebrow {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 7px 12px;
      border: 1px solid #ddd6fe;
      background: #f5f3ff;
      color: var(--primary-dark);
      border-radius: 999px;
      font-size: 0.84rem;
      font-weight: 700;
      margin-bottom: 20px;
    }

    .eyebrow::before {
      content: "";
      width: 7px;
      height: 7px;
      background: #22c55e;
      border-radius: 50%;
    }

    .hero h1 {
      font-size: clamp(2.7rem, 6vw, 5rem);
      line-height: 1.05;
      letter-spacing: -3px;
      margin-bottom: 18px;
    }

    .hero h1 span {
      color: var(--primary);
    }

    .hero h2 {
      font-size: 1.45rem;
      color: #475467;
      margin-bottom: 20px;
    }

    .hero p {
      max-width: 670px;
      color: var(--muted);
      font-size: 1.05rem;
      margin-bottom: 30px;
    }

    .hero-buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 13px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 12px 20px;
      border-radius: 11px;
      font-weight: 700;
      border: 1px solid var(--border);
      transition: 0.2s;
    }

    .btn-primary {
      background: var(--primary);
      color: white;
      border-color: var(--primary);
    }

    .btn-primary:hover {
      background: var(--primary-dark);
      transform: translateY(-2px);
    }

    .btn-secondary {
      background: white;
    }

    .btn-secondary:hover {
      border-color: var(--primary);
      color: var(--primary);
      transform: translateY(-2px);
    }

    /* ================= PROFILE CARD ================= */

    .hero-card {
      background: var(--white);
      border: 1px solid var(--border);
      box-shadow: var(--shadow);
      border-radius: 24px;
      padding: 34px;
    }

    .profile-placeholder {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      margin: 0 auto 24px;
      background: linear-gradient(135deg, #4f46e5, #7c3aed);
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2.2rem;
      font-weight: 800;
    }

    .hero-card h3 {
      text-align: center;
      margin-bottom: 5px;
    }

    .hero-card > p {
      text-align: center;
      color: var(--muted);
      margin-bottom: 22px;
    }

    .quick-info {
      display: grid;
      gap: 12px;
    }

    .quick-info div {
      display: flex;
      justify-content: space-between;
      padding-bottom: 10px;
      border-bottom: 1px solid var(--border);
      font-size: 0.9rem;
    }

    .quick-info span {
      color: var(--muted);
    }

    /* ================= GENERAL ================= */

    section {
      padding: 95px 0;
    }

    .section-heading {
      margin-bottom: 45px;
    }

    .section-label {
      color: var(--primary);
      font-weight: 800;
      text-transform: uppercase;
      letter-spacing: 1.5px;
      font-size: 0.78rem;
      margin-bottom: 8px;
    }

    .section-heading h2 {
      font-size: 2.7rem;
      letter-spacing: -1.5px;
      margin-bottom: 10px;
    }

    .section-heading p {
      color: var(--muted);
      max-width: 680px;
    }

    /* ================= ABOUT ================= */

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 35px;
    }

    .about-card {
      background: var(--white);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 30px;
    }

    .about-card h3 {
      margin-bottom: 13px;
    }

    .about-card p {
      color: var(--muted);
    }

    .focus-list {
      list-style: none;
      display: grid;
      gap: 12px;
    }

    .focus-list li {
      padding: 13px 15px;
      background: var(--soft);
      border-radius: 10px;
      font-weight: 600;
    }

    .focus-list li::before {
      content: "✓";
      color: var(--primary);
      font-weight: 900;
      margin-right: 10px;
    }

    /* ================= SKILLS ================= */

    #skills,
    #projects,
    #certifications {
      background: white;
    }

    .skills-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 20px;
    }

    .skill-card {
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 25px;
      background: var(--white);
    }

    .skill-card h3 {
      margin-bottom: 17px;
    }

    .tags {
      display: flex;
      flex-wrap: wrap;
      gap: 9px;
    }

    .tag {
      padding: 7px 11px;
      border-radius: 8px;
      background: var(--soft);
      color: #344054;
      font-size: 0.84rem;
      font-weight: 600;
      border: 1px solid #e7ebf0;
    }

    /* ================= EXPERIENCE ================= */

    .timeline {
      max-width: 850px;
      margin: auto;
    }

    .timeline-item {
      position: relative;
      padding: 0 0 35px 35px;
      border-left: 2px solid #ddd6fe;
    }

    .timeline-item::before {
      content: "";
      position: absolute;
      left: -7px;
      top: 3px;
      width: 12px;
      height: 12px;
      background: var(--primary);
      border-radius: 50%;
      box-shadow: 0 0 0 5px #ede9fe;
    }

    .timeline-date {
      color: var(--primary);
      font-size: 0.82rem;
      font-weight: 800;
    }

    .timeline h3 {
      font-size: 1.3rem;
      margin-top: 5px;
    }

    .timeline h4 {
      color: var(--muted);
      font-weight: 600;
      margin-bottom: 15px;
    }

    .timeline ul {
      padding-left: 19px;
      color: var(--muted);
    }

    .timeline li {
      margin-bottom: 7px;
    }

    /* ================= PROJECTS ================= */

    .projects-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 25px;
    }

    .project-card {
      background: white;
      border: 1px solid var(--border);
      border-radius: var(--radius);
      overflow: hidden;
      transition: 0.25s;
    }

    .project-card:hover {
      transform: translateY(-5px);
      box-shadow: var(--shadow);
    }

    .project-top {
      height: 145px;
      display: flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(135deg, #eef2ff, #f5f3ff);
      font-size: 3.5rem;
    }

    .project-content {
      padding: 27px;
    }

    .project-content h3 {
      margin-bottom: 10px;
    }

    .project-content p {
      color: var(--muted);
      font-size: 0.93rem;
      margin-bottom: 18px;
    }

    .project-tech {
      display: flex;
      flex-wrap: wrap;
      gap: 7px;
    }

    .project-tech span {
      color: var(--primary-dark);
      background: #eef2ff;
      padding: 5px 9px;
      border-radius: 7px;
      font-size: 0.77rem;
      font-weight: 700;
    }

    /* ================= EDUCATION ================= */

    .education-card {
      max-width: 850px;
      margin: auto;
      background: white;
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 30px;
      display: flex;
      justify-content: space-between;
      gap: 25px;
    }

    .education-card p {
      color: var(--muted);
    }

    .cgpa {
      min-width: 120px;
      text-align: center;
      background: #f5f3ff;
      border-radius: 13px;
      padding: 14px;
      height: fit-content;
    }

    .cgpa strong {
      display: block;
      color: var(--primary);
      font-size: 1.3rem;
    }

    .cgpa span {
      font-size: 0.78rem;
      color: var(--muted);
    }

    /* ================= CERTIFICATIONS ================= */

    .cert-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 17px;
    }

    .cert-card {
      border: 1px solid var(--border);
      border-radius: 13px;
      padding: 20px;
      background: var(--white);
    }

    .cert-card strong {
      display: block;
      margin-bottom: 4px;
    }

    .cert-card span {
      color: var(--muted);
      font-size: 0.88rem;
    }

    /* ================= CONTACT ================= */

    .contact-box {
      background: #111827;
      color: white;
      border-radius: 24px;
      padding: 55px;
      text-align: center;
    }

    .contact-box h2 {
      font-size: 3rem;
      margin-bottom: 12px;
    }

    .contact-box p {
      color: #cbd5e1;
      max-width: 620px;
      margin: 0 auto 28px;
    }

    .contact-links {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 12px;
    }

    .contact-link {
      padding: 11px 17px;
      border: 1px solid #374151;
      border-radius: 10px;
      color: white;
      font-weight: 600;
    }

    .contact-link:hover {
      background: white;
      color: #111827;
    }

    /* ================= FOOTER ================= */

    footer {
      padding: 30px 0;
      text-align: center;
      color: var(--muted);
      font-size: 0.88rem;
    }

    /* ================= MOBILE ================= */

    @media (max-width: 850px) {

      .nav-links {
        display: none;
      }

      .hero-grid,
      .about-grid,
      .skills-grid,
      .projects-grid,
      .cert-grid {
        grid-template-columns: 1fr;
      }

      .hero {
        padding: 65px 0;
      }

      .hero-grid {
        gap: 40px;
      }

      .education-card {
        flex-direction: column;
      }

      .cgpa {
        width: 130px;
      }
    }

    @media (max-width: 500px) {

      section {
        padding: 70px 0;
      }

      .hero-buttons {
        flex-direction: column;
      }

      .btn {
        width: 100%;
      }

      .contact-box {
        padding: 35px 22px;
      }

      .contact-box h2 {
        font-size: 2.2rem;
      }
    }
  </style>
</head>

<body>

  <!-- ================= NAVIGATION ================= -->

  <header>
    <div class="container">

      <nav>

        <a href="#home" class="logo">
          Aleesha<span>.</span>
        </a>

        <ul class="nav-links">

          <li>
            <a href="#about">About</a>
          </li>

          <li>
            <a href="#skills">Skills</a>
          </li>

          <li>
            <a href="#experience">Experience</a>
          </li>

          <li>
            <a href="#projects">Projects</a>
          </li>

          <li>
            <a href="#education">Education</a>
          </li>

          <li>
            <a href="#contact" class="nav-button">
              Contact
            </a>
          </li>

        </ul>

      </nav>

    </div>
  </header>


  <!-- ================= HERO ================= -->

  <main id="home">

    <section class="hero">

      <div class="container hero-grid">

        <div>

          <div class="eyebrow">
            Data Science Portfolio
          </div>

          <h1>
            Hi, I'm <span>Aleesha</span>.
          </h1>

          <h2>
            Data Scientist | Machine Learning | Data Analytics
          </h2>

          <p>
            I work with Python, SQL, Machine Learning and Data Visualization
            to analyse data, build predictive models and create meaningful
            data-driven solutions.
          </p>

          <div class="hero-buttons">

            <a href="#projects" class="btn btn-primary">
              View My Projects
            </a>

            <a href="#contact" class="btn btn-secondary">
              Get In Touch
            </a>

          </div>

        </div>


        <div class="hero-card">

          <div class="profile-placeholder">
            AF
          </div>

          <h3>
            Aleesha Fathima PK
          </h3>

          <p>
            Data Scientist
          </p>

          <div class="quick-info">

            <div>
              <span>Location</span>
              <strong>Calicut, Kerala</strong>
            </div>

            <div>
              <span>Education</span>
              <strong>B.Tech AI & DS</strong>
            </div>

            <div>
              <span>CGPA</span>
              <strong>8.0 / 10</strong>
            </div>

            <div>
              <span>Focus</span>
              <strong>Data Science</strong>
            </div>

          </div>

        </div>

      </div>

    </section>


    <!-- ================= ABOUT ================= -->

    <section id="about">

      <div class="container">

        <div class="section-heading">

          <div class="section-label">
            About Me
          </div>

          <h2>
            Turning data into meaningful insights.
          </h2>

          <p>
            A focused introduction to my background, technical interests
            and areas of work.
          </p>

        </div>


        <div class="about-grid">

          <div class="about-card">

            <h3>
              Who I Am
            </h3>

            <p>
              I'm a Data Scientist with expertise in Python, SQL, Machine
              Learning, Data Analysis and Data Visualization. I have
              experience working with data cleaning, exploratory data
              analysis, statistical analysis, predictive modelling and
              dashboard development.
            </p>

            <br>

            <p>
              I enjoy transforming datasets into actionable insights and
              developing data-driven solutions using modern analytics and
              machine learning techniques.
            </p>

          </div>


          <div class="about-card">

            <h3>
              What I Work With
            </h3>

            <ul class="focus-list">

              <li>
                Data Analysis & Cleaning
              </li>

              <li>
                Exploratory Data Analysis
              </li>

              <li>
                Machine Learning
              </li>

              <li>
                Predictive Modelling
              </li>

              <li>
                Power BI & Data Visualization
              </li>

              <li>
                SQL & MySQL
              </li>

            </ul>

          </div>

        </div>

      </div>

    </section>


    <!-- ================= SKILLS ================= -->

    <section id="skills">

      <div class="container">

        <div class="section-heading">

          <div class="section-label">
            Technical Skills
          </div>

          <h2>
            Tools & technologies
          </h2>

          <p>
            Technologies and concepts I use across data science and analytics.
          </p>

        </div>


        <div class="skills-grid">

          <div class="skill-card">

            <h3>
              Programming & Database
            </h3>

            <div class="tags">

              <span class="tag">Python</span>
              <span class="tag">SQL</span>
              <span class="tag">MySQL</span>

            </div>

          </div>


          <div class="skill-card">

            <h3>
              Data Science & Analytics
            </h3>

            <div class="tags">

              <span class="tag">Data Analysis</span>
              <span class="tag">Data Cleaning</span>
              <span class="tag">EDA</span>
              <span class="tag">Statistical Analysis</span>
              <span class="tag">Feature Engineering</span>

            </div>

          </div>


          <div class="skill-card">

            <h3>
              Machine Learning
            </h3>

            <div class="tags">

              <span class="tag">Scikit-learn</span>
              <span class="tag">Supervised Learning</span>
              <span class="tag">Unsupervised Learning</span>
              <span class="tag">Predictive Modelling</span>
              <span class="tag">Model Evaluation</span>

            </div>

          </div>


          <div class="skill-card">

            <h3>
              Visualization
            </h3>

            <div class="tags">

              <span class="tag">Power BI</span>
              <span class="tag">Tableau</span>
              <span class="tag">Microsoft Excel</span>
              <span class="tag">Matplotlib</span>
              <span class="tag">Seaborn</span>

            </div>

          </div>

        </div>

      </div>

    </section>


    <!-- ================= EXPERIENCE ================= -->

    <section id="experience">

      <div class="container">

        <div class="section-heading">

          <div class="section-label">
            Experience
          </div>

          <h2>
            Professional experience
          </h2>

          <p>
            My practical experience in data science and analytics.
          </p>

        </div>


        <div class="timeline">

          <div class="timeline-item">

            <span class="timeline-date">
              FEB 2026 — PRESENT
            </span>

            <h3>
              Data Science Intern
            </h3>

            <h4>
              Techolas Technologies · Calicut, Kerala
            </h4>

            <ul>

              <li>
                Collected, cleaned and analysed datasets using Python,
                Pandas and NumPy.
              </li>

              <li>
                Performed Exploratory Data Analysis and statistical
                analysis to identify trends and patterns.
              </li>

              <li>
                Built and evaluated machine learning models using
                Scikit-learn.
              </li>

              <li>
                Developed interactive Power BI dashboards to communicate
                key metrics and business insights.
              </li>

            </ul>

          </div>

        </div>

      </div>

    </section>


    <!-- ================= PROJECTS ================= -->

    <section id="projects">

      <div class="container">

        <div class="section-heading">

          <div class="section-label">
            Projects
          </div>

          <h2>
            Selected work
          </h2>

          <p>
            A selection of projects demonstrating my interests in AI,
            machine learning and data-driven applications.
          </p>

        </div>


        <div class="projects-grid">


          <article class="project-card">

            <div class="project-top">
              🎥
            </div>

            <div class="project-content">

              <h3>
                Violence Detection Using YOLOv7
              </h3>

              <p>
                An AI-powered surveillance system designed to detect
                violent activities in real time and support faster
                threat identification.
              </p>

              <div class="project-tech">

                <span>Python</span>
                <span>YOLOv7</span>
                <span>Deep Learning</span>

              </div>

            </div>

          </article>


          <article class="project-card">

            <div class="project-top">
              🌾
            </div>

            <div class="project-content">

              <h3>
                AI-Powered Farm Expense Tracker
              </h3>

              <p>
                An AI-based system designed to monitor agricultural
                expenses, analyse spending patterns and support
                data-driven financial planning.
              </p>

              <div class="project-tech">

                <span>Python</span>
                <span>Machine Learning</span>
                <span>MySQL</span>

              </div>

            </div>

          </article>


        </div>

      </div>

    </section>


    <!-- ================= EDUCATION ================= -->

    <section id="education">

      <div class="container">

        <div class="section-heading">

          <div class="section-label">
            Education
          </div>

          <h2>
            Academic background
          </h2>

        </div>


        <div class="education-card">

          <div>

            <h3>
              Bachelor of Technology in Artificial Intelligence and Data Science
            </h3>

            <p>
              Dhanalakshmi Srinivasan College of Engineering, Coimbatore
            </p>

            <p>
              Anna University · 2026
            </p>

          </div>


          <div class="cgpa">

            <strong>
              8.0
            </strong>

            <span>
              CGPA / 10
            </span>

          </div>

        </div>

      </div>

    </section>


    <!-- ================= CERTIFICATIONS ================= -->

    <section id="certifications">

      <div class="container">

        <div class="section-heading">

          <div class="section-label">
            Certifications
          </div>

          <h2>
            Learning & certifications
          </h2>

        </div>


        <div class="cert-grid">


          <div class="cert-card">

            <strong>
              Machine Learning Internship
            </strong>

            <span>
              IPCS Global, Calicut · 2023
            </span>

          </div>


          <div class="cert-card">

            <strong>
              Data Science Internship
            </strong>

            <span>
              Camerin Folks Pvt. Ltd. · 2023
            </span>

          </div>


          <div class="cert-card">

            <strong>
              Data Science Program
            </strong>

            <span>
              Oracle Naan Mudhalvan, Anna University · 2024
            </span>

          </div>


          <div class="cert-card">

            <strong>
              UI/UX Design Program
            </strong>

            <span>
              Naan Mudhalvan, Anna University · 2025
            </span>

          </div>


        </div>

      </div>

    </section>


    <!-- ================= CONTACT ================= -->

    <section id="contact">

      <div class="container">

        <div class="contact-box">

          <h2>
            Let's connect.
          </h2>

          <p>
            I'm interested in opportunities related to data science,
            machine learning, data analytics and business intelligence.
          </p>


          <div class="contact-links">

            <a
              class="contact-link"
              href="mailto:aleeshafathimapk@gmail.com"
            >
              ✉ Email
            </a>


            <!--
              REPLACE # WITH YOUR LINKEDIN PROFILE URL

              Example:
              href="https://www.linkedin.com/in/yourusername/"
            -->

            <a
              class="contact-link"
              href="#"
            >
              LinkedIn
            </a>


            <!--
              REPLACE # WITH YOUR GITHUB PROFILE URL

              Example:
              href="https://github.com/yourusername"
            -->

            <a
              class="contact-link"
              href="#"
            >
              GitHub
            </a>

          </div>

        </div>

      </div>

    </section>

  </main>


  <!-- ================= FOOTER ================= -->

  <footer>

    <div class="container">

      <p>
        © 2026 Aleesha Fathima PK · Data Scientist
      </p>

    </div>

  </footer>

</body>
</html>

