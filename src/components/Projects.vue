<template>
  <section id="projects" class="projects-section">
    <div class="container">

      <!-- SECTION HEADER -->
      <div class="projects-header">
        <div class="header-title">
          <p class="section-label">FEATURED PROJECTS</p>

          <h2 class="section-title">
            Some Things
            <span>I've Built</span>
          </h2>
        </div>

        <p class="section-intro">
          Here are some of my recent projects. Each one was built to solve
          real problems and showcase my skills in backend, full-stack
          development, and deployment.
        </p>
      </div>


      <!-- FEATURED PROJECT -->
      <article class="featured-project">

        <div class="featured-image">
          <img
            src="/images/ecommerce.png"
            alt="Fullstack E-commerce App"
          />
        </div>

        <div class="featured-content">

          <div class="project-tags">
            <span class="category-tag">
              <i class="bi bi-stack"></i>
              Full-Stack
            </span>

            <span class="category-tag">
              <i class="bi bi-cart3"></i>
              E-commerce
            </span>
          </div>

          <h3>Fullstack E-commerce App</h3>

          <p class="project-description">
            A complete e-commerce platform with authentication, cart,
            checkout, admin management, and REST API integration.
          </p>

          <div class="tech-stack">
            <span>Vue.js</span>
            <span>Node.js</span>
            <span>MongoDB</span>
            <span>Stripe</span>
          </div>

          <div class="featured-details">

            <div class="detail-item">
              <i class="bi bi-person-check"></i>
              <span>User Authentication</span>
            </div>

            <div class="detail-item">
              <i class="bi bi-speedometer2"></i>
              <span>Admin Dashboard</span>
            </div>

            <div class="detail-item">
              <i class="bi bi-box-seam"></i>
              <span>Product Management</span>
            </div>

            <div class="detail-item">
              <i class="bi bi-cart-check"></i>
              <span>Shopping Cart & Checkout</span>
            </div>

            <div class="detail-item">
              <i class="bi bi-cloud-check"></i>
              <span>Cloud Deployment</span>
            </div>

            <div class="detail-item">
              <i class="bi bi-diagram-3"></i>
              <span>REST API Integration</span>
            </div>

          </div>

          <div class="project-links">
            <a
              href="https://fullstack-ecommerce-app-v41g.onrender.com/"
              target="_blank"
              rel="noopener"
              class="live-link"
            >
              Live Demo
              <i class="bi bi-arrow-up-right"></i>
            </a>

            <span class="link-divider"></span>

            <a
              href="https://github.com/roxbraga/fullstack-ecommerce-app"
              target="_blank"
              rel="noopener"
              class="code-link"
            >
              <i class="bi bi-github"></i>
              View Code
            </a>
          </div>

        </div>

      </article>


      <!-- SECONDARY PROJECTS -->
      <div class="secondary-projects">

        <!-- PROXY CHECKER -->
        <article class="secondary-card">

          <div class="secondary-image">
            <img
              src="/images/Proxy.png"
              alt="Proxy Checker"
            />
          </div>

          <div class="secondary-content">

            <div class="project-tags">
              <span class="category-tag">
                <i class="bi bi-tools"></i>
                Tool
              </span>

              <span class="category-tag">
                <i class="bi bi-hdd-rack"></i>
                Backend
              </span>
            </div>

            <h3>Proxy Checker</h3>

            <p class="project-description">
              A TypeScript and Node.js CLI tool for validating proxy
              connectivity, measuring response times, and processing
              proxy lists concurrently.
            </p>

            <div class="tech-stack">
              <span>TypeScript</span>
              <span>Node.js</span>
              <span>Axios</span>
              <span>Docker</span>
            </div>

            <div class="project-links">
              <a
                href="https://github.com/roxbraga/Proxy-checker"
                target="_blank"
                rel="noopener"
                class="live-link"
              >
                View Project
                <i class="bi bi-arrow-up-right"></i>
              </a>

              <span class="link-divider"></span>

              <a
                href="https://github.com/roxbraga/Proxy-checker"
                target="_blank"
                rel="noopener"
                class="code-link"
              >
                <i class="bi bi-github"></i>
                View Code
              </a>
            </div>

          </div>

        </article>


        <!-- REST API -->
        <article class="secondary-card">

          <div class="secondary-image">
            <img
              src="/images/Postman.png"
              alt="REST API E-commerce Database"
            />
          </div>

          <div class="secondary-content">

            <div class="project-tags">
              <span class="category-tag">
                <i class="bi bi-hdd-rack"></i>
                Backend
              </span>

              <span class="category-tag">
                <i class="bi bi-braces"></i>
                REST API
              </span>
            </div>

            <h3>REST API E-commerce Database</h3>

            <p class="project-description">
              A RESTful e-commerce API built with Node.js, Express,
              and MongoDB, featuring CRUD operations, authentication,
              database integration, and API testing with Postman.
            </p>

            <div class="tech-stack">
              <span>Node.js</span>
              <span>Express</span>
              <span>MongoDB</span>
              <span>Postman</span>
            </div>

            <div class="project-links">
              <a
                href="https://fullstack-ecommerce-api-1.onrender.com"
                target="_blank"
                rel="noopener"
                class="live-link"
              >
                Live API
                <i class="bi bi-arrow-up-right"></i>
              </a>

              <span class="link-divider"></span>

              <a
                href="https://github.com/roxbraga/fullstack-ecommerce-api"
                target="_blank"
                rel="noopener"
                class="code-link"
              >
                <i class="bi bi-github"></i>
                View Code
              </a>
            </div>

          </div>

        </article>

      </div>


      <!-- MORE PROJECTS CTA -->
      <div class="projects-cta">

        <div class="cta-content">
          <p>MORE PROJECTS</p>

          <h3>
            Interested in seeing
            <span>more of my work?</span>
          </h3>

          <small>
            Check out my GitHub for more projects and contributions.
          </small>
        </div>

        <a
          href="https://github.com/roxbraga"
          target="_blank"
          rel="noopener"
          class="github-btn"
        >
          <i class="bi bi-github"></i>
          Visit GitHub
          <i class="bi bi-arrow-right"></i>
        </a>

      </div>

    </div>
  </section>
