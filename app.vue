<template>
  <div class="container">
    <div class="logo">
      <svg width="200" height="120" viewBox="0 0 200 120">
        <!-- Lock -->
        <g transform="translate(20, 10)">
          <rect x="10" y="40" width="60" height="50" rx="10" fill="none" stroke="#fff" stroke-width="5"/>
          <path d="M25 40 V 25 C25 15 55 15 55 25 V 40" fill="none" stroke="#fff" stroke-width="5"/>
          <circle cx="40" cy="65" r="5" fill="#fff"/>
        </g>

        <!-- Key -->
        <g transform="translate(100, 0)">
          <circle cx="50" cy="25" r="15" fill="none" stroke="#fff" stroke-width="5"/>
          <line x1="50" y1="40" x2="50" y2="80" stroke="#fff" stroke-width="5"/>
          <path d="M50 70 L 60 70 L 60 80" fill="none" stroke="#fff" stroke-width="5"/>
        </g>
      </svg>
    </div>
    <h1>pkix.io is coming soon</h1>
    <p>We're building something awesome. Stay tuned.</p>
  </div>
</template>

<style>
@font-face {
  font-family: 'JetBrains Mono Nerd Font';
  src: url('/fonts/JetBrainsMonoNerdFont-Regular.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: 'JetBrains Mono Nerd Font';
  src: url('/fonts/JetBrainsMonoNerdFont-Bold.ttf') format('truetype');
  font-weight: bold;
  font-style: normal;
}

body {
  font-family: 'JetBrains Mono Nerd Font', monospace;
  color: #ffffff;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  margin: 0;
  background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
}

@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}

.container {
  text-align: center;
}

@keyframes levitate {
  0% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-20px);
  }
  100% {
    transform: translateY(0px);
  }
}

.logo {
  margin-bottom: 2rem;
  animation: levitate 3s ease-in-out infinite;
}

h1 {
  font-size: 4rem;
  font-weight: 700;
  margin-bottom: 1rem;
  text-shadow: 0 0 10px rgba(0,0,0,0.5);
}

p {
  font-size: 1.5rem;
  color: #eeeeee;
  text-shadow: 0 0 5px rgba(0,0,0,0.5);
}
</style>