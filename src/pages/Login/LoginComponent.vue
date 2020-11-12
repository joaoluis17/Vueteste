<template>
    <div class="login">
        <form @submit,prevent="submit" class="login-box">
            <div class="card">
                <div class="card-header">Login</div>
                <div class="card-body">
                    <div class="form-group">
                        <input required type="email" class="form-control" placeholder="E-mail">
                    </div>
                    <div class="form-group">
                        <input required type="password" class="form-control" placeholder="Senha">
                    </div>

                    <button class="btn btn-primary d-block" @click="submit">
                        Entrar
                    </button>
                </div>
            </div>
        </form>
    </div> 
</template>

<script>
export default {
  name: 'LoginComponent',
  
  data: () => ({
      form:{
          email: "",
          password: ""
      }
  }),
  methods: {
      submit(){
          this.$router.push({name: 'home'});
      }
  }
}
</script>

<style scoped lang="css">
.login{	
    background-color: transparent;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
}
    .login-box{
        height: 24rem;
    }

    .card{
        border-style: solid;	
        border-color: #6b46c1;
        border-radius: 0.5rem;
        width: 24rem;
        height: 12rem;
    }
    .card-header{
    color: #68d391;
    font-size: 1rem;	    
    margin-top: 1%;
    margin-left: 2%;
    }
</style>