<template>
<div class="teste" >
  <b-row class="vh-100 vw-100 row-login">
    <b-col class="d-flex justify-content-start background-color-red align-items-center center-login">
      <div class="col-8 vw-10" style="align-items: center; display: flex; flex-direction: column; background-color: blue">
        <b-form class="formul" style="width: 60%;">
          <b-form-group
            label="Nome Completo"
            label-for="name"
            >
              <b-form-input
                id="nome"
                type="name"
                autocomplete="off"
              ></b-form-input>
            </b-form-group>
 
            <b-form-group>
              <label class="d-flex justify-content-between">
                CPF
              </label>
 
              <b-form-input
                id="CPF"
              ></b-form-input>
            </b-form-group>

             <b-form-group>
              <label class="d-flex justify-content-between">
                Data de Nascimento
              </label>
 
              <b-form-input
                id="datanasc"
                type="date"
              ></b-form-input>
            </b-form-group>

             <b-form-group>
              <label class="d-flex justify-content-between">
                Turma
              </label>
 
              <b-form-input
                id="turma"
                type="list"
              ></b-form-input>
            </b-form-group>
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
      <div class="teste2" style="background-color: red">
        <img href="C:\Users\lab10\Desktop\FrontEnd-CadastroCandidato\cadastro_candidato\src\media\imgperfil.jpg"/>
      </div>
    </b-col>
  </b-row>
</div>
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

.d-flex justify-content-center align-items-center center-login{
background-color: blue;
display: flex-start;
flex-direction: column;
align-items: left;
}

.center-login {
  background-color: #F2F2F2;
}

#email.form-control {
  background-color: #C4C4C4;
  padding: 2vh;
}
#password.form-control {
  background-color: #C4C4C4;
  padding: 2vh;
}

#button{
  background-color: #757575;
  padding: 1vh;
}


 
</style>