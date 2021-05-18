<template>
  <div id="hello">
    <div id="hello-text">
      <h1>I'm Dominik Kołodziej</h1>
      <button class="white-btn" @click="onScrollToMenu">
        Get to know me
      </button>
    </div>

  </div>
</template>

<script>
export default {
  name: 'Hello',
  methods: {
    onScrollToMenu: function (){
      document.getElementById("appBar").scrollIntoView();
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: white;
  font-size: 64px;
}

#hello {
  /*background-color: #0e9aa7 ;*/
  background: linear-gradient(-45deg, #1f4068, #1b1b2f, #e43f5a);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

#hello-text {
  display: flex;
  flex-direction: column;
  align-items: center;
}

@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}




</style>
