<template>
    <h1>Contador de ovejas</h1>
    <form @submit.prevent="onSubmit">
        <input type="text" name="number" v-model="add">
        <input type="submit" value="Sumar" >
    </form>  
    <h3>Acumulador de ovejas: {{numberOfSheeps}}</h3>
    <h3 v-if="numberOfSheeps == 100" style="color:red;">Ojo! Has llegado a las 100 ovejas</h3>
</template>

<script>
export default {

    data(){

        return{
            numberOfSheeps: 0,
            add: '',
        }

    },
    methods:{

        onSubmit(){

            this.numberOfSheeps+= Number(this.add);

        }

    }

}
</script>

<style>

</style>