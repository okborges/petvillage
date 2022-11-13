<template>
  <footer class="p-4">
    <div class="container mx-auto px-6 grid lg:grid-cols-3 items-center">
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
            <img
              src="~/assets/icons/face.svg"
              alt="Facebook"
              width="33"
              height="32"
            />
          </a>
          <a href="https://www.instagram.com/_petvillage_/" target="_blank">
            <img
              src="~/assets/icons/insta.svg"
              alt="Instagram"
              width="34"
              height="33"
            />
          </a>
          <a href="https://wa.me/5511981287333" target="_blank">
            <img
              src="~/assets/icons/zap.svg"
              alt="Whatsapp"
              width="33"
              height="32"
            />
          </a>
        </div>
      </div>

      <iframe
        title="Google Maps"
        class="mt-3"
        src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d7308.761102809774!2d-46.529490574640306!3d-23.662345229542996!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x120da4947b31fdd!2sPet%20Village%20Dermatologia%20e%20Alergologia%20Veterin%C3%A1ria!5e0!3m2!1spt-BR!2sbr!4v1667577561968!5m2!1spt-BR!2sbr"
        width="310"
        height="200"
        style="border-radius: 0.5rem"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
footer {
  background-color: #ff457e;
  color: #40111f;
  font-weight: 600;
  h1 {
    font-family: 'Fraunces';
    font-weight: 600;
    font-size: 2.5rem;
  }
}
</style>
