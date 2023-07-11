<script setup></script>

<template>
  <footer>
    <div class="redes">
      <img src="" alt="Instagram" />
      <img src="" alt="LinkedIn" />
      <img src="" alt="Correo" />
    </div>

    <div>
      <img src="" alt="Logo" />
    </div>
  </footer>
</template>

<style scoped>
footer {
  height: 100px;
  background-color: var(--primary-second);
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
}

.redes {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}
</style>
