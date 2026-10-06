<template>
  <section id="contact" class="contact-section">

    <!-- Background -->
    <div class="gold-orbit gold-orbit-one"></div>
    <div class="gold-orbit gold-orbit-two"></div>
    <div class="gold-glow gold-glow-top"></div>
    <div class="gold-glow gold-glow-bottom"></div>

    <div class="contact-container">

      <!-- Header -->
      <div class="contact-header">

        <div class="section-label">
          <span>LET'S CONNECT</span>
          <span class="label-line"></span>
        </div>

        <h2 class="contact-title">
          Let's Build Something
          <span>Together</span>
        </h2>

        <p class="contact-intro">
          Have a project in mind or looking for a developer to work with?
          I’d love to hear about it. Feel free to reach out through any
          of the platforms below or send me a message directly.
        </p>

      </div>

      <!-- Contact Grid -->
      <div class="contact-grid">

        <!-- Left Contact Card -->
        <div class="contact-left">

          <div class="contact-card">

            <h3 class="card-title">
              GET IN TOUCH
            </h3>

            <a
              href="mailto:cristinofrancemadali@gmail.com"
              class="contact-row"
            >
              <div class="contact-icon">
                <i class="bi bi-envelope"></i>
              </div>

              <div class="contact-row-content">
                <span>EMAIL</span>
                <strong>cristinofrancemadali@gmail.com</strong>
              </div>

              <i class="bi bi-arrow-up-right row-arrow"></i>
            </a>

            <a
              href="https://github.com/roxbraga"
              target="_blank"
              rel="noopener noreferrer"
              class="contact-row"
            >
              <div class="contact-icon">
                <i class="bi bi-github"></i>
              </div>

              <div class="contact-row-content">
                <span>GITHUB</span>
                <strong>github.com/roxbraga</strong>
              </div>

              <i class="bi bi-arrow-up-right row-arrow"></i>
            </a>

            <a
              href="https://www.linkedin.com/in/cristino-madali-596450296"
              target="_blank"
              rel="noopener noreferrer"
              class="contact-row"
            >
              <div class="contact-icon">
                <i class="bi bi-linkedin"></i>
              </div>

              <div class="contact-row-content">
                <span>LINKEDIN</span>
                <strong>linkedin.com/in/cristino-madali-596450296</strong>
              </div>

              <i class="bi bi-arrow-up-right row-arrow"></i>
            </a>

            <div class="availability">

              <div class="availability-header">
                <span class="status-dot"></span>
                <span>AVAILABLE FOR</span>
              </div>

              <div class="availability-tags">
                <span>Freelance</span>
                <span>Remote Work</span>
                <span>Full-time</span>
                <span>Collaboration</span>
              </div>

            </div>

          </div>

        </div>

        <!-- Right Message Form -->
        <div class="contact-right">

          <div class="form-card">

            <div class="form-header">

              <div class="form-icon">
                <i class="bi bi-send"></i>
              </div>

              <div>
                <span class="form-label">
                  START A CONVERSATION
                </span>

                <h3>
                  Send me a message
                </h3>
              </div>

            </div>

            <form @submit.prevent="submitForm">

              <div class="form-row">

                <div class="input-group">

                  <label for="contact-name">
                    Name
                  </label>

                  <input
                    id="contact-name"
                    v-model="form.name"
                    type="text"
                    placeholder="Your name"
                    autocomplete="name"
                    required
                  />

                </div>

                <div class="input-group">

                  <label for="contact-email">
                    Email
                  </label>

                  <input
                    id="contact-email"
                    v-model="form.email"
                    type="email"
                    placeholder="your@email.com"
                    autocomplete="email"
                    required
                  />

                </div>

              </div>

              <div class="input-group">

                <label for="contact-subject">
                  Subject
                </label>

                <input
                  id="contact-subject"
                  v-model="form.subject"
                  type="text"
                  placeholder="What can I help you with?"
                  required
                />

              </div>

              <div class="input-group">

                <label for="contact-message">
                  Message
                </label>

                <textarea
                  id="contact-message"
                  v-model="form.message"
                  placeholder="Tell me about your project..."
                  required
                ></textarea>

              </div>

              <button
                type="submit"
                class="submit-btn"
                :disabled="isSubmitting"
              >

                <template v-if="!isSubmitting">

                  <i class="bi bi-send"></i>
                  <span>Send Message</span>
                  <i class="bi bi-arrow-right"></i>

                </template>

                <template v-else>

                  <span class="spinner"></span>
                  <span>Sending...</span>

                </template>

              </button>

            </form>

          </div>

        </div>

      </div>

      <!-- Footer -->
      <footer class="contact-footer">

        <div class="footer-info">

          <strong>
            © 2026 Cristino France Madali
          </strong>

          <span>
            Backend / Full-Stack Web Developer
          </span>

        </div>

        <div class="footer-links">

          <a
            href="https://github.com/roxbraga"
            target="_blank"
            rel="noopener noreferrer"
          >
            <i class="bi bi-github"></i>
            <span>GitHub</span>
          </a>

          <span class="footer-divider"></span>

          <a
            href="https://www.linkedin.com/in/cristino-madali-596450296"
            target="_blank"
            rel="noopener noreferrer"
          >
            <i class="bi bi-linkedin"></i>
            <span>LinkedIn</span>
          </a>

          <span class="footer-divider"></span>

          <a href="mailto:cristinofrancemadali@gmail.com">
            <i class="bi bi-envelope"></i>
            <span>Email</span>
          </a>

          <button
            type="button"
            class="back-to-top"
            aria-label="Back to top"
            @click="scrollToTop"
          >
            <i class="bi bi-arrow-up"></i>
          </button>

        </div>

      </footer>

    </div>

  </section>
