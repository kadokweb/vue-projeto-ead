<template>
  <section
    id="loginPage"
    :style="{
      backgroundImage: 'url(' + require('@/assets/images/bgLogin.jpg') + ')',
    }"
  >
    <div class="loginContent">
      <div class="loginCard">
        <div
          class="decor"
          style="background-image: url('./assets/images/building.jpg')"
        >
          <div class="content">
            <span class="logo">
              <img :src="require('@/assets/images/logo.svg')" alt="KadokWEb" />
            </span>
            <span class="dots">
              <span></span>
              <span></span>
              <span></span>
            </span>
            <span class="description">
              <p>
                Os melhores e mais completos cursos de Laravel do Brasil, cursos
                com projetos reais. Do zero ao profissional.
              </p>
            </span>
            <span class="copyright fontSmall">
              Todos os Direitos reservados - <b>KadokWEb</b>
            </span>
          </div>
        </div>
        <div class="login">
          <div class="content">
            <!-- <span class="logo">
              <img
                :src="require('@/assets/images/logoDark.svg')"
                alt="KadokWEb"
              />
            </span> -->
            <span style="margin-top: 5rem">
              <h1>Seja muito bem vindo(a)!</h1>
            </span>
            <span class="dots">
              <span></span>
              <span></span>
              <span></span>
            </span>
            <span class="description">
              Acesse nossa plataforma e desfrute de cursos completos para sua
              especialização.
            </span>
            <form action="/dist/index.html" method="">
              <div class="groupForm">
                <input type="email" name="email" placeholder="Email" required />
                <i class="far fa-envelope"></i>
              </div>
              <div class="groupForm">
                <!-- <i class="fa fa-lock"></i> -->

                <input
                  type="password"
                  name="password"
                  placeholder="Senha"
                  required
                />
                <i class="far fa-eye buttom"></i>
              </div>
              <button class="btn primary" type="submit">Login</button>
            </form>
            <span>
              <p class="fontSmall">
                Esqueceu sua senha?
                <router-link
                  :to="{ name: 'forget.password' }"
                  class="link primary"
                  >Clique aqui</router-link
                >
              </p>
            </span>
          </div>
          <span class="copyright fontSmall">
            Todos os Direitos reservados - <b>KadokWEb</b>
          </span>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "Auth",
};
</script>
<style>
</style>