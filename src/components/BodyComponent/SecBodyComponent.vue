<template>
  <div>
    <div class="container">
      <div class="title">
        <div>EXPE<br />RIENCE<span style="color: rgb(24, 189, 255);">.</span></div>
      </div>
      <div class="figures"></div>
      <div class="texto">
        Como estudante de Sistemas de Informação na Universidade de Vila Velha,
        trago habilidades sólidas em programação. Domino linguagens como
        JavaScript, essencial para o desenvolvimento web, e frameworks como
        Vue.js para construir interfaces dinâmicas.
        <br /><br />
        Além disso, estou confortável com Node.js no desenvolvimento do
        back-end, garantindo a integridade e eficiência dos sistemas.[ Minha
        experiência acadêmica inclui projetos práticos que aprimoraram minhas
        habilidades. Com Vue.js, criei interfaces envolventes e intuitivas,
        enquanto Node.js me permitiu desenvolver APIs robustas para suportar
        sistemas complexos. Estou ansioso para aplicar essas habilidades no
        mercado de trabalho, contribuindo para soluções inovadoras e eficazes.
        Determinado a aprender continuamente e acompanhar as tendências, estou
        preparado para enfrentar desafios e me destacar.
        <br /><br />
        Com minha paixão pela programação e dedicação à excelência, estou
        confiante em minha capacidade de agregar valor a qualquer equipe e
        impulsionar o sucesso da organização.
      </div>
    </div>
  </div>
</template>

<style scoped>
*{
    font-family: "Poppins", sans-serif;
}
.container {
  display: grid;
  justify-content: center;
  grid-template-rows: 0.7fr 1fr;
  grid-template-columns: 1fr 1fr;
  padding-top: 200px;
  padding-inline: 15vw;

}
.title {
  grid-column: 1 / span 2;
  margin: 0 auto;
  font-weight: 900;
  font-size: 100px;
  line-height: 100px;
  text-align: start;
  
}
.figures {
  border-right-color: red;
  width: 380px;
  height: 700px;
  background: url("../../assets/letters1/figures.svg");
  /* background-repeat: no-repeat;
  background-size: 0vw 0px;
  background-position: 0px 0px;*/
}
.texto {
  font-size: 22px;
  color: black;
  text-align: start;
}
</style>