</template>


<style scoped>
/* PROJECTS SECTION */

.projects-section {
  position: relative;

  padding: 105px 0 90px;

  background: #050505;

  overflow: hidden;
}

/* HEADER */

.projects-header {
  display: flex;
  align-items: flex-end;
  justify-content: space-between;

  gap: 55px;

  margin-bottom: 42px;
}

.header-title {
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
  max-width: 440px;

  margin: 0 0 3px;

  color: #a7a7a7;

  font-size: 0.82rem;
  line-height: 1.7;
}

/* FEATURED PROJECT */

.featured-project {
  display: grid;

  grid-template-columns: 52% 48%;

  min-height: 455px;

  overflow: hidden;

  background: #080808;

  border: 1px solid rgba(212, 175, 55, 0.2);

  border-radius: 10px;

  transition:
    transform 0.3s ease,
    border-color 0.3s ease,
    box-shadow 0.3s ease;
}

.featured-project:hover {
  transform: translateY(-3px);

  border-color: rgba(212, 175, 55, 0.38);

  box-shadow:
    0 18px 45px rgba(0, 0, 0, 0.38);
}

/* FEATURED IMAGE */

.featured-image {
  position: relative;

  min-height: 455px;

  overflow: hidden;

  background: #080808;

  border-right: 1px solid rgba(212, 175, 55, 0.1);
}

.featured-image::after {
  content: "";

  position: absolute;
  inset: 0;

  background:
    linear-gradient(
      90deg,
      rgba(5, 5, 5, 0.02) 55%,
      rgba(5, 5, 5, 0.5) 100%
    );
}

.featured-image img {
  width: 100%;
  height: 100%;

  display: block;

  object-fit: cover;

  transition: transform 0.6s ease;
}

.featured-project:hover .featured-image img {
  transform: scale(1.025);
}

/* FEATURED CONTENT */

.featured-content {
  display: flex;
  flex-direction: column;
  justify-content: center;

  padding: 38px 42px;
}

/* PROJECT TAGS */