</template>

<script setup>
import { ref } from "vue";
import { Notyf } from "notyf";
import "notyf/notyf.min.css";

const WEB3FORMS_ACCESS_KEY =
  "ccbb74f7-4ceb-4247-b533-c7a8807ccd29";

const form = ref({
  name: "",
  email: "",
  subject: "",
  message: ""
});

const isSubmitting = ref(false);

const notyf = new Notyf({
  duration: 3500,
  position: {
    x: "right",
    y: "top"
  },
  dismissible: true
});

const submitForm = async () => {
  if (isSubmitting.value) {
    return;
  }

  isSubmitting.value = true;

  try {
    const response = await fetch(
      "https://api.web3forms.com/submit",
      {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
          Accept: "application/json"
        },
        body: JSON.stringify({
          access_key: WEB3FORMS_ACCESS_KEY,
          name: form.value.name,
          email: form.value.email,
          subject: form.value.subject,
          message: form.value.message,
          from_name: form.value.name,
          replyto: form.value.email
        })
      }
    );

    const result = await response.json();

    if (result.success) {
      notyf.success("Message sent successfully!");

      form.value = {
        name: "",
        email: "",
        subject: "",
        message: ""
      };
    } else {
      notyf.error(
        "Something went wrong. Please try again."
      );
    }
  } catch (error) {
    console.error(
      "Contact form error:",
      error
    );

    notyf.error(
      "Unable to send your message. Please try again."
    );
  } finally {
    isSubmitting.value = false;
  }
};

const scrollToTop = () => {
  window.scrollTo({
    top: 0,
    behavior: "smooth"
  });
};
</script>

<style scoped>
.contact-section {
  position: relative;
  min-height: 100vh;
  padding: 55px 0 0;
  background: #050505;
  overflow: hidden;
}

.contact-container {
  position: relative;
  z-index: 2;
  width: min(943px, calc(100% - 40px));
  margin: 0 auto;
}

.gold-orbit {
  position: absolute;
  border: 1px solid rgba(212, 175, 55, 0.12);
  border-radius: 50%;
  pointer-events: none;
}

.gold-orbit-one {
  width: 720px;
  height: 350px;
  top: -165px;
  right: -210px;
  transform: rotate(-25deg);
}

.gold-orbit-two {
  width: 650px;
  height: 300px;
  bottom: -170px;
  left: -250px;
  transform: rotate(27deg);
}

.gold-glow {
  position: absolute;
  width: 320px;
  height: 320px;
  border-radius: 50%;
  filter: blur(100px);
  pointer-events: none;
}

.gold-glow-top {
  top: -170px;
  right: -80px;
  background: rgba(212, 175, 55, 0.07);
}

.gold-glow-bottom {
  bottom: -180px;
  left: -100px;
  background: rgba(212, 175, 55, 0.04);
}

.contact-header {
  width: 48%;
  margin-bottom: 42px;
}

.section-label {
  display: flex;
  align-items: center;
  gap: 13px;
  margin-bottom: 12px;
}

