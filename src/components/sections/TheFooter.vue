<script setup></script>

<template>
  <footer>
    <div class="redes">
      <img src="@/assets/images/instagram.svg" alt="Instagram" />
      <img src="@/assets/images/linkedin.svg" alt="LinkedIn" />
      <img src="@/assets/images/correo.svg" alt="Correo" />
      <img src="@/assets/images/behance.svg" alt="Behance" />
    </div>

    <div>
      <img class="logo" src="@/assets/images/azula.svg" alt="Logo" />
    </div>
  </footer>
</template>

<style scoped>
footer {
  height: 100px;
  background-color: var(--primary-second);
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 300px;
}

.redes {
  display: flex;
  justify-content: start;
  align-items: center;
  gap: 30px;
  margin-left: 70px;
}

.redes > img {
  width: 40px;
}

.logo {
  width: 200px;
}
</style>