.project-tags {
  display: flex;
  align-items: center;
  flex-wrap: wrap;

  gap: 7px;

  margin-bottom: 13px;
}

.category-tag {
  display: inline-flex;
  align-items: center;

  gap: 6px;

  padding: 5px 9px;

  color: #c2c2c2;

  background: #0d0d0d;

  border: 1px solid rgba(212, 175, 55, 0.14);

  border-radius: 5px;

  font-size: 0.64rem;
  font-weight: 500;
}

.category-tag i {
  color: #D4AF37;

  font-size: 0.65rem;
}

/* PROJECT TITLE */

.featured-content h3,
.secondary-content h3 {
  margin: 0 0 10px;

  color: #F5F5F5;

  font-weight: 600;
}

.featured-content h3 {
  font-size: 1.45rem;
}

/* DESCRIPTION */

.project-description {
  max-width: 560px;

  margin: 0 0 18px;

  color: #969696;

  font-size: 0.8rem;

  line-height: 1.65;
}

/* TECH STACK */

.tech-stack {
  display: flex;
  flex-wrap: wrap;

  gap: 7px;

  margin-bottom: 22px;
}

.tech-stack span {
  padding: 5px 9px;

  color: #a5a5a5;

  background: rgba(212, 175, 55, 0.025);

  border: 1px solid rgba(212, 175, 55, 0.16);

  border-radius: 5px;

  font-size: 0.64rem;
}

/* FEATURE DETAILS */

.featured-details {
  display: grid;

  grid-template-columns: repeat(2, 1fr);

  gap: 11px 20px;

  margin-bottom: 25px;

  padding-top: 18px;

  border-top: 1px solid rgba(212, 175, 55, 0.1);
}

.detail-item {
  display: flex;
  align-items: center;

  gap: 8px;

  color: #858585;

  font-size: 0.69rem;
}

.detail-item i {
  flex-shrink: 0;

  color: #D4AF37;

  font-size: 0.8rem;
}

/* PROJECT LINKS */

.project-links {
  display: flex;
  align-items: center;

  gap: 18px;
}

.project-links a {
  display: inline-flex;
  align-items: center;

  gap: 7px;

  text-decoration: none;

  font-size: 0.73rem;
  font-weight: 500;

  transition: all 0.25s ease;
}

.live-link {
  color: #D4AF37;
}

.live-link:hover {
  color: #E3C15A;

  transform: translateX(2px);
}

.code-link {
  color: #8e8e8e;
}

.code-link:hover {
  color: #F5F5F5;
}

.code-link i {
  font-size: 0.92rem;
}

.link-divider {
  width: 1px;
  height: 17px;

  background: rgba(212, 175, 55, 0.18);
}

/* SECONDARY PROJECTS */

.secondary-projects {
  display: grid;

  grid-template-columns: repeat(2, 1fr);

  gap: 16px;

  margin-top: 16px;
}

.secondary-card {
  overflow: hidden;

  background: #080808;

  border: 1px solid rgba(212, 175, 55, 0.11);

  border-radius: 9px;

  transition:
    transform 0.3s ease,
    border-color 0.3s ease,
    box-shadow 0.3s ease;
}

.secondary-card:hover {
  transform: translateY(-3px);

  border-color: rgba(212, 175, 55, 0.3);

  box-shadow:
    0 14px 35px rgba(0, 0, 0, 0.32);
}

/* SECONDARY IMAGE */

.secondary-image {
  position: relative;

  height: 245px;

  overflow: hidden;

  background: #080808;

  border-bottom: 1px solid rgba(212, 175, 55, 0.1);
}

.secondary-image img {
  width: 100%;
  height: 100%;

  display: block;

  object-fit: cover;

  transition: transform 0.5s ease;
}

.secondary-card:hover .secondary-image img {
  transform: scale(1.025);
}

/* SECONDARY CONTENT */

.secondary-content {
  padding: 24px 25px 25px;
}

.secondary-content h3 {
  font-size: 1.08rem;
}

/* MORE PROJECTS CTA */

