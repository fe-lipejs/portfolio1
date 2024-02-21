<template>
  <div>
    <div class="container">
      <div class="cont1"></div>
      <div class="cont2">
        <div class="contact-container">
           <div class="ttl-form">Sign In</div>
          <div><input type="text" class="ipt" placeholder="Email" /></div>
          <div><input type="text" class="ipt" placeholder="Password" /></div>
          <div class="button">CONTACTAR</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.ttl-form{
  font-family: "Roboto", sans-serif;
  font-weight: 900;
  font-size: 40px;
  /* font-size: ; */
  line-height: 4vw;
  text-align: center;
}
.container {
  display: grid;
  vertical-align: center;
  align-items: center;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr;
  background-color: #7a34a0;
  padding: 60px;
}
.contact-container {
  background-color: #fff;
  width: 600px;
  height: 700px;
  border-radius: 30px;
  box-shadow: 0px 0px 20px #00000025;
  padding: 50px;
}
.contact-container div {
    margin: 30px;
}
.button {
  margin-top: 100px !important;
  background-color: #64f185;
  color: #fff;
  font-size: 18px;
  font-weight: 900;
  padding: 20px 10px;
  border-radius: 30px;
  cursor: pointer;
}
.button:active {
  background-color: #50dc71;
}
.ipt {
  padding: 20px 40px;
  border-radius: 5px;
  background-color: #ffffff;
  border: 1px solid #a2a2a2;
  border-radius: 10px;
  font-size: 16px;
  color: #333;
  width: 86.5%;
   background: url("../assets/letters1/cadeado.svg");
  background-repeat: no-repeat;
  background-size: 15px 15px;
  background-position: 92% 20px;
}

.ipt::placeholder {
  color: #999999;
  font-size: 18px;
  font-weight: 700;
  /* text-indent: 20px; */
}

.ipt:focus {
  /* outline: none; */
  background-color: #fff;
  outline: 2px solid #4c4c4c;
  /* box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2); */
}
</style>