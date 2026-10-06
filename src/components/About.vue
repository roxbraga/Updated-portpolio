<template>
  <section id="about" class="about-section">
    <div class="container">

      <!-- MAIN ABOUT -->
      <div class="row align-items-center about-main">

        <!-- IMAGE -->
        <div class="col-lg-5">
          <div class="about-image-wrapper">
            <img
              src="/images/profile.png"
              alt="Cristino France - Backend Full-Stack Developer"
              class="about-image"
            />
          </div>
        </div>

        <!-- CONTENT -->
        <div class="col-lg-7">
          <div class="about-content">

            <!-- LABEL -->
            <div class="about-label">
              <span>ABOUT ME</span>
              <div class="label-line"></div>
            </div>

            <!-- TITLE -->
            <h2 class="about-title">
              More than just
              <span>writing code.</span>
            </h2>

            <!-- DESCRIPTION -->
            <div class="about-description">

              <p>
                I'm a backend-focused developer who enjoys turning ideas
                into working applications and solving the technical problems
                behind them.
              </p>

              <p>
                I've worked on projects involving APIs, databases,
                authentication, e-commerce workflows, cloud deployment,
                and real-time communication.
              </p>

              <p>
                I enjoy understanding how applications work from end to end -
                from designing backend logic to connecting services,
                deploying applications, and continuously improving systems.
              </p>

            </div>

          </div>
        </div>

      </div>

      <!-- ABOUT HIGHLIGHTS -->
      <div class="about-highlights">

        <!-- ITEM 1 -->
        <div class="highlight-item">
          <div class="highlight-icon">
            <i class="bi bi-hdd-rack"></i>
          </div>

          <div class="highlight-content">
            <h3>Backend Focus</h3>
            <p>
              Designing robust and
              maintainable systems.
            </p>
          </div>
        </div>

        <!-- ITEM 2 -->
        <div class="highlight-item">
          <div class="highlight-icon">
            <i class="bi bi-cloud"></i>
          </div>

          <div class="highlight-content">
            <h3>Cloud & Deployment</h3>
            <p>
              Bringing applications
              from development to production.
            </p>
          </div>
        </div>

        <!-- ITEM 3 -->
        <div class="highlight-item">
          <div class="highlight-icon">
            <i class="bi bi-diagram-3"></i>
          </div>

          <div class="highlight-content">
            <h3>System Integration</h3>
            <p>
              Connecting different
              technologies and services.
            </p>
          </div>
        </div>

        <!-- ITEM 4 -->
        <div class="highlight-item">
          <div class="highlight-icon">
            <i class="bi bi-bar-chart-line"></i>
          </div>

          <div class="highlight-content">
            <h3>Continuous Growth</h3>
            <p>
              Always learning and
              exploring new tools to build better solutions.
            </p>
          </div>
        </div>

      </div>

    </div>
  </section>
</template>

<style scoped>
/* ABOUT SECTION */

.about-section {
  position: relative;
  padding: 105px 0 85px;

  background: #050505;

  overflow: hidden;
}

/* MAIN CONTENT */

.about-main {
  min-height: 500px;
}

/* IMAGE */

.about-image-wrapper {
  position: relative;

  display: flex;
  align-items: center;
  justify-content: center;

  min-height: 500px;
}

.about-image-wrapper::before {
  content: "";

  position: absolute;

  width: 330px;
  height: 330px;

  border-radius: 50%;

  background: rgba(212, 175, 55, 0.07);

  filter: blur(85px);

  z-index: 0;
}

.about-image {
  position: relative;
  z-index: 1;

  width: 100%;
  max-width: 540px;

  object-fit: contain;

  filter:
    drop-shadow(0 18px 35px rgba(0, 0, 0, 0.45));
}

/* CONTENT */

.about-content {
  padding-left: 35px;
}

/* LABEL */

.about-label {
  display: flex;
  align-items: center;
  gap: 14px;

  margin-bottom: 18px;
}

