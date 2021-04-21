<template>
  <div id="app">
    <Card/>
  </div>
</template>

<script>
import Card from './components/Card.vue'

export default {
  name: 'App',
  components: {
    Card
  }
}
</script>

<style>
#app {
    width: 100%;
    font-family: 'Roboto', sans-serif;
}

.cardBody {
    position: absolute;
    width: 499px;
    height: 305px;
    /* left: 729px; */
    top: calc(50% - 305px / 2 - 36.5px);
    background: #131313;
    border-radius: 20px;
}

.iconBackground {
    background-image: url(images/patriciaIcon.png);
    background-size: cover;
    position: relative;
    top: -2.5rem;
    left: -2rem;
    background-repeat: no-repeat;
    height: 21.5rem;
}

.cardContents {
    position: relative;
    left: 5.4rem;
    top: 5.9rem;
}

.passwordEye {
    position: relative;
    left: 17rem;
    background: transparent;
    border: none;
}

input {
    border: none;
    background: transparent;
    color: rgb(255, 255, 255);
    font-style: normal;
    font-weight: normal;
    font-size: 23px;
    line-height: 29px;
    letter-spacing: 0.08em;
}

input:active {
    outline: none;
    border: none;
}

input:focus {
    outline: 0;
}

button:active {
    outline: none;
    border: none;
}

button:focus {
    outline: 0;
}

.passwordText {
    position: relative;
    top: 5rem;
}

.passwordAppendage {
    color: #fff;
    position: relative;
    left: 2rem;
    font-style: normal;
    font-weight: normal;
    font-size: 23px;
    line-height: 29px;
    letter-spacing: 0.08em;
}

.openPasswordAppendage {
    color: #fff;
    position: relative;
    left: 3rem;
    font-style: normal;
    font-weight: normal;
    font-size: 23px;
    line-height: 29px;
    letter-spacing: 0.08em;
}

.footerInfo {
    display: flex;
    color: #fff;
    position: relative;
    top: 8.5rem;
}

.footerRightInfo {
    display: flex;
    color: #fff;
    position: relative;
    left: 16rem;
}

.validDate {
    font-style: normal;
    font-weight: normal;
    font-size: 7px;
    line-height: 8px;
    margin-top: 1rem;
    margin-right: 1rem;
    color: #9da8b6;
}

.cardName {
    position: absolute;
    color: #d3dce6;
}

.ccv {
    font-style: normal;
    font-weight: normal;
    font-size: 7px;
    line-height: 8px;
    color: #9da8b6;
    margin-left: 1rem;
}

#hiddenPassword {
    margin-left: 0.8rem;
}

@media screen and (max-width: 768px) {
.cardBody {
    position: absolute;
    width: 450px;
    height: 305px;
    /* left: 729px; */
    top: calc(50% - 305px / 2 - 36.5px);
    background: #131313;
    border-radius: 20px;
}

.cardContents {
    position: relative;
    left: 4rem;
    top: 5.9rem;
}

.iconBackground {
    background-image: url(/img/patriciaIcon.4c2336dd.png);
    background-size: cover;
    position: relative;
    top: -2rem;
    left: -2rem;
    background-repeat: no-repeat;
    height: 21rem;
}
}

</style>
