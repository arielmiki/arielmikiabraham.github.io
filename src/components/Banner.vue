<template>
     <div id="banner">
         <h1 class="centered">Welcome To My Github Page</h1>
     </div>
</template>

<script>
export default {
  name: "banner"
};
</script>

<style scoped>
#banner {
    min-height: 100vh;
    background: #fff url(https://picsum.photos/1366/768?image=30);
    background-size: cover;
    align-items: center;
}
.centered {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: whitesmoke;
    text-shadow: 2px 2px #000;
    font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 5rem;
    text-align: center;
}

</style>
