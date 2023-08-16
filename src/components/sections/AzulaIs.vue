<script setup></script>

<template>
  <section>
    <p class="text--style-3">Azula<span class="text--style-2">is</span></p>

    <div class="animation--container text--style">
      <p class="fade--in" id="fi1">a Photographer</p>
      <p class="fade--in" id="fi2">an Artist</p>
      <p class="fade--in" id="fi3">a Designer</p>
      <p class="fade--in" id="fi4">an Illustrator</p>
    </div>
  </section>
</template>

<style scoped>
.azula > img {
  width: 70%;
}

section {
  height: 400px;
  margin: 70px 0 0 70px;
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

.text--style-2 {
  font-size: 130px;
  font-family: Didot, serif;
  color: var(--primary-second);
  text-align: left;
  opacity: 80%;
  margin-left: 40px;
}

.text--style-3 {
  font-size: 130px;
  font-family: Didot;
  font-weight: italic;
  color: var(--primary-third);
  text-align: left;
  opacity: 70%;
}

.text--style {
  font-size: 130px;
  font-family: Didot, italic;
  color: var(--primary-first);
  text-align: right;
  margin-left: 350px;
}
</style>
