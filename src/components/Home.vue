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

import photo from '@/assets/images/hero.jpg'
const heroStyles = {
  height: '100vh',
  width: '100%',
  backgroundImage: `url(${photo})`,
  backgroundSize: 'cover',
  backgroundAttachment: 'fixed',
  display: 'flex',
  flexDirection: 'column',
  justifyContent: 'center',
  padding: '70px',
  position: 'relative',
  // box-shadow:'rgba (0, 0, 0 , 20%)'
};



const options = {
  strings: ["Vue JS Developer", "Designer", "Accountant"],
  loop: true,
  typeSpeed: 100,
};

</script>

<style lang="scss" scoped></style>