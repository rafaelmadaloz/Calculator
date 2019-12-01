<template>
    <div id="app">
        <Calculator />
    </div>
</template>

<script>

import Calculator from './main/Calculator'

export default {
    components: { Calculator }
}
</script>

<style>

@import url('https://fonts.googleapis.com/css?family=Roboto+Mono:300,300i,400,500&display=swap');

* {
    font-family: "Roboto Mono", monospace;
    font-weight: 300;
}

body {
    margin: 0;
    
}

#app {
    display: flex;
    flex-direction: column;
    height: 100vh;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: #fff;
    background: linear-gradient(to right, #304352, #d7d2cc);
}

</style>