<script>
export default {
    props: {
        changeAmount: {
            type: Function,
            required: true 
        },
         convert: {
            type: Function,
            required: true 
        }
    }
}


</script>

<template>
  <input type="number" @input="changeAmount($event.target.value)" placeholder="Введите число"><br>
  <button @click="convert()">Конвертировать</button>
</template>

<style scoped>
input {
    outline: none;
    width: 500px;
    position: relative;
    top: -30px;
    font-size: 1.2em;
    border-radius: 3px;
    border:0;
    padding:10px 15px;
}

button {
    padding: 15px 20px;
    color: #fff;
    text-transform: uppercase;
    cursor: pointer;
    background: #fbb606;
    border: 0;
    border-radius: 3px;

}
</style>
