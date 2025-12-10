<template>
  <section id="features" class="features">
    <div class="features-container">
      <h2 class="section-title">Why Choose reefs.io?</h2>
      <p class="section-subtitle">Powerful features designed for developers</p>

      <div class="features-grid">
        <div class="feature-card">
          <div class="feature-icon">🚀</div>
          <h3>Lightning Fast</h3>
          <p>Global CDN with blazing-fast package delivery to developers worldwide.</p>
        </div>

        <div class="feature-card">
          <div class="feature-icon">🔒</div>
          <h3>Secure by Default</h3>
          <p>Enterprise-grade security with package scanning and vulnerability detection.</p>
        </div>

        <div class="feature-card">
          <div class="feature-icon">📊</div>
          <h3>Analytics</h3>
          <p>Track downloads, get insights, and monitor your package performance in real-time.</p>
        </div>

        <div class="feature-card">
          <div class="feature-icon">🌐</div>
          <h3>Open Source</h3>
          <p>Built on open standards. Publish any type of package or library.</p>
        </div>

        <div class="feature-card">
          <div class="feature-icon">⚙️</div>
          <h3>Easy Integration</h3>
          <p>Simple CLI and API for seamless publishing and package management.</p>
        </div>

        <div class="feature-card">
          <div class="feature-icon">👥</div>
          <h3>Community Driven</h3>
          <p>Join a few of developers sharing and collaborating on amazing projects.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.features {
  background-color: #fff;
  padding: 6rem 2rem;
}

.features-container {
  width: 100%;
  padding: 0 2rem;
}

.section-title {
  font-size: 2.5rem;
  font-weight: 800;
  text-align: center;
  color: #000;
  margin: 0 0 0.5rem 0;
}

.section-subtitle {
  text-align: center;
  color: #666;
  font-size: 1.1rem;
  margin: 0 0 3rem 0;
}

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 2rem;
}

.feature-card {
  background: #f9f9f9;
  border: 2px solid #f0f0f0;
  border-radius: 10px;
  padding: 2rem;
  text-align: center;
  transition: all 0.3s ease;
  position: relative;
  overflow: hidden;
}

.feature-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 3px;
  background: linear-gradient(90deg, #f26727, #f07237);
  transform: translateX(-100%);
  transition: transform 0.3s ease;
}

.feature-card:hover {
  border-color: #f26727;
  box-shadow: 0 10px 30px rgba(255, 140, 0, 0.1);
  transform: translateY(-5px);
}

.feature-card:hover::before {
  transform: translateX(0);
}

.feature-icon {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  display: inline-block;
}

.feature-card h3 {
  font-size: 1.3rem;
  color: #000;
  margin: 1rem 0;
  font-weight: 700;
}

.feature-card p {
  color: #666;
  line-height: 1.6;
  margin: 0;
  font-size: 0.95rem;
}

@media (max-width: 768px) {
  .features {
    padding: 3rem 1.5rem;
  }

  .section-title {
    font-size: 2rem;
  }

  .features-grid {
    grid-template-columns: 1fr;
  }
}
</style>
