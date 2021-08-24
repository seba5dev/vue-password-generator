<template>
    <h1>Generador con modulo</h1>
    <p>{{ password }}</p>
</template>

<script>
import 'custom-password-generator';
export default {
    data:{
        generator: require('custom-password-generator'),
        password: {
            randomPassword:{
                length: 10, // Number : length of the password
                useNumbers: false, // Boolean : put numbers on the password
                useLetters: {
                    lowercase: false, // Boolean : use lowercase letters
                    uppercase: true // Boolean : use uppercase letters
                }, // False or object with lowercase and uppercase
                useSymbols: true // Boolean : put symbols in the password
            }
        }
    }
}
</script>

<style>

</style>