<template>
  <footer class="p-4">
    <div class="container mx-auto px-6 grid lg:grid-cols-2 items-center">
      <div>
        <h1>contato</h1>
        <p>R. Cel. Agenor de Camargo, 57 - Centro, Santo André</p>
        <div class="block sm:flex">
          <p class="mr-3">Whatsapp: (11) 9 8128-7333</p>
          <p>tel: (11) 4427-8776</p>
        </div>
        <p>Seg a Sex - 09:00 às 17:30</p>
        <p>Sábado - 09:00 às 17:00</p>
        <p>Domingo - FECHADO</p>
      </div>

      <div>
        <h1 class="pb-3">Mídias</h1>
        <div class="flex gap-5">
          <a href="https://www.facebook.com/Petvilage" target="_blank">
            <img src="~/assets/icons/face.svg" alt="" />
          </a>
          <a href="https://www.instagram.com/_petvillage_/" target="_blank">
            <img src="~/assets/icons/insta.svg" alt="" />
          </a>
          <a href="https://wa.me/5511981287333" target="_blank">
            <img src="~/assets/icons/zap.svg" alt="" />
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
footer {
  background-color: #ff457e;
  color: #ffffff;
  h1 {
    font-family: 'Fraunces';
    font-weight: 600;
    font-size: 40px;
  }
}
</style>