.projects-cta {
  position: relative;

  display: flex;
  align-items: center;
  justify-content: space-between;

  gap: 30px;

  margin-top: 55px;

  padding: 32px 38px;

  overflow: hidden;

  background:
    radial-gradient(
      circle at 88% 50%,
      rgba(212, 175, 55, 0.11),
      transparent 31%
    ),
    #080808;

  border: 1px solid rgba(212, 175, 55, 0.17);

  border-radius: 9px;
}

.projects-cta::after {
  content: "";

  position: absolute;

  right: 7%;
  bottom: -95px;

  width: 260px;
  height: 190px;

  border: 1px solid rgba(212, 175, 55, 0.07);

  border-radius: 50%;

  transform: rotate(-10deg);

  pointer-events: none;
}

.cta-content {
  position: relative;
  z-index: 1;
}

.cta-content p {
  margin: 0 0 7px;

  color: #D4AF37;

  font-size: 0.62rem;
  font-weight: 600;

  letter-spacing: 2.5px;
}

.cta-content h3 {
  margin: 0 0 8px;

  color: #F5F5F5;

  font-size: 1.5rem;
  font-weight: 600;

  line-height: 1.15;
}

.cta-content h3 span {
  display: block;

  color: #D4AF37;
}

.cta-content small {
  color: #737373;

  font-size: 0.7rem;
}

/* GITHUB BUTTON */

.github-btn {
  position: relative;
  z-index: 1;

  display: inline-flex;
  align-items: center;
  justify-content: center;

  gap: 9px;

  min-width: 150px;

  padding: 12px 20px;

  background: #D4AF37;

  border: 1px solid #D4AF37;

  border-radius: 6px;

  color: #080808;

  text-decoration: none;

  font-size: 0.77rem;
  font-weight: 600;

  white-space: nowrap;

  transition: all 0.3s ease;
}

.github-btn:hover {
  background: #E3C15A;
  border-color: #E3C15A;

  color: #080808;

  transform: translateY(-2px);

  box-shadow:
    0 8px 22px rgba(212, 175, 55, 0.15);
}

/* TABLET */

@media (max-width: 991px) {
  .projects-section {
    padding: 90px 0 70px;
  }

  .projects-header {
    align-items: flex-start;

    flex-direction: column;

    gap: 20px;

    margin-bottom: 35px;
  }

  .section-intro {
    max-width: 600px;
  }

  .featured-project {
    grid-template-columns: 48% 52%;
  }

  .featured-content {
    padding: 30px;
  }

  .featured-details {
    gap: 10px;
  }

  .secondary-image {
    height: 210px;
  }
}

/* MOBILE */

@media (max-width: 767px) {
  .projects-section {
    padding: 75px 0 60px;
  }

  .section-label {
    font-size: 0.62rem;

    letter-spacing: 2.5px;
  }

  .section-title {
    font-size: 2.7rem;
  }

  .featured-project {
    display: block;
  }

  .featured-image {
    min-height: 270px;

    border-right: none;

    border-bottom: 1px solid rgba(212, 175, 55, 0.1);
  }

  .featured-content {
    padding: 25px 22px;
  }

  .featured-content h3 {
    font-size: 1.2rem;
  }

  .featured-details {
    grid-template-columns: 1fr;

    gap: 10px;

    margin-bottom: 22px;
  }

  .secondary-projects {
    grid-template-columns: 1fr;

    gap: 14px;
  }

  .secondary-image {
    height: 230px;
  }

  .secondary-content {
    padding: 22px;
  }

  .projects-cta {
    flex-direction: column;

    align-items: flex-start;

    padding: 27px 23px;
  }

  .github-btn {
    width: 100%;
  }
}

/* SMALL MOBILE */

@media (max-width: 576px) {
  .section-title {
    font-size: 2.5rem;
  }

  .featured-image {
    min-height: 220px;
  }

  .secondary-image {
    height: 200px;
  }

  .featured-content {
    padding: 22px 19px;
  }

  .secondary-content {
    padding: 20px;
  }

  .project-description {
    font-size: 0.76rem;
  }

  .projects-cta {
    margin-top: 45px;
  }

  .cta-content h3 {
    font-size: 1.3rem;
  }
}
</style>