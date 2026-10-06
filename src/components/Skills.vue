<template>
  <section id="skills" class="skills-section">
    <div class="container">

      <!-- HEADER -->
      <div class="skills-header">
        <div class="skills-heading">
          <p class="section-label">TECHNICAL SKILLS</p>

          <h2 class="section-title">
            What I
            <span>Work With</span>
          </h2>
        </div>

        <p class="section-intro">
          Here are the technologies, tools, and platforms I use to build,
          deploy, and maintain modern web applications.
        </p>
      </div>

      <!-- SKILL GRID -->
      <div class="skills-grid">

        <!-- BACKEND -->
        <article class="skill-card">
          <div class="skill-card-header">
            <div class="skill-icon">
              <i class="bi bi-server"></i>
            </div>

            <div>
              <h3>Backend Development</h3>

              <p>
                Building robust APIs, server-side logic,
                and scalable backend systems.
              </p>
            </div>
          </div>

          <div class="skill-list">
            <span>
              <i class="bi bi-node-plus"></i>
              Node.js
            </span>

            <span>
              <i class="bi bi-code-slash"></i>
              Express.js
            </span>

            <span>
              <i class="bi bi-filetype-tsx"></i>
              TypeScript
            </span>

            <span>
              <i class="bi bi-braces"></i>
              REST APIs
            </span>

            <span>
              <i class="bi bi-shield-check"></i>
              Authentication
            </span>

            <span>
              <i class="bi bi-arrow-repeat"></i>
              CRUD
            </span>

            <span>
              <i class="bi bi-lightning-charge"></i>
              Socket.IO
            </span>

            <span>
              <i class="bi bi-check2-square"></i>
              Zod
            </span>
          </div>
        </article>

        <!-- DATABASE -->
        <article class="skill-card">
          <div class="skill-card-header">
            <div class="skill-icon">
              <i class="bi bi-database"></i>
            </div>

            <div>
              <h3>Database</h3>

              <p>
                Designing and working with databases
                to store and manage application data.
              </p>
            </div>
          </div>

          <div class="skill-list">
            <span>
              <i class="bi bi-circle-fill"></i>
              MongoDB
            </span>

            <span>
              <i class="bi bi-database-fill"></i>
              PostgreSQL
            </span>

            <span>
              <i class="bi bi-diagram-3"></i>
              Mongoose
            </span>

            <span>
              <i class="bi bi-table"></i>
              Data Modeling
            </span>
          </div>
        </article>

        <!-- FRONTEND -->
        <article class="skill-card">
          <div class="skill-card-header">
            <div class="skill-icon">
              <i class="bi bi-display"></i>
            </div>

            <div>
              <h3>Frontend Development</h3>

              <p>
                Building responsive interfaces and
                connecting frontend applications with APIs.
              </p>
            </div>
          </div>

          <div class="skill-list">
            <span>
              <i class="bi bi-code-square"></i>
              Vue.js
            </span>

            <span>
              <i class="bi bi-braces"></i>
              React.js
            </span>

            <span>
              <i class="bi bi-filetype-js"></i>
              JavaScript
            </span>

            <span>
              <i class="bi bi-filetype-html"></i>
              HTML5
            </span>

            <span>
              <i class="bi bi-filetype-css"></i>
              CSS3
            </span>

            <span>
              <i class="bi bi-bootstrap"></i>
              Bootstrap
            </span>
          </div>
        </article>

        <!-- CLOUD -->
        <article class="skill-card">
          <div class="skill-card-header">
            <div class="skill-icon">
              <i class="bi bi-cloud"></i>
            </div>

            <div>
              <h3>Cloud & Deployment</h3>

              <p>
                Deploying and managing applications
                across cloud and production environments.
              </p>
            </div>
          </div>

          <div class="skill-list">
            <span>
              <i class="bi bi-cloud-fill"></i>
              AWS
            </span>

            <span>
              <i class="bi bi-hdd-rack"></i>
              EC2
            </span>

            <span>
              <i class="bi bi-bucket"></i>
              S3
            </span>

            <span>
              <i class="bi bi-lightning"></i>
              Lambda
            </span>

            <span>
              <i class="bi bi-diagram-3"></i>
              API Gateway
            </span>

            <span>
              <i class="bi bi-server"></i>
              Nginx
            </span>

            <span>
              <i class="bi bi-gear"></i>
              PM2
            </span>

            <span>
              <i class="bi bi-cloud-arrow-up"></i>
              Render
            </span>

            <span>
              <i class="bi bi-triangle"></i>
              Vercel
            </span>
          </div>
        </article>

        <!-- TOOLS -->
        <article class="skill-card skill-card-wide">
          <div class="skill-card-header">
            <div class="skill-icon">
              <i class="bi bi-tools"></i>
            </div>

            <div>
              <h3>Tools & DevOps</h3>

              <p>
                Tools I use for development, testing,
                version control, and deployment.
              </p>
            </div>
          </div>

          <div class="skill-list">
            <span>
              <i class="bi bi-git"></i>
              Git
            </span>

            <span>
              <i class="bi bi-github"></i>
              GitHub
            </span>

            <span>
              <i class="bi bi-send"></i>
              Postman
            </span>

            <span>
              <i class="bi bi-box"></i>
              Docker
            </span>

            <span>
              <i class="bi bi-terminal"></i>
              VS Code
            </span>

            <span>
              <i class="bi bi-check-circle"></i>
              Chai
            </span>

            <span>
              <i class="bi bi-beaker"></i>
              API Testing
            </span>

            <span>
              <i class="bi bi-github"></i>
              GitHub Actions
            </span>
          </div>
        </article>

      </div>

    </div>
  </section>
