<template>
  <section id="home" class="hero-section">
    <div class="hero-overlay"></div>

    <div class="container hero-container">
      <div class="hero-content">
        <p class="hero-greeting">FULL STACK DEVELOPER</p>

        <h1 class="hero-title">
          Building Scalable
          <span>Web Applications</span>
        </h1>

        <p class="hero-description">
          I create modern, high performance web applications using
          Node.js, Express, MongoDB, PostgreSQL and cloud technologies
          like AWS, Vercel, and Render.
        </p>

        <div class="hero-buttons">
          <a href="#projects" class="btn-primary">
            View My Work
            <i class="bi bi-arrow-right"></i>
          </a>

          <a href="#contact" class="btn-secondary">
            Get In Touch
          </a>
        </div>

        <div class="hero-stack">
          <div class="stack-item">
            <i class="bi bi-code-square"></i>
            <span>Clean Code</span>
          </div>

          <div class="stack-item">
            <i class="bi bi-bar-chart-line"></i>
            <span>Scalable Solutions</span>
          </div>

          <div class="stack-item">
            <i class="bi bi-cpu"></i>
            <span>Modern Stack</span>
          </div>

          <div class="stack-item">
            <i class="bi bi-puzzle"></i>
            <span>Problem Solver</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero-section {
  position: relative;
  min-height: 455px;
  overflow: hidden;
  display: flex;
  align-items: center;
  background: #050505 url("/images/hero.png") center center / cover no-repeat;
  border-bottom: 1px solid rgba(212, 175, 55, 0.08);
}

.hero-overlay {
  position: absolute;
  inset: 0;
  background:
    linear-gradient(
      90deg,
      rgba(5, 5, 5, 0.96) 0%,
      rgba(5, 5, 5, 0.88) 27%,
      rgba(5, 5, 5, 0.58) 48%,
      rgba(5, 5, 5, 0.12) 72%,
      rgba(5, 5, 5, 0.05) 100%
    ),
    linear-gradient(
      180deg,
      rgba(0, 0, 0, 0.18),
      rgba(0, 0, 0, 0.22)
    );
  z-index: 1;
}

.hero-container {
  position: relative;
  z-index: 2;
  width: 100%;
}

.hero-content {
  max-width: 560px;
  padding: 58px 0;
}

.hero-greeting {
  margin: 0 0 12px;
  color: #D4AF37;
  font-size: 0.72rem;
  font-weight: 600;
  letter-spacing: 4px;
  text-transform: uppercase;
}

.hero-title {
  margin: 0;
  color: #f5f5f5;
  font-size: clamp(2.5rem, 4.5vw, 4rem);
  font-weight: 700;
  line-height: 1.02;
  letter-spacing: -1.5px;
}

.hero-title span {
  display: block;
  color: #D4AF37;
}

.hero-description {
  max-width: 500px;
  margin: 20px 0 25px;
  color: #b8b8b8;
  font-size: 0.9rem;
  line-height: 1.65;
}

/* BUTTONS */

.hero-buttons {
  display: flex;
  align-items: center;
  gap: 15px;
  margin-bottom: 27px;
}

.hero-buttons a {
  text-decoration: none;
}

.btn-primary,
.btn-secondary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 9px;
  min-height: 42px;
  padding: 9px 19px;
  border-radius: 6px;
  font-size: 0.82rem;
  font-weight: 500;
  transition: all 0.3s ease;
}

.btn-primary {
  color: #080808;
  background: #D4AF37;
  border: 1px solid #D4AF37;
}

.btn-primary:hover {
  background: #E3C15A;
  border-color: #E3C15A;
  transform: translateY(-2px);
}

.btn-secondary {
  color: #D4AF37;
  background: transparent;
  border: 1px solid #D4AF37;
}

.btn-secondary:hover {
  background: rgba(212, 175, 55, 0.1);
  border-color: #FFD700;
  color: #FFD700;
  box-shadow: 0 0 15px rgba(212, 175, 55, 0.25);
  transform: translateY(-2px);
}

/* STACK */

.hero-stack {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  gap: 24px;
}

.stack-item {
  display: inline-flex;
  align-items: center;
  gap: 7px;
  color: #a7a7a7;
  font-size: 0.72rem;
  white-space: nowrap;
  transition: color 0.3s ease;
}

.stack-item i {
  color: #D4AF37;
  font-size: 0.9rem;
}

.stack-item:hover {
  color: #ffffff;
}

/* TABLET */

@media (max-width: 991px) {
  .hero-section {
    min-height: 440px;
    background-position: 58% center;
  }

  .hero-overlay {
    background:
      linear-gradient(
        90deg,
        rgba(5, 5, 5, 0.96) 0%,
        rgba(5, 5, 5, 0.82) 48%,
        rgba(5, 5, 5, 0.35) 100%
      );
  }

  .hero-content {
    max-width: 520px;
    padding: 55px 20px;
  }
}

/* MOBILE */

@media (max-width: 576px) {
  .hero-section {
    min-height: 590px;
    background-position: 65% center;
  }

  .hero-overlay {
    background:
      linear-gradient(
        180deg,
        rgba(5, 5, 5, 0.88) 0%,
        rgba(5, 5, 5, 0.76) 45%,
        rgba(5, 5, 5, 0.88) 100%
      );
  }

  .hero-content {
    padding: 55px 15px;
  }

  .hero-greeting {
    font-size: 0.65rem;
    letter-spacing: 3px;
  }

  .hero-title {
    font-size: 2.7rem;
    line-height: 1.03;
  }

  .hero-description {
    font-size: 0.88rem;
    line-height: 1.6;
  }

  .hero-buttons {
    flex-wrap: wrap;
  }

  .btn-primary,
  .btn-secondary {
    min-width: 135px;
  }

  .hero-stack {
    gap: 14px 20px;
  }

  .stack-item {
    font-size: 0.7rem;
  }
}
</style>