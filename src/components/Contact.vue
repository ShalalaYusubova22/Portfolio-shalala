<template>
<main>
  <section id="contact">
    <h1 class="sub-heading">Contact</h1>
    <div class="divider"></div>
    <p class="sub-para">
     You can contact with me by Phone & by sending mail...
    </p>

    <div class="contact-row">
      <div class="contact-left">
        <div class="icon-box">
          <div class="icon"><i class="fa-solid fa-envelope"></i></div>
          <div class="info">
            <h4>Email:</h4>
            <p>shelale2205@gmail.com</p>
          </div>
        </div>

        <div class="icon-box">
          <div class="icon"><i class="fa-solid fa-phone"></i></div>
          <div class="info">
            <h4>Call:</h4>
            <p>+998 94 0810002</p>
          </div>
        </div>

        <div class="icon-box">
          <div class="icon"><i class="fa-solid fa-location"></i></div>
          <div class="info">
            <h4>Location:</h4>
            <p>Tashkent ,Uzbekistan / Baku, Azerbaijan</p>
          </div>
        </div>

        <div class="map">
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2997.1685392433933!2d69.2621950765688!3d41.3051970010886!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38ae8b2020878009%3A0x90f60f5cf233ff60!2z0JrQvtGB0LzQvtC90LDQstGC0L7Qsg!5e0!3m2!1sru!2s!4v1695989956494!5m2!1sru!2s"
            width="100%"
            height="250"
            style="border: 0"
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          ></iframe>
        </div>
      </div>

      <div class="contact-right">
        <form action="">
          <input type="text" name="name" id="name" placeholder="Your Name" />
          <input
            type="email"
            name="email"
            id="email"
            placeholder="Your Email"
          />
          <input
            type="text"
            name="subject"
            id="subject"
            placeholder="Subject"
          />
          <textarea
            name="msg"
            id="msg"
            rows="9"
            placeholder="Your Message"
          ></textarea>
          <input type="submit" value="Send Message" />
        </form>
      </div>
    </div>
  </section>
</main>
</template>

<script setup></script>

<style lang="scss" scoped></style>
