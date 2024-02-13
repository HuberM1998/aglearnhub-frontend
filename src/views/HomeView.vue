<template>
  <main>
    <v-row no-gutters>
      <v-col cols="12">
        <div class="home">
          <div class="card-container">
            <v-card class="card-home" min-width="500" max-width="500" elevation="16">
              <v-card-title>
                <v-img class="mx-auto" :width="300" aspect-ratio="16/9" cover
                  src="../assets/logotipo_aglearnhub.png"></v-img>
              </v-card-title>
              <v-card-item>
                <v-text-field label="E-mail" :rules="emailRules"></v-text-field>
                <v-text-field label="Senha" type="password"
                  hint="Entre com a sua senha para acessar a plataforma"></v-text-field>
              </v-card-item>
              <p class="login-text-social">
                Faça login com suas redes sociais:
              </p>
              <v-card-item>
                <v-btn color="red-accent-3" class="ma-1" prepend-icon="mdi-google">
                  Google
                </v-btn>
                <v-btn class="ma-1" prepend-icon="mdi-linkedin">
                  Linkedin
                </v-btn>
                <v-btn color="blue-darken-2" class="ma-1" prepend-icon="mdi-facebook">
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
  display: flex;
  justify-content: center; 
  align-items: center;
}

.login-text-social {
  font-size: 0.8em;
  color: gray;
}

.card-home {
  margin: -40% auto auto 0;
  background: rgb(255,255,255,0.5);
}
</style>
