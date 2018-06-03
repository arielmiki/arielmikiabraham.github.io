<template>
    <div id="welcome">
        <div class="text-container">
            <h1 class="title"> {{title}}</h1>
        </div>
    </div>
</template>

<script>
export default {
  name: "welcome",
  data() {
    return {
      title: "Welcome to My Github Project Page",
    };
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Bowlby+One+SC");
#welcome {
  height: 100vh;
  background: url(../assets/image/background.jpg) no-repeat center;
  background-size: cover;
  overflow: hidden;
}

.text-container {
  position: absolute;
  top: 50%;
  left: 50%;
  text-align: center;
  transform: translate(-50%, -50%);
  width: 60vw;
  background: rgba(0.2, 0.2, 0.2, 0.5);
}

.title {
  font-size: 5rem;
  font-family: "Bowlby One SC", cursive;
  color: whitesmoke;
}

@media screen and (max-width: 768px) {
   .title {
       font-size: 2.5rem;
   }
}
</style>
