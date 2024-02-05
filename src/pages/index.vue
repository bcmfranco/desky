<template>
  <div id="container">

    <div>
      <Brander />
    </div>

    <div id="core">
      <div class="box">
        <a href="https://codev-ar.atlassian.net/jira/software/projects/URG/boards/44/backlog" target="_blank">URG Backlog</a>
      </div>
      <div class="box">
        <a href="https://codev-ar.atlassian.net/jira/software/projects/URG/boards/44" target="_blank">URG Tablero</a>
      </div>
      <div class="box">
        <a href="https://codev-ar.atlassian.net/jira/software/projects/AZ/boards/55/backlog" target="_blank">AZK Backlog</a>
      </div>
      <div class="box">
        <a href="https://codev-ar.atlassian.net/jira/software/projects/AZ/boards/55" target="_blank">AZK Tablero</a>
      </div>
      <div class="box">
        <a href="https://codev-ar.atlassian.net/jira/software/projects/GA/boards/60/backlog" target="_blank">GOF Backlog</a>
      </div>
      <div class="box">
        <a href="https://codev-ar.atlassian.net/jira/software/projects/GA/boards/60" target="_blank">GOF Tablero</a>
      </div>
      <div class="box">
        <a href="https://codev-ar.atlassian.net/jira/servicedesk/projects/SD/queues/custom/2" target="_blank">SD Colas</a>
      </div>
    </div>

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

#core {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
}

.box {
  background-color: #723f78;
  padding: 20px;
  text-align: center;
  border-radius: 8px;
}

a {
  color: #fff;
  text-decoration: none;
  font-size: 18px;
}

@media (max-width: 480px) {
  #container {
    display: flex;
    flex-direction: column;
  }
}


</style>