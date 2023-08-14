# CSS_Animation_snippet

/* Animation */

.desktop-nav {
  animation: fadeDown 1000ms forwards;
  opacity: 0;
}

@keyframes fadeDown {
  from {
    opacity: 0;
    transform: translateY(-20px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.hero-container .left p {
  animation: fadeIn 800ms forwards;
  opacity: 0;
  animation-delay: 400ms;
}

@keyframes fadeIn {
  to {
    opacity: 1;
  }
}

.hero-container .left h1 {
  animation: fadeToRight 800ms forwards cubic-bezier(0.22, 0.32, 0, 1.54);
  opacity: 0;
  animation-delay: 800ms;
}

@keyframes fadeToRight {
  from {
    opacity: 0;
    transform: translateX(-100px);
  }

  to {
    opacity: 1;
    transform: translateX(0);
  }
}

.hero-container .left .btn:nth-of-type(1) {
  animation: fadeIn 1000ms forwards;
  opacity: 0;
  animation-delay: 1400ms;
}

.hero-container .left .btn:nth-of-type(2) {
  animation: fadeIn 1000ms forwards;
  opacity: 0;
  animation-delay: 1600ms;
}

.hero-container .right {
  animation: fadeToLeft 1200ms forwards;
  opacity: 0;
  animation-delay: 900ms;
}

@keyframes fadeToLeft {
  from {
    transform: translateX(30px);
  }

  to {
    opacity: 1;
    transform: translateX(0);
  }
}

.hero-container .polygon,
.hero-container .polygon2,
.hero-container .polygon3 {
  opacity: 0;
  animation-name: fadeIn, rotate;
  animation-duration: 800ms, 80s;
  animation-delay: 1800ms;
  animation-iteration-count: 1, infinite;
  animation-fill-mode: forwards;
  animation-timing-function: ease-in, linear;
}

@keyframes rotate {
  from {
    transform: rotate(360deg);
  }
  to {
    transform: rotate(0deg);
  }
}
