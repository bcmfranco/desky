<template>
  <div id="container">

    <div>
      <Brander />
    </div>

    <div>core</div>

  </div>
</template>

<script>

// Poner todo el header dentro de un componente, y la navbarr adentro

import Brander from '../../public/components/brander.vue';

export default {
  components: {
    Brander
  },
  data() {
    return {

    };
  },
  computed: {
  }
};
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@400;700&display=swap');

#container{
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: 1fr;
  align-items: center;
  justify-items: center;
  height: 100vh;
  font-family: Nunito;
}

#calculator_form {
  display: flex;
  flex-direction: column;
  max-width: 400px;
  margin: 0 auto;
}

#calculator_form h2{
  color: #26a69a;
}

#isotype h1 {
  color: #26a69a;
  margin: 0px;
  padding: 0px;
}

#isotype h2 {
  font-size: 24px;
  color: #26a69a;
  margin-bottom: 20px;
  margin: 0px;
  padding: 0px;
}

label {
  font-size: 16px;
  color: #26a69a;
  margin-bottom: 8px;
}

input {
  font-size: 16px;
  padding: 10px;
  border: 1px solid #26a69a;
  border-radius: 4px;
  margin-bottom: 20px;
  width: 100%;
  box-sizing: border-box;
}

input[disabled] {
  background-color: #f5f5f5;
}

button {
  font-size: 16px;
  padding: 10px 20px;
  background-color: #26a69a;
  color: #fff;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #00796b;
}

@media (max-width: 480px) {
  #container {
    display: flex;
    flex-direction: column;
  }

  #container #brand{
    /* grid-template-columns: 1fr; */

    display: flex;
    flex-direction: column;
  }
}


</style>