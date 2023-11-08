<template>
  <div>
    <img src="../../public/images/vite.png" alt="vite">
  </div>
</template>

<script>
export default {
  setup () {
    

    return {}
  }
}
</script>

<style lang="css" scoped>
  @keyframes hover-in {
    0% {
      transform: scale(1);
      box-shadow: none;
    }
    100% {
      transform: scale(1.1);
      box-shadow: 10px 10px 30px #7B36AC80, -10px -10px 30px #33617ACC;
    }
  }
  @keyframes hover-out {
    from {
      transform: scale(1.1);
      box-shadow: 10px 10px 30px #7B36AC80, -10px -10px 30px #33617ACC;
    }
    to {
      transform: scale(1);
      box-shadow: none;
      transition: box-shadow 0.3s ease-in-out;
    }
  }
  img {
      margin-top: 50px;
      width: 50%;
      border: 5px solid transparent;
      border-radius: 50px;
      animation: hover-out 430ms forwards;
  }
  img:hover{
      cursor: pointer;
      animation: hover-in 430ms forwards;
  }
</style>