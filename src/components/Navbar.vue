
<template>
  <header>
    <div class="profile">
      <img src="@/assets/images/profile-img.jpg" alt="" width="150px">
      <h1>Y Shalala</h1>
    </div>

    <button ref="MenuBtn" @click="toggleMobileNav">Toggle Mobile Nav</button>
    
    <nav>
      <ul>
        <li>
          <a href="#home" :class="{ 'active': activeLink === 'home' }">
            <i class="fa-solid fa-house"></i> Home
          </a>
        </li>
        <li>
          <a href="#about" :class="{ 'active': activeLink === 'about' }">
            <i class="fa-solid fa-user"></i> About
          </a>
        </li>
        <li>
          <a href="#portfolio" :class="{ 'active': activeLink === 'portfolio' }">
            <i class="fa-solid fa-briefcase"></i> Portfolio
          </a>
        </li>
        <li>
          <a href="#service" :class="{ 'active': activeLink === 'service' }">
            <i class="fa-solid fa-server"></i> Services
          </a>
        </li>
        <li>
          <a href="#contact" :class="{ 'active': activeLink === 'contact' }">
            <i class="fa-solid fa-envelope"></i> Contact
          </a>
        </li>
      </ul>
    </nav>

    <div class="footer">
      <p>&copy; Copyright 2023 <br>Designed By Y.Sh</p>
    </div>
  </header>
</template>

<script setup>


import { ref, onMounted, onBeforeUnmount } from 'vue';

const MenuBtn = ref(null);
const activeLink = ref('home');

const toggleMobileNav = () => {
  document.body.classList.toggle('mobile-nav-active');
};

const handleScroll = () => {
  const scrollPos = window.scrollY + 20;
  const sectionIds = ['home', 'about', 'portfolio', 'service', 'contact'];

  for (const sectionId of sectionIds) {
    const section = document.getElementById(sectionId);
    if (!section) continue;

    if (scrollPos > section.offsetTop && scrollPos < section.offsetTop + section.offsetHeight) {
      activeLink.value = sectionId;
    }
  }
};

onMounted(() => {
  window.addEventListener('scroll', handleScroll);
});

onBeforeUnmount(() => {
  window.removeEventListener('scroll', handleScroll);
});


</script>


<style>

</style>