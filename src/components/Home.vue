<template>
  <div class="home">
    <main id="home">
      <h1 class="lg-heading">
        Rikesh 
        <span class="text-secondary"> Maharjan</span>
      </h1>
      <h2 class="sm-heading">
        Web Developer
      </h2>
      <div class="icons">
        <a href="https://www.facebook.com/rikesh.maharjan.568" target="_blank">
          <font-awesome-icon :icon="['fab', 'facebook']" size="2x" />
        </a>
        <a href="https://www.linkedin.com/in/rikesh-maharajan-998759169/" target="_blank">
          <font-awesome-icon :icon="['fab', 'linkedin']" size="2x" />
        </a>
        <a href="https://github.com/Rikesh1" target="_blank">
          <font-awesome-icon :icon="['fab', 'github']" size="2x" />
        </a>
        <a href="https://www.instagram.com/rikesh_mhjn/" target="_blank">
          <font-awesome-icon :icon="['fab', 'instagram']" size="2x" />
        </a>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>