</template>

<style scoped>
/* SKILLS SECTION */

.skills-section {
  position: relative;

  padding: 105px 0 95px;

  background: #050505;

  overflow: hidden;
}

.skills-section::before {
  content: "";

  position: absolute;

  top: -180px;
  left: -180px;

  width: 420px;
  height: 420px;

  background: radial-gradient(
    circle,
    rgba(212, 175, 55, 0.06),
    transparent 68%
  );

  pointer-events: none;
}

/* HEADER */

.skills-header {
  display: flex;
  align-items: flex-end;
  justify-content: space-between;

  gap: 60px;

  margin-bottom: 45px;
}

.skills-heading {
  flex-shrink: 0;
}

.section-label {
  margin: 0 0 11px;

  color: #D4AF37;

  font-size: 0.67rem;
  font-weight: 600;

  letter-spacing: 3px;
}

.section-title {
  margin: 0;

  color: #F5F5F5;

  font-size: clamp(2.7rem, 4.5vw, 3.8rem);

  font-weight: 700;

  line-height: 0.98;

  letter-spacing: -1.7px;
}

.section-title span {
  display: block;

  color: #D4AF37;
}

.section-intro {
  max-width: 450px;

  margin: 0 0 3px;

  color: #a7a7a7;

  font-size: 0.82rem;

  line-height: 1.7;
}

/* SKILL GRID */

.skills-grid {
  display: grid;

  grid-template-columns: repeat(2, 1fr);

  gap: 16px;
}

/* SKILL CARD */

.skill-card {
  padding: 25px;

  background: #080808;

  border: 1px solid rgba(212, 175, 55, 0.13);

  border-radius: 10px;

  transition:
    transform 0.3s ease,
    border-color 0.3s ease,
    box-shadow 0.3s ease;
}

.skill-card:hover {
  transform: translateY(-3px);

  border-color: rgba(212, 175, 55, 0.32);

  box-shadow:
    0 14px 35px rgba(0, 0, 0, 0.32);
}

/* WIDE CARD */

.skill-card-wide {
  grid-column: 1 / -1;
}

/* CARD HEADER */

.skill-card-header {
  display: flex;
  align-items: flex-start;

  gap: 18px;

  margin-bottom: 22px;
}

/* ICON */

.skill-icon {
  flex-shrink: 0;

  width: 54px;
  height: 54px;

  display: flex;
  align-items: center;
  justify-content: center;

  color: #D4AF37;

  background:
    linear-gradient(
      145deg,
      rgba(212, 175, 55, 0.08),
      rgba(212, 175, 55, 0.015)
    );

  border: 1px solid rgba(212, 175, 55, 0.5);

  border-radius: 11px;

  font-size: 1.55rem;
}

/* CARD TITLE */

.skill-card h3 {
  margin: 2px 0 6px;

  color: #F5F5F5;

  font-size: 1.12rem;

  font-weight: 600;
}

/* CARD DESCRIPTION */

.skill-card-header p {
  max-width: 480px;

  margin: 0;

  color: #8f8f8f;

  font-size: 0.75rem;

  line-height: 1.55;
}

/* SKILL LIST */

.skill-list {
  display: flex;

  flex-wrap: wrap;

  gap: 8px;
}

/* SKILL ITEM */

.skill-list span {
  display: inline-flex;

  align-items: center;

  gap: 8px;

  padding: 8px 12px;

  color: #c4c4c4;

  background: #0b0b0b;

  border: 1px solid rgba(212, 175, 55, 0.1);

  border-radius: 7px;

  font-size: 0.7rem;

  transition:
    color 0.25s ease,
    border-color 0.25s ease,
    background 0.25s ease;
}

.skill-list span i {
  color: #D4AF37;

  font-size: 0.78rem;
}

.skill-list span:hover {
  color: #F5F5F5;

  background: rgba(212, 175, 55, 0.045);

  border-color: rgba(212, 175, 55, 0.3);
}

/* TABLET */

@media (max-width: 991px) {
  .skills-section {
    padding: 90px 0 75px;
  }

  .skills-header {
    align-items: flex-start;

    flex-direction: column;

    gap: 20px;

    margin-bottom: 35px;
  }

  .section-intro {
    max-width: 620px;
  }

  .skills-grid {
    gap: 14px;
  }

  .skill-card {
    padding: 22px;
  }
}

/* MOBILE */

@media (max-width: 767px) {
  .skills-section {
    padding: 75px 0 60px;
  }

  .section-label {
    font-size: 0.62rem;

    letter-spacing: 2.5px;
  }

  .section-title {
    font-size: 2.7rem;
  }

  .skills-grid {
    grid-template-columns: 1fr;
  }

  .skill-card-wide {
    grid-column: auto;
  }

  .skill-card {
    padding: 21px;
  }

  .skill-card-header {
    gap: 14px;

    margin-bottom: 18px;
  }

  .skill-icon {
    width: 48px;
    height: 48px;

    font-size: 1.35rem;
  }

  .skill-card h3 {
    font-size: 1rem;
  }

  .skill-card-header p {
    font-size: 0.72rem;
  }
}

/* SMALL MOBILE */

@media (max-width: 576px) {
  .section-title {
    font-size: 2.5rem;
  }

  .skill-card {
    padding: 19px;
  }

  .skill-list {
    gap: 7px;
  }

  .skill-list span {
    padding: 7px 10px;

    font-size: 0.66rem;
  }
}
</style>