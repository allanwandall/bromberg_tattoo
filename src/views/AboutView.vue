<template>
  <div class="about-view">
    <div class="hero">
      <h1>About Us</h1>
    </div>
    <div class="content">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed sit amet
        nulla auctor, vestibulum magna sed, convallis ex. Cum sociis natoque
        penatibus et magnis dis parturient montes, nascetur ridiculus mus.
      </p>
      <p>
        Cras mattis consectetur purus sit amet fermentum. Cum sociis natoque
        penatibus et magnis dis parturient montes, nascetur ridiculus mus.
        Maecenas faucibus mollis interdum. Aenean lacinia bibendum nulla sed
        consectetur.
      </p>
      <p>
        Donec ullamcorper nulla non metus auctor fringilla. Cum sociis natoque
        penatibus et magnis dis parturient montes, nascetur ridiculus mus.
        Maecenas faucibus mollis interdum. Aenean lacinia bibendum nulla sed
        consectetur.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutView',
}
</script>

<style scoped>
.about-view {
  max-width: 800px;
  margin: 40px auto;
  padding: 20px;
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.hero {
  background-color: #333;
  color: #fff;
  padding: 20px;
  text-align: center;
  border-radius: 10px 10px 0 0;
}

.hero h1 {
  margin-top: 0;
}

.content {
  padding: 20px;
}

.content p {
  margin-bottom: 20px;
}
</style>
