<script setup></script>

<template>
  <section>
    <div>
      <p class="text--style-2">Azula is&nbsp;</p>
    </div>
    <div class="animation--container text--style">
      <p class="fade--in" id="fi1">a Designer</p>
      <p class="fade--in" id="fi2">an Artist</p>
      <p class="fade--in" id="fi3">a Photographer</p>
      <p class="fade--in" id="fi4">an Illustrator</p>
    </div>
  </section>
</template>

<style scoped>
.azula > img {
  width: 70%;
}

section {
  height: 500px;
  margin: 100px 0 80px 0;
}

@keyframes moveFade {
  0% {
    z-index: 0;
    opacity: 0;
    transform: translateX(100px);
  }

  15% {
    opacity: 1;
  }

  25% {
    opacity: 1;
    transform: translateX(0px);
  }

  35% {
    opacity: 0;
  }
  100% {
    opacity: 0;
    transform: translateX(0px);
  }
}

/* Applying the animation to a div */
.fade--in {
  opacity: 0;
  animation: moveFade 6s ease-in infinite;
  transform: translateX(100px);
}

#fi1 {
  animation-delay: 1.5s;
}

#fi2 {
  animation-delay: 3s;
}

#fi3 {
  animation-delay: 4.5s;
}

#fi4 {
  animation-delay: 6s;
}

.animation--container {
  width: 1000px;
}

.animation--container > p {
  position: absolute;
}

.text--style-1 {
  font-size: 400px;
  font-family: "Italiana", serif;
  color: var(--primary-first);
  opacity: 30%;
  text-align: right;
  margin-right: 100px;
  padding: 0px;
}

.text--style-2 {
  font-size: 150px;
  font-family: "Italiana", serif;
  color: var(--primary-second);
  text-align: right;
  margin-top: 0px;
  padding: 0px;
}

.text--style {
  font-size: 150px;
  font-family: "Italiana", serif;
  color: var(--primary-third);
  text-align: center;
}
</style>
