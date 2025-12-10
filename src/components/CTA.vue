<template>
  <section class="cta">
    <div class="cta-content">
      <h2>Ready to Share Your Package?</h2>
      <p>Join a few of developers building the future of open-source software.</p>
      <button class="btn btn-cta">Publish Now</button>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped>
.cta {
  background: linear-gradient(135deg, #f26727, #f07237);
  color: #000;
  padding: 5rem 2rem;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.cta::before {
  content: '';
  position: absolute;
  top: -50%;
  right: -10%;
  width: 400px;
  height: 400px;
  background: rgba(0, 0, 0, 0.1);
  border-radius: 50%;
  pointer-events: none;
}

.cta::after {
  content: '';
  position: absolute;
  bottom: -50%;
  left: -10%;
  width: 400px;
  height: 400px;
  background: rgba(0, 0, 0, 0.1);
  border-radius: 50%;
  pointer-events: none;
}

.cta-content {
  max-width: 800px;
  margin: 0 auto;
  position: relative;
  z-index: 2;
}

.cta-content h2 {
  font-size: 2.5rem;
  font-weight: 800;
  margin: 0 0 1rem 0;
  line-height: 1.2;
}

.cta-content p {
  font-size: 1.1rem;
  margin: 0 0 2rem 0;
  opacity: 0.95;
  line-height: 1.6;
}

.btn-cta {
  background-color: #000;
  color: #ff8c00;
  border: 2px solid #000;
  padding: 1rem 2.5rem;
  border-radius: 6px;
  font-weight: 700;
  font-size: 1.05rem;
  cursor: pointer;
  transition: all 0.3s ease;
}

.btn-cta:hover {
  background-color: transparent;
  color: #000;
  transform: translateY(-3px);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
}

@media (max-width: 768px) {
  .cta {
    padding: 3rem 1.5rem;
  }

  .cta-content h2 {
    font-size: 2rem;
  }

  .cta-content p {
    font-size: 1rem;
  }
}
</style>
