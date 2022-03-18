<template>
  <b-row class="vh-100 vw-100 row-login">
    <b-col class="d-flex justify-content-center align-items-center center-login">
      <div class="col-8" style="align-items: center; display: flex; flex-direction: column">
        <b-form class="formul" style="width: 60%; min-width: 30%;">
          <b-form-group
            label="Nome"
            label-for="name"
            >
              <b-form-input
                id="nome"
                type="name"
                autocomplete="off"
                v-model="form.name"
              ></b-form-input>
            </b-form-group>
 
            <b-form-group
            label="E-mail"
            label-for="email"
            >
              <b-form-input
                id="email"
                type="email"
                autocomplete="off"
                v-model="form.email"
              ></b-form-input>
            </b-form-group>

            <b-form-group
            label="EDV"
            label-for="edv"
            >
              <b-form-input
                id="edv"
                type="input"
                autocomplete="off"
              ></b-form-input>
            </b-form-group>

            <div class="senhas">
              <div class="boxsenha">
              <b-form-group
                label="Senha"
                label-for="password"
              >
  
                <b-form-input
                  id="senha"
                  type="password"
                  v-model="form.password"
                ></b-form-input>
             </b-form-group>
              </div>
              <div class="boxconfirmacao">
              <b-form-group
                label="Confirme"
                label-for="password"
              >
    
                <b-form-input
                  id="confirmacao"
                  type="password"
                  v-model="form.password"
                ></b-form-input>
              </b-form-group>
              </div>
            </div>
            <div class="imagem">
            <label class="d-flex justify-content-between">
                  <b>Imagem de Perfil</b>
                  <div>
                    <b-link href="file:////C:/" style="margin-left: 10px">Escolha um arquivo...</b-link>
                  </div>
                </label>
            
            </div>
            <br>
            <br>
            <b-button
              id="button"
              type="button"
              block>
              <i class="fas fa-sign-in-alt"></i> Login
            </b-button>
 
        </b-form>
      </div>
    </b-col>
  </b-row>
</template>
 
<script>
 
export default {
  data() {
    return {
      form: {
        email: "",
        password: ""
      }
    }
  },
 
  methods: {
    login() {},
 
  }
}
</script>
 
<style>
 
*, /*resetar o estilo da página*/
*::after,
*::before {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
}
 
.row-login {
  margin-left: 0;
}

.formul{
 align-items: center;
 justify-content: center;
}
 
.center-login {
  background-color: #F2F2F2;
}


#nome.form-control{
  background-color: #C4C4C4;
  padding: 2vh;
}

#email.form-control {
  background-color: #C4C4C4;
  padding: 2vh;
}

#edv.form-control{
  background-color: #C4C4C4;
  padding: 2vh;
}

.senhas{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: flex-start;
}

.boxsenha{
  width: 50%;
  padding-right: 2vh;
}

#senha.form-control {
  background-color: #C4C4C4;
  padding: 2vh;
}

.boxconfirmacao{
  padding-left: 2vh;
  width: 50%;
}

#confirmacao.form-control {
  background-color: #C4C4C4;
  padding: 2vh;
}

.imagem{
  justify-content: center;
  display: flex;
}

#button{
  background-color: #757575;
  padding: 1vh;
}

 
</style>