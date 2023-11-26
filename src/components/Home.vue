<template>
<main>
 <section  :style="heroStyles" id="home">
       <div class="home-row">
       <h1>Hello, This is <br>Yusubova Shalala<span>.</span></h1>
       <p>I'm a 
       
       
        <Typed :options="options">
    <span class="typing"></span>
                </Typed>
       
       </p>

       
       </div>
   </section>
</main>
   
</template>

<script setup>
import photo from '@/assets/images/hero.png'
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

};

import { Typed } from "@duskmoon/vue3-typed-js";

const options = {
  strings: ["Vue JS Developer", "Designer", "Accountant"],
  loop: true,
  typeSpeed: 100,
};

</script>

<style lang="scss" scoped>

</style>