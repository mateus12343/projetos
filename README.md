* soft reset do css */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

}

body {
  /background-image: url('https://img.freepik.com/fotos-gratis/parede-de-estudio-gradiente-de-ouro-amarelo-abstrato-de-luxo-bem-como-uso-como-plano-de-fundo-layout-banner-e-apresentacao-do-produto_1258-63544.jpg?w=2000');*/max-width:;
  background-color: orange;
  background-size: auto 100vh; 
  font-family: Arial;
  height: 100vh;
}
/*se a tela tiver pelo menos 400px vai carregar estes estilos */
@media (min-width: 400px) {
  body {
    font-size: 14px;
  }
}

/* breakpoint*/
@media (min-width: 600px) {
  body {
    font-size: 18px;
  }
}

/* breakpoint*/
@media (min-width: 1200px) {
  body {
    font-size: 20px;
  }
}

header {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

h1 {
  margin:  -30px;
  padding: 0px;
}

.menu {
  background-color: darkgreen;
  position: fixed;
  width: 100vw;
  top: 0;
  z-index: 1;
}

.menu ul {
  display: flex;
  justify-content: space-around;
}

.menu li {
 list-style: none; 
}

.menu a {
  display: block;
  padding: 10px 20px;
  color: aliceblue;
  transition: background-color 1s, color 1s;

}

.menu a:hover {
  background-color: aliceblue;
  color: darkgreen;
}

.menu a:active {
  background-color: black;
  color: greenyellow;
}

a {
  color: black;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

.titulo {
  transform: scale(0.2)  translateY(50vh);
  opacity: 0;

  animation: 1s linear 2s animacaoTitulo forwards;
}

@keyframes animacaoTitulo {

  100% {
    transform: scale(1)  translateY(0);
    opacity: 1;

  }
}
.sobre,
.sub-sub-title,
.site-subtitle,
.site-title {
  color: darkgreen;
  text-align: center;
  margin-left: auto;
  margin-right: auto;
}

.site-title {
  font-size: 4em;
  font-family: 'Gloria Hallelujah', cursive;
}

.site-subtitle {
 font-style: bolde;
 font-family: 'Dancing Script', cursive;
 /* font-family: 'Press Start 2P', cursive; */
 line-height: 1.5em;
 font-size: 3em;
}

.sub-sub-title {
 font-style: bolde;
 font-family: 'Dancing Script', cursive;
 /* font-family: 'Press Start 2P', cursive; */
 line-height: 1.5em;
 font-size: 2em;
 margin-top: 100px;
}

.sobre,
.contato,
.portfolio {
  padding: 2em;
  margin-bottom: 5em;
  text-align: center;
  /*min-height: 100vh;*/
}

@media (min-width: 1200px) {
  .container {
    margin-left: auto;
    margin-right: auto;
    max-width: 1200px;
  }
}

.sobre h2,
.contato h2,
.portfolio h2 {
  color: darkgreen;
  font-family: 'Press Start 2P', cursive;
  margin-bottom: 2em;
  padding-top: 2em;
  font-size: 2em;
}

.sobre p {
  font-style: normal;
  font-family: 'Dancing Script', cursive;
  /* font-family: 'Press Start 2P', cursive; */
  line-height: 1.5em;
  font-size: 1.2em;
  text-indent: 1.5em;
  margin-bottom: 1.2em;
}

.sobre .avatar {
  float: right;
  margin-left: 2em;
  text-align: justify;
  clip-path: polygon(100% 0%, 75% 50%, 100% 100%, 25% 100%, 0% 50%, 25% 0%);
}

.portfolio figcaption {
  color: whitesmoke;
}

.img-sobre {
  height: 310px;
  width: 310px;
}

.img-portfolio {
  height: 180px;
  width: 100%;
  object-fit: cover;
  object-position: left bottom;
  border-radius: 0%;
  transition: transform 500 ms ;
}

/* .img-portfolio:hover {
  transform: scale(1.2) rotate3d(0, 0, 1, 10deg);
} */

.card {
  background-color: darkgreen;
  position: relative;
}

.card-front, 
.card-back {
  position: absolute;
  top:  0;
  left: 0;
}

.card-back {
  background-color: red;
  height: 180px;
  width: 100%;
}

.contato .icon {
  text-align: center;

}

.contato a {
  color: darkgreen;
  font-size: 4em;
  margin-right: 40px;
  transition: text-shadow 1s;
}

.contato a:hover {
  text-decoration: none;
  text-shadow: 0px 0px 10px rgba(255, 255, 255, 1.0);
}

.contato h3 {
  color: darkgreen;
  margin-top: 2em;
  font-size: 1.7em;
}

.contato h4 {
  color: darkgreen;
  margin: 2em;
  font-size: 1.3em;
}

.portfolio .grid { /* grid do portfolio */
  display: grid;
  gap: 2em;
  margin-left: auto;
  margin-right: auto;
}

@media (min-width: 560px) {
  .portfolio .grid {
    grid-template-columns: 240px 240px;
    justify-content: center;
  }
}

@media (min-width: 880px) {
  .portfolio .grid {
    grid-template-columns: repeat(3, 240px);
    justify-content: center;
   /* height: calc(100vh - 2em - 48px - 2em);*/
  }
}

@media (min-width: 1200px) {
 .img-portfolio {
  height: 180px;
  width: auto;
}
Footer
© 2022 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
