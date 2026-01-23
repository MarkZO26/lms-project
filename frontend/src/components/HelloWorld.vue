<script setup>
defineProps({
  msg: String,
})
</script>

<template>
  <div class="container">
    <!-- Navbar -->
    <nav class="navbar">
      <h1 class="logo">{{ msg }}</h1>
      <div class="nav-links">
        <a href="/login" class="btn-outline">Login</a>
        <a href="/register" class="btn">Register</a>
        <a href="/I love You" class="btn">I love YOu</a>
      </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
      <h2 class="hero-title">Learn. Grow. Achieve.</h2>
      <p class="hero-subtitle">
        Explore our courses and start your journey today. Master new skills, track progress, and succeed in your learning goals.
      </p>
      <div class="hero-buttons">
        <a href="/courses" class="btn">Explore Courses</a>
        <a href="/register" class="btn-outline">Get Started</a>
      </div>
    </section>

    <!-- Features Section -->
    <section class="features">
      <h3>Why Choose Our LMS?</h3>
      <div class="feature-cards">
        <div class="card">
          <h4>Wide Course Selection</h4>
          <p>Hundreds of courses covering multiple topics to boost your skills and knowledge.</p>
        </div>
        <div class="card">
          <h4>Track Progress</h4>
          <p>Monitor your learning journey with progress tracking and achievements.</p>
        </div>
        <div class="card">
          <h4>Accessible Anywhere</h4>
          <p>Learn anytime, anywhere with our web-based platform that works on all devices.</p>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
      <p>© 2026 My LMS. All rights reserved.</p>
    </footer>
  </div>
</template>

<style scoped>
/* --- Reset & Base --- */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

/* Container */
.container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

/* Navbar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 50px;
  background-color: #ffffff;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
}

.logo {
  color: #2c3e50;
  font-size: 24px;
  font-weight: bold;
}

.nav-links a {
  margin-left: 15px;
  padding: 10px 20px;
  border-radius: 5px;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
}

.nav-links .btn {
  background-color: #3498db;
  color: white;
  border: none;
}

.nav-links .btn:hover {
  background-color: #2980b9;
}

.nav-links .btn-outline {
  border: 2px solid #3498db;
  color: #3498db;
}

.nav-links .btn-outline:hover {
  background-color: #3498db;
  color: white;
}

/* Hero Section */
.hero {
  flex: 1;
  background: linear-gradient(135deg, #3498db, #8e44ad);
  color: white;
  text-align: center;
  padding: 100px 20px;
}

.hero-title {
  font-size: 48px;
  font-weight: 800;
  margin-bottom: 20px;
}

.hero-subtitle {
  font-size: 20px;
  max-width: 700px;
  margin: 0 auto 40px auto;
  line-height: 1.5;
}

.hero-buttons a {
  margin: 0 10px;
  padding: 12px 25px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
}

.hero-buttons .btn {
  background-color: white;
  color: #3498db;
}

.hero-buttons .btn:hover {
  background-color: #ecf0f1;
}

.hero-buttons .btn-outline {
  border: 2px solid white;
  color: white;
}

.hero-buttons .btn-outline:hover {
  background-color: white;
  color: #3498db;
}

/* Features Section */
.features {
  background-color: #f7f7f7;
  padding: 80px 20px;
  text-align: center;
}

.features h3 {
  font-size: 32px;
  font-weight: bold;
  margin-bottom: 50px;
  color: #2c3e50;
}

.feature-cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 30px;
}

.card {
  background-color: white;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  padding: 30px 20px;
  max-width: 300px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
}

.card h4 {
  font-size: 20px;
  margin-bottom: 10px;
  color: #3498db;
}

.card p {
  font-size: 16px;
  color: #555;
  line-height: 1.4;
}

/* Footer */
.footer {
  background-color: #2c3e50;
  color: white;
  text-align: center;
  padding: 20px;
  font-size: 14px;
}
</style>
