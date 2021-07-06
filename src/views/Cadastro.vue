<template>
    <div>
        <h4>Rota Pai</h4>
        <input type="text" name="email" id="email" placeholder="Email..."><br>
        <input type="text" class="button" name="senha" id="senha" placeholder="******"><br>
        <button id='button'>Testar</button>
        <h4>{{parametroDaRota}}</h4>
        <router-view/>
    </div>
</template>

<script>

export default {
    created(){
       // this.parametroDaRota = this.$route.params.dado
    },
    data(){
        return{
            parametroDaRota: "Nada"
        }
    }
}

</script>



<style scoped>
#button{
    margin-top: 0.5%
}
.button{
    margin-top: 0.5%
}

</style>