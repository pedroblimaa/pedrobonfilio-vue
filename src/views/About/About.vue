<template>
  <div class="about">
    <div class="block main-block">
      <div class="main-card">
        My name is Pedro Bonfilio Lima, I'm a Full-Stack developer, currently
        attending control and automation course . Please have a seat, scroll
        down, and I'll get you a coffee.
      </div>
    </div>
    <div class="block img-block">
      <div class="description-card">
        <div class="about-text">
          <p>
            I'm a Brazilian <strong> Web Developer </strong>currently in Santa
            Rita do Sapucaí, MG.
          </p>
          <p>
            Originally from <strong>Poço Fundo, MG</strong>, I moved to Santa
            Rita to study Control and Automation Engeneering, wich appeared to
            be the best carrer for my personal taste!
          </p>
        </div>
      </div>
      <div class="about-img">
        <img src="../../assets/me.png" alt="" />
      </div>
    </div>
    <div class="block hobbies-block">
      <div class="hobbies-card">
        <h1 class="hobbies-title">3 of my hobbies.</h1>
        <div class="hobbies">
          <div class="hobbie">
            <img class="hobbie-icon" src="../../assets/icons/guitar.svg" alt="">
            <p>
              I love music, I try to play whenever i have a litte time gap
              between my activities.
            </p>
          </div>
          <div class="hobbie">
            <img class="hobbie-icon" src="../../assets/icons/games.svg" alt="">
            <p>
              Games always have been a great entertainment to me, since kid I
              prefer to play rather then watch tv.
            </p>
          </div>
          <div class="hobbie">
            <img class="hobbie-icon" src="../../assets/icons/pulling-up.svg" alt="">
            <p>
              Some exercises are good to heath and bring happiness, try
              Calisthenics you will not regret it.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import "../../assets/me.png";

export default {
  name: "About",
};
</script>

<style scoped src="./About.css">
</style>
