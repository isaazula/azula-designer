<script setup></script>

<template>
  <footer>
    <div class="redes footer__nav item__1">
      <img src="/images/instagram.svg" alt="Instagram"/>
      <img src="/images/linkedin.svg" alt="LinkedIn" />
      <img src="/images/correo.svg" alt="Correo" />
      <img src="/images/behance.svg" alt="Behance" />
    </div>

    <div class="footer__copy item__2">
      <p>All rights reserved © 2023 | Isabella Azula Tovar</p>
    </div>
    
    <img class="logo item__3" src="/images/azula.svg" alt="Logo" />
    
  </footer>
</template>

<style scoped>
footer {
  height: 100px;
  background-color: var(--primary-second);
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: 1fr 30px;
  align-items: center;
}

.redes {
  display: flex;
  gap: 30px;
  margin: 30px 0 0 70px;

}

.redes > img {
  width: 40px;
}

.logo {
  width: 200px;
}

.footer__copy > p {
  margin: 0%;
  font-family: "Playfair Display", serif;
  font-size: 16px;
  text-align: center;
  color: aliceblue;
}

.item__2 {
  margin-bottom: 35px;
  grid-column:2/3;
  grid-row: 2;
}

.item__3{
  margin: 25px 70px 0 0;
  grid-row: 1;
  grid-column: 3;
  justify-self: end;
}

</style>
