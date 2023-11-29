<template>
  <main>
    <section id="home">
      <div class="home-img">
        <img src="@/assets/images/hero.jpg" class="hero-img-web" />
        <img src="@/assets/images/hero-second.jpg" class="hero-img-mobile" />


        <div class="home-row">
          <h1>Hello, This is <br>Yusubova Shalala<span>.</span></h1>
          <p>I'm a


            <Typed :options="options">
              <span class="typing"></span>
            </Typed>

          </p>


        </div>
      </div>



      
    </section>
  </main>
</template>

<script setup>
import { Typed } from "@duskmoon/vue3-typed-js";




const options = {
  strings: ["Vue JS Developer", "Designer", "Accountant"],
  loop: true,
  typeSpeed: 100,
};

</script>

<style lang="scss" scoped></style>