<template>
    <header>
        <h1>Generador de contraseñas</h1>
    </header>
    <div class="main" id="app">
        <input :type="type" class="input" auto="auto" :value="password" />
        <button type="button" class="btn" @click="generatePassword()">
            Generar contraseña
        </button>
    </div>
</template>

<script>
export default {
    props: {
        type: {
            type: String,
            default: 'text',
        },
        size: {
            type: String,
            default: '10',
        },
        characters: {
            type: String,
            default: 'a-z,A-Z,0-9,#',
        },
    },
    data: function() {
        return{
            password: this.value,
        }
    },
    methods: {
        generatePassword () {
            var charactersArray = this.characters.split(',');  
            var CharacterSet = '';
            var password = '';

            if( charactersArray.indexOf('a-z') >= 0)     {
                CharacterSet += 'abcdefghijklmnopqrstuvwxyz';
            }
            if( charactersArray.indexOf('A-Z') >= 0) {
                CharacterSet += 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
            }
            if( charactersArray.indexOf('0-9') >= 0) {
                CharacterSet += '0123456789';
            }
            if( charactersArray.indexOf('#') >= 0) {
                CharacterSet += '![]{}()%&*$#^<>~@|';
            }

            for(var i=0; i < this.size; i++) {
                password += CharacterSet.charAt(Math.floor(Math.random() * CharacterSet.length));
            }
            this.password = password;
        }
    }
}
</script>

<style scoped>

</style>