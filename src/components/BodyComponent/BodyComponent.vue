<template>
  <div>
    <!-- ----------------------------------------------- -->
    <div class="grid-container">
      <div class="item item1">
        <div class="item1-tornado">
          <div>PORT<br />FOLIO</div>
        </div>
        <!-- <div>PORT</div>
        <div>FÓLIO</div> -->
      </div>
      <div class="item item2">
        <div class="sub-item sub-item2-1">Sub Item 1</div>
        <div class="sub-item sub-item2-2"></div>
      </div>
      <div class="item item3">
        <div class="sub-item sub1 sub-item1">
          <div>ABOUT ME</div>
          <div>
            Estudante de Sistemas de Informação na UVV, descobri minha paixão
            pela programação desde cedo, enquanto explorava os desafios
            apresentados pelos deveres de casa do meu irmão. Meu primeiro
            contato foi com C++, a qual dispertou meu interesse e uns anos
            depois minha paixão pela área.
          </div>
        </div>
        <div class="sub-item sub2 sub-item2">2tem</div>
        <div class="sub-item sub3 sub-item3">
          <div style="background-color: #161616" class="sub-sub-item">
            Sub Item 1
          </div>
          <div style="background-color: #ff16da" class="sub-sub-item">
            Sub Item 2
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
  
  <style scoped>
.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 723px 723px;
  width: 100%;
}

.item {
  text-align: center;
}

.item1 {
  font-family: Roboto, sans-serif;
  background-color: #64f185;
  grid-column: 1;
  grid-row: 1;
}
.item1-tornado {
  width: 100%;
  height: 723px;
  /* ------------------------ */
  background: url("../../assets/letters1/tornado.svg");
  background-repeat: no-repeat;
  background-size: 60vw 500px;
  background-position: 0px 250px;
  display: flex;
  justify-content: center;
}
.item1-tornado div {
  margin-top: 40px;
  margin-left: 7vw;
  font-family: "Poppins", sans-serif;
  font-weight: 900;
  font-size: 5vw;
  font-size: ;
  line-height: 4vw;
  text-align: start;
}


.item2 {
  grid-column: 2;
  padding: 0;
  grid-column: 2;
  grid-row: 1 / span 2;
  display: grid;
  grid-template-rows: 723px 723px;
  background: url("../../../public/zendaya.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: -350px 0;
}

.item3 {
  grid-column: 1;
  grid-row: 2;
  display: grid;
  padding: 0;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 500px 223px;
}

.sub-item {
  text-align: center;
  display: grid;
}

.sub-item1 {
  background-color: #60cffe;
  grid-column: 1 / span 2;
  grid-row: 1;
  display: grid;
  justify-content: center;
}
.sub-item1 div {
  text-align: justify;
  width: 24vw;
  margin-left: 18vw;
}
.sub-item1 div:nth-child(1) {
  font-family: "Poppins", sans-serif;
  font-weight: 900;
  font-size: 40px;
  line-height: 125px;
  text-align: start;
}
.sub-item1 div:nth-child(2) {
  margin-top: -100px;
  font-size: 20px;
  font-weight: 500;
}

.item2 .sub-item1 {
}

.sub-item2 {
  background-color: #ffffc1;
  grid-column: 1;
  grid-row: 2;
  /* height: 100px; */
}

.sub-item2-2 {
  background: url("../../assets/letters1/amoeba.svg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: 0px 0;
}

.sub-sub-item {
  /* height: 140px; */
  text-align: center;
}

@media only screen and (max-width: 768px) {
}

/* Media Query para Celulares */
@media only screen and (max-width: 750px) {
  .item {
    /* height: 100vw; */
  }
  .item1 {
    grid-column: 1;
    grid-row: 1;
  }
  .item2 {
    height: auto;
    grid-column: 2;
    grid-row: 1;
    background-position: -20vw 0;
  }
  .item3 {
    grid-column: 1 / span 2;
    grid-row: 2;
    display: grid;
  }

  /* --------------- */

  .sub-item1 {
    /* azul */
    grid-column: 2;
    grid-row: 1 / span 2;
    height: 100%;
  }
  .sub-item2 {
    grid-column: 1;
    grid-row: 2;
  }
  .sub-item3 {
    grid-column: 1;
    grid-row: 1;
  }
}
</style>
  