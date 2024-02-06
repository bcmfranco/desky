<template>
  <div id="container">

    <div>
      <Brander />
    </div>

    <div id="shelf">
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
      <div class="box">
        <a href="https://bitbucket.org/codev1/workspace/overview/" target="_blank">BITBUCKET</a>
      </div>
      <div class="box">
        <a href="https://docs.google.com/spreadsheets/d/1KBwLndLSXm_ip4CD-5xr32FZ3hr1br4lmnjHwUONvQM/edit" target="_blank">URG HORAS</a>
      </div>
      <div class="box">
        <a href="https://docs.google.com/spreadsheets/d/1oqgH_ci9RvHELqBD1pF0tuaLtrpA2ZjtU9gNAPM84Ew/edit#gid=1922020271" target="_blank">AZK HORAS</a>
      </div>
    </div>

  </div>
</template>

<script>

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
  background: rgb(159,48,162);
  background: linear-gradient(129deg, rgba(159,48,162,1) 0%, rgba(67,115,156,1) 52%);
}

#shelf {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  margin-top: 30px;
}

.box {
  background-color: #723f78;
  padding: 20px;
  border-radius: 8px;
  width: 150px;
  height: 40px;
  line-height: 40px;
  text-align: center;
}

a {
  text-decoration: none;
  font-size: 18px;
  color: #fff;
}

@media (max-width: 480px) {
  #container {
    display: flex;
    flex-direction: column;
    margin-top: unset;
  }

  .box{
    width: 150px;
    height: 75px;
    padding: 0px;
    margin: 0px;
    line-height: 75px;
  }
}


</style>