.about-label span {
  color: #D4AF37;

  font-size: 0.72rem;
  font-weight: 600;

  letter-spacing: 3.5px;
}

.label-line {
  width: 65px;
  height: 1px;

  background: #D4AF37;
}

/* TITLE */

.about-title {
  max-width: 650px;

  margin: 0 0 25px;

  color: #F5F5F5;

  font-size: clamp(2.5rem, 4vw, 3.8rem);

  font-weight: 700;

  line-height: 1.05;
  letter-spacing: -1px;
}

.about-title span {
  display: block;

  color: #D4AF37;
}

/* DESCRIPTION */

.about-description {
  max-width: 650px;
}

.about-description p {
  margin-bottom: 18px;

  color: #a7a7a7;

  font-size: 0.92rem;

  line-height: 1.7;
}

.about-description p:last-child {
  margin-bottom: 0;
}

/* HIGHLIGHTS */

.about-highlights {
  display: grid;

  grid-template-columns: repeat(4, 1fr);

  margin-top: 60px;

  padding-top: 28px;

  border-top: 1px solid rgba(212, 175, 55, 0.12);
}

/* HIGHLIGHT ITEM */

.highlight-item {
  display: flex;
  align-items: flex-start;

  gap: 16px;

  padding: 0 28px;

  min-height: 75px;
}

.highlight-item:first-child {
  padding-left: 0;
}

.highlight-item:last-child {
  padding-right: 0;
}

.highlight-item:not(:last-child) {
  border-right: 1px solid rgba(212, 175, 55, 0.1);
}

/* ICON */

.highlight-icon {
  flex-shrink: 0;

  color: #D4AF37;

  font-size: 1.45rem;

  line-height: 1;
}

/* TEXT */

.highlight-content h3 {
  margin: 0 0 7px;

  color: #e5e5e5;

  font-size: 0.84rem;

  font-weight: 600;
}

.highlight-content p {
  max-width: 170px;

  margin: 0;

  color: #737373;

  font-size: 0.76rem;

  line-height: 1.5;
}

/* TABLET */

@media (max-width: 991px) {
  .about-section {
    padding: 90px 0 70px;
  }

  .about-main {
    min-height: auto;
  }

  .about-image-wrapper {
    min-height: auto;

    margin-bottom: 40px;
  }

  .about-image {
    max-width: 500px;
  }

  .about-content {
    padding-left: 0;

    text-align: center;
  }

  .about-label {
    justify-content: center;
  }

  .about-title {
    margin-left: auto;
    margin-right: auto;
  }

  .about-description {
    margin-left: auto;
    margin-right: auto;
  }

  .about-highlights {
    grid-template-columns: repeat(2, 1fr);

    gap: 30px;

    border-top: none;
  }

  .highlight-item {
    padding: 0 20px;
  }

  .highlight-item:nth-child(2) {
    border-right: none;
  }

  .highlight-item:nth-child(3) {
    padding-left: 20px;
  }
}

/* MOBILE */

@media (max-width: 576px) {
  .about-section {
    padding: 75px 0 60px;
  }

  .about-image-wrapper {
    margin-bottom: 25px;
  }

  .about-image {
    width: 115%;
    max-width: none;
    margin-left: -7.5%;
  }

  .about-label {
    gap: 10px;
  }

  .about-label span {
    font-size: 0.68rem;
    letter-spacing: 2.5px;
  }

  .label-line {
    width: 45px;
  }

  .about-title {
    font-size: 2.5rem;
    line-height: 1.05;
  }

  .about-description p {
    font-size: 0.88rem;
    line-height: 1.7;
  }

  .about-highlights {
    grid-template-columns: 1fr;

    gap: 25px;

    margin-top: 50px;
  }

  .highlight-item,
  .highlight-item:first-child,
  .highlight-item:last-child {
    padding: 0;

    border-right: none;
  }

  .highlight-item:not(:last-child) {
    padding-bottom: 22px;

    border-bottom: 1px solid rgba(212, 175, 55, 0.1);
  }

  .highlight-content p {
    max-width: none;
  }
}
</style>