<template>
  <header class="navbar-wrapper">
    <nav class="navbar navbar-expand-lg">
      <div class="container">

        <!-- Logo -->
        <a href="#home" class="brand">
          <span class="brand-name">Cristino France</span>
          <span class="brand-role">WEB DEVELOPER</span>
        </a>

        <!-- Mobile Toggle -->
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#mainNavbar"
          aria-controls="mainNavbar"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <i class="bi bi-list"></i>
        </button>

        <!-- Navigation -->
        <div id="mainNavbar" class="collapse navbar-collapse">
          <ul class="navbar-nav mx-auto">
            <li class="nav-item">
              <a class="nav-link active" href="#home">Home</a>
            </li>

            <li class="nav-item">
              <a class="nav-link" href="#about">About</a>
            </li>

            <li class="nav-item">
              <a class="nav-link" href="#projects">Projects</a>
            </li>

            <li class="nav-item">
              <a class="nav-link" href="#skills">Skills</a>
            </li>

            <li class="nav-item">
              <a class="nav-link" href="#contact">Contact</a>
            </li>
          </ul>

          <!-- Download CV -->
          <a
            href="/images/CFM-Resume.pdf"
            target="_blank"
            rel="noopener"
            class="hire-btn"
          >
            <i class="bi bi-download"></i>
            Download CV
          </a>
        </div>

      </div>
    </nav>
  </header>
</template>

<style scoped>
.navbar-wrapper {
  position: sticky;
  top: 0;
  z-index: 1000;

  background: rgba(5, 5, 5, 0.94);
  backdrop-filter: blur(12px);

  border-bottom: 1px solid rgba(212, 175, 55, 0.12);
}

.navbar {
  min-height: 78px;
}

/* BRAND */

.brand {
  display: flex;
  flex-direction: column;
  text-decoration: none;
  line-height: 1;
}

.brand-name {
  color: #f5f5f5;

  font-size: 1.5rem;
  font-weight: 700;
  letter-spacing: -0.5px;

  transition: color 0.3s ease;
}

.brand:hover .brand-name {
  color: #D4AF37;
}

.brand-role {
  margin-top: 6px;

  color: #D4AF37;

  font-size: 0.47rem;
  font-weight: 600;
  letter-spacing: 3.5px;
}

/* NAV LINKS */

.navbar-nav {
  gap: 7px;
}

.nav-link {
  position: relative;

  padding: 8px 14px !important;

  color: #9a9a9a !important;

  font-size: 0.9rem;
  font-weight: 500;

  transition: color 0.3s ease;
}

.nav-link:hover,
.nav-link.active {
  color: #D4AF37 !important;
}

.nav-link::after {
  content: "";

  position: absolute;

  left: 50%;
  bottom: 1px;

  width: 0;
  height: 1px;

  transform: translateX(-50%);

  background: #D4AF37;

  transition: width 0.3s ease;
}

.nav-link:hover::after,
.nav-link.active::after {
  width: 22px;
}

/* DOWNLOAD CV */

.hire-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 9px;

  min-width: 128px;
  min-height: 42px;
  padding: 9px 19px;

  border: 1px solid #D4AF37;
  border-radius: 6px;

  background: #D4AF37;
  color: #080808;

  text-decoration: none;

  font-size: 0.82rem;
  font-weight: 500;

  transition: all 0.3s ease;
}

.hire-btn i {
  font-size: 0.85rem;
}

.hire-btn:hover {
  background: #E3C15A;
  border-color: #E3C15A;
  color: #080808;

  transform: translateY(-2px);
}

/* MOBILE */

.navbar-toggler {
  padding: 7px 10px;

  border: 1px solid rgba(212, 175, 55, 0.45);

  color: #D4AF37;
}

.navbar-toggler:focus {
  box-shadow: none;
}

.navbar-toggler i {
  font-size: 1.5rem;
}

@media (max-width: 991px) {
  .navbar-collapse {
    margin-top: 15px;
    padding: 18px;

    background: rgba(5, 5, 5, 0.98);

    border: 1px solid rgba(212, 175, 55, 0.14);
    border-radius: 8px;
  }

  .navbar-nav {
    gap: 2px;
  }

  .nav-link {
    padding: 11px 8px !important;
  }

  .hire-btn {
    width: 100%;
    margin-top: 12px;
  }
}
</style>