.section-label span:first-child {
  color: #D4AF37;
  font-size: 0.65rem;
  font-weight: 700;
  letter-spacing: 3px;
}

.label-line {
  width: 76px;
  height: 1px;
  background: #D4AF37;
  opacity: 0.65;
}

.contact-title {
  margin: 0 0 13px;
  color: #F5F5F5;
  font-size: clamp(2.7rem, 4.3vw, 4.15rem);
  font-weight: 700;
  line-height: 0.98;
  letter-spacing: -2px;
}

.contact-title span {
  display: block;
  color: #D4AF37;
}

.contact-intro {
  width: 100%;
  max-width: 430px;
  margin: 0;
  color: #a7a7a7;
  font-size: 0.86rem;
  line-height: 1.6;
}

.contact-grid {
  display: grid;
  grid-template-columns: 1fr 1.02fr;
  gap: 17px;
  align-items: stretch;
}

.contact-left,
.contact-right {
  display: flex;
  align-self: stretch;
}

.contact-card,
.form-card {
  width: 100%;
  height: 405px;
  box-sizing: border-box;
  border: 1px solid rgba(212, 175, 55, 0.22);
  border-radius: 10px;
}

.contact-card {
  padding: 19px 21px;
  background: rgba(8, 8, 8, 0.72);
}

.card-title {
  margin: 0 0 13px;
  color: #D4AF37;
  font-size: 0.68rem;
  font-weight: 700;
  letter-spacing: 3px;
}

.contact-row {
  display: flex;
  align-items: center;
  gap: 14px;
  min-height: 58px;
  border-bottom: 1px solid rgba(212, 175, 55, 0.09);
  color: inherit;
  text-decoration: none;
  transition:
    transform 0.25s ease,
    border-color 0.25s ease;
}

.contact-row:hover {
  transform: translateX(3px);
  border-color: rgba(212, 175, 55, 0.25);
}

.contact-icon {
  width: 40px;
  height: 40px;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #D4AF37;
  background: rgba(212, 175, 55, 0.03);
  border: 1px solid rgba(212, 175, 55, 0.22);
  border-radius: 8px;
  font-size: 0.95rem;
}

.contact-row-content {
  display: flex;
  flex-direction: column;
  gap: 3px;
  min-width: 0;
}

.contact-row-content span {
  color: #707070;
  font-size: 0.57rem;
  font-weight: 600;
  letter-spacing: 2px;
}

.contact-row-content strong {
  color: #d0d0d0;
  font-size: 0.73rem;
  font-weight: 500;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.row-arrow {
  margin-left: auto;
  color: #666;
  font-size: 0.78rem;
}

.contact-row:hover .row-arrow {
  color: #D4AF37;
}

.availability {
  padding-top: 18px;
}

.availability-header {
  display: flex;
  align-items: center;
  gap: 9px;
  margin-bottom: 11px;
  color: #d0d0d0;
  font-size: 0.68rem;
  font-weight: 500;
}

.status-dot {
  width: 6px;
  height: 6px;
  border-radius: 50%;
  background: #D4AF37;
  box-shadow: 0 0 0 4px rgba(212, 175, 55, 0.07);
}

.availability-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 7px;
}

.availability-tags span {
  padding: 6px 12px;
  color: #a7a7a7;
  border: 1px solid rgba(212, 175, 55, 0.22);
  border-radius: 999px;
  font-size: 0.63rem;
}

.form-card {
  padding: 20px 21px 22px;
  background: rgba(8, 8, 8, 0.76);
}

.form-header {
  display: flex;
  align-items: center;
  gap: 13px;
  margin-bottom: 16px;
}

.form-icon {
  width: 45px;
  height: 45px;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #D4AF37;
  background: rgba(212, 175, 55, 0.03);
  border: 1px solid rgba(212, 175, 55, 0.22);
  border-radius: 8px;
}

.form-label {
  display: block;
  margin-bottom: 3px;
  color: #707070;
  font-size: 0.57rem;
  font-weight: 600;
  letter-spacing: 2px;
}

.form-header h3 {
  margin: 0;
  color: #F5F5F5;
  font-size: 1.15rem;
  font-weight: 600;
}

.form-row {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 15px;
}

.input-group {
  display: flex;
  flex-direction: column;
  gap: 6px;
  margin-bottom: 11px;
}

.input-group label {
  color: #b8b8b8;
  font-size: 0.65rem;
}

.input-group input,
.input-group textarea {
  width: 100%;
  box-sizing: border-box;
  color: #F5F5F5;
  background: #0a0a0a;
  border: 1px solid rgba(212, 175, 55, 0.15);
  border-radius: 5px;
  outline: none;
  font-family: inherit;
  font-size: 0.7rem;
}

.input-group input {
  height: 38px;
  padding: 0 12px;
}

.input-group textarea {
  height: 96px;
  min-height: 96px;
  padding: 10px 12px;
  resize: none;
  line-height: 1.5;
}

.input-group input::placeholder,
.input-group textarea::placeholder {
  color: #555;
}

.input-group input:focus,
.input-group textarea:focus {
  border-color: rgba(212, 175, 55, 0.5);
  box-shadow: 0 0 0 3px rgba(212, 175, 55, 0.04);
}

.submit-btn {
  width: 100%;
  height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  color: #080808;
  background: #D4AF37;
  border: 1px solid #D4AF37;
  border-radius: 6px;
  font-family: inherit;
  font-size: 0.7rem;
  font-weight: 600;
  cursor: pointer;
  transition:
    background 0.25s ease,
    transform 0.25s ease,
    box-shadow 0.25s ease;
}

.submit-btn:hover:not(:disabled) {
  background: #E3C15A;
  border-color: #E3C15A;
  transform: translateY(-2px);
  box-shadow: 0 8px 20px rgba(212, 175, 55, 0.15);
}

.submit-btn:disabled {
  opacity: 0.65;
  cursor: not-allowed;
}

.spinner {
  width: 12px;
  height: 12px;
  border: 2px solid rgba(8, 8, 8, 0.3);
  border-top-color: #080808;
  border-radius: 50%;
  animation: spin 0.7s linear infinite;
}

@keyframes spin {
  to {
    transform: rotate(360deg);
  }
}

.contact-footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  margin-top: 38px;
  padding: 18px 0 22px;
  border-top: 1px solid rgba(212, 175, 55, 0.12);
}

.footer-info {
  display: flex;
  flex-direction: column;
  gap: 4px;
}

.footer-info strong {
  color: #dcdcdc;
  font-size: 0.7rem;
  font-weight: 500;
}

.footer-info span {
  color: #707070;
  font-size: 0.63rem;
}

.footer-links {
  display: flex;
  align-items: center;
  gap: 15px;
}

.footer-links a {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  color: #999;
  text-decoration: none;
  font-size: 0.65rem;
  transition: color 0.25s ease;
}

.footer-links a:hover {
  color: #D4AF37;
}

.footer-links a i {
  font-size: 0.82rem;
}

.footer-divider {
  width: 1px;
  height: 15px;
  background: rgba(212, 175, 55, 0.15);
}

.back-to-top {
  width: 39px;
  height: 39px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 10px;
  color: #D4AF37;
  background: transparent;
  border: 1px solid rgba(212, 175, 55, 0.4);
  border-radius: 50%;
  cursor: pointer;
  transition:
    color 0.25s ease,
    background 0.25s ease,
    transform 0.25s ease;
}

.back-to-top:hover {
  color: #080808;
  background: #D4AF37;
  transform: translateY(-2px);
}

@media (max-width: 991px) {
  .contact-section {
    padding-top: 70px;
  }

  .contact-container {
    width: min(700px, calc(100% - 40px));
  }

  .contact-header {
    width: 100%;
    margin-bottom: 30px;
  }

  .contact-grid {
    grid-template-columns: 1fr;
    align-items: start;
  }

  .contact-left,
  .contact-right {
    display: block;
  }

  .contact-card,
  .form-card {
    height: auto;
  }

  .contact-footer {
    margin-top: 50px;
  }
}

@media (max-width: 576px) {
  .contact-section {
    padding-top: 65px;
  }

  .contact-container {
    width: calc(100% - 30px);
  }

  .contact-title {
    font-size: 2.65rem;
    letter-spacing: -1.5px;
  }

  .contact-intro {
    font-size: 0.8rem;
  }

  .form-row {
    grid-template-columns: 1fr;
    gap: 0;
  }

  .contact-card,
  .form-card {
    padding: 20px;
  }

  .contact-footer {
    align-items: flex-start;
    flex-direction: column;
  }

  .footer-links {
    flex-wrap: wrap;
  }

  .footer-divider {
    display: none;
  }

  .gold-orbit-one {
    right: -450px;
  }

  .gold-orbit-two {
    left: -450px;
  }
}
</style>