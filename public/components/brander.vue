<template>

  <div id="gumcom_brander">
    <div id="logotype">
      <div>DE</div>
    </div>
    <div id="isotype">
      <h1>desky</h1>
      <h2>virtual desk organizer</h2>
      <Navbarr />
    </div>
  </div>


</template>


<style scoped>

  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

  #gumcom_brander{
    font-family: Roboto;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-items: center;
    margin: 10px 0px;
  }

  #gumcom_brander #logotype{
    font-size: 25px;
    color: #dedede;
    width: 50px; /* Ajusta el ancho según tus necesidades */
    height: 50px; /* Ajusta la altura según tus necesidades */
    border: 2px solid #c4c4c4; /* Color del borde */
    border-radius: 8px; /* Ajusta el radio del borde según tus necesidades */
    box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.1); /* Añade una sombra */
    margin: 10px;
  }

  #gumcom_brander #isotype h1 {
    color: #dedede;
    margin: 0px;
    padding: 0px;
  }
  
  #gumcom_brander #isotype h2 {
    font-size: 24px;
    color: #dedede;
    margin-bottom: 20px;
    margin: 0px;
    padding: 0px;
  }


  @media (max-width: 480px) {

    #gumcom_brander{
      flex-direction: column;
      align-items: start;
    }


  }




</style>