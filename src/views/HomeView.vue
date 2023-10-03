<template>
  <main>
    <div class="information">
      <img src="/img/perfil.png" alt="profile" class="profile" />
      <p class="name">Théo Lansana</p>
      <p class="about">
        Desde que a tecnologia teve seu ápice, nunca foi tão difícil se
        atualizar, diante de tantas inovações e desafios, aqui vem a pergunta.
      </p>

      <WhatsAppButton tel="5566992824038"> Posso lhe ajudar? </WhatsAppButton>
    </div>

    <div class="menu">
      <p class="text-chanel">Meus Canais</p>
      <ul class="icons">
        <a href="https://instagram.com/theo.lansana"
          ><li><i class="fa-brands fa-instagram"></i></li
        ></a>
        <a href="https://www.github.com/teolando"
          ><li><i class="fa-brands fa-github"></i></li
        ></a>
      </ul>
    </div>
    <p class="rights">© All rights reserved</p>
  </main>
</template>

<script>
import WhatsAppButton from "@/components/WhatsAppButton.vue";

export default {
  components: {
    WhatsAppButton,
  },
};
</script>

<style>
main {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
}

.information {
  width: 830px;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 30px;
  background-color: #212121;
  border-radius: 50px;
  text-align: center;
  color: white;
}

.profile {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  margin-top: 30px;
}

.name {
  color: #0d7377;
  font-size: 24px;
}

.about {
  padding-left: 40px;
  padding-right: 40px;
}

.menu {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 300px;
}

.text-chanel,
.rights {
  color: #ffffff;
  font-size: 24px;
  margin-bottom: 15px;
  margin-top: 15px;
}

.icons {
  width: 265px;
  height: 100px;
  border-radius: 30px;
  background-color: #212121;
  display: flex;
  justify-content: center;
  gap: 40px;
  align-items: center;
}

.icons > a {
  list-style: none;
}

.fa-brands {
  color: #14ffec;
  font-size: 50px;
}

@media only screen and (max-width: 600px) {
  .information {
    width: 100%;
    gap: 15px;
    border-radius: 0;
  }

  .profile {
    width: 140px;
    height: 140px;
  }

  .about {
    padding: 0px 20px;
    font-size: 16px;
  }

  .icons {
    width: 200px;
    height: 70px;
  }

  .fa-brands {
    font-size: 40px;
  }

  .text-chanel,
  .rights {
    font-size: 18px;
    margin-bottom: 10px;
  }
}

@media only screen and (min-width: 600px) {
  .information {
    width: 500px;
  }

  .icons {
    width: 240px;
    height: 90px;
  }

  .fa-brands {
    font-size: 55px;
  }
}

@media only screen and (min-width: 1200px) {
  .information {
    width: 830px;
  }

  .icons {
    width: 300px;
  }
}
</style>
