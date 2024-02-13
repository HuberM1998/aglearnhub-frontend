<template>
  <main>
    <v-row no-gutters>
      <v-col cols="12">
        <div class="home">
          <v-card class="card-home" min-width="500" max-width="500" elevation="16">
            <v-card-title>
              <v-img class="mx-auto" :width="300" aspect-ratio="16/9" cover
                src="../assets/logotipo_aglearnhub.jpg"></v-img>
            </v-card-title>
            <v-card-item>
              <v-text-field label="E-mail" :rules="emailRules"></v-text-field>
              <v-text-field label="Senha" type="password"
                hint="Entre com a sua senha para acessar a plataforma"></v-text-field>
            </v-card-item>
            <p class="login-text-social">
              Faça login com suas redes sociais:
            </p>
            <v-card-item class="footer-login">
              <v-btn color="red-accent-3" class="buttons-footer" prepend-icon="mdi-google">
                Google
              </v-btn>
              <v-btn class="buttons-footer" prepend-icon="mdi-linkedin">
                Linkedin
              </v-btn>
              <v-btn color="blue-darken-2" class="buttons-footer" prepend-icon="mdi-facebook">
                Facebook
              </v-btn>
            </v-card-item>
            <v-card-item>
              <v-btn color="success" class="mt-4" block @click="validate">
                Entrar
              </v-btn>
            </v-card-item>
          </v-card>
        </div>
      </v-col>
    </v-row>
  </main>
</template>

<script>

export default {
  name: 'HomeView'
}
</script>

<style scoped>
.home {
  background: url(../assets/home-bg.jpg);
  height: 100vh;
  width: 100%;
}

.login-text-social{
  font-size: 0.8em;
  color: gray;
}
.card-home {
  float: right;
  margin-top: 10%;
  margin-right: 10%;
}

.footer-login .buttons-footer {
  margin: 10px;
}
</style>
