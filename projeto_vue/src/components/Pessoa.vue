<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{ nome }} </h2>
        <Info :email="email" :esta_trabalhando=false />
        <Form />
    </div>
</template>

<script>
    import Form from './Form'
    import Info from './Info'
    export default {
        name: 'Pessoa',
        components: {
            Info, 
            Form
        },
        data() {
            return {
                nome: 'Nathálya',
                email: 'nath.conta14@gmail.com'
            }
        }
    }
</script>