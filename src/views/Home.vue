<template>
  <div class="home">

    <img style="width: 200px" alt="Vue logo" src="../assets/logo.png">
    <div style="margin-bottom: 100px">
      <b>Sedia</b>
      <hr>
      <b>Frozen food :</b>
      Dinsum,
      Pastel,
      Risol mayo,
      Sambosa
      <br>
      <b>PO :</b>
      Ayam woku,
      Timus,
      Kue Sagu
      <hr>
    </div>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <div>
      <a href="https://api.whatsapp.com/send?phone=6287788698906&text=Halo,%20saya%20mau%20pesan%20makanan%20Wan%20Ipeh%0ANama:%0AAlamat:%0ANo.HP:%0AJumlah:"><button class="learn-more">Whatsapp</button></a>
      <a href="https://www.instagram.com/dapur.wanipeh/"><button class="instagram">Instagram</button></a>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
<style scoped lang="scss">
  @import url('https://fonts.googleapis.com/css?family=Rubik:700&display=swap');

  $bg: #fff;
  $text: #382b22;
  $light-pink: #fff0f0;
  $pink: #ffe9e9;
  $dark-pink: #f9c4d2;
  $pink-border: #b18597;
  $pink-shadow: #ffe3e2;

  * {
    box-sizing: border-box;
    &::before, &::after {
      box-sizing: border-box;
    }
  }

  body {
    font-family: 'Rubik', sans-serif;
    font-size: 1rem;
    line-height: 1.5;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0;
    min-height: 100vh;
    background: $bg;
  }

  button {
    position: relative;
    display: inline-block;
    cursor: pointer;
    outline: none;
    border: 0;
    vertical-align: middle;
    text-decoration: none;
    font-size: inherit;
    font-family: inherit;
    &.learn-more {
      font-weight: 600;
      color: $text;
      text-transform: uppercase;
      padding: 1em 1.5em;
      background: $light-pink;
      border: 2px solid $pink-border;
      border-radius: 0.75em;
      transform-style: preserve-3d;
      transition: transform 150ms cubic-bezier(0, 0, 0.58, 1), background 150ms cubic-bezier(0, 0, 0.58, 1);
      &::before {
        position: absolute;
        content: '';
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: #42b983;
        border-radius: inherit;
        transform: translate3d(0, 0.75em, -1em);
        transition: transform 150ms cubic-bezier(0, 0, 0.58, 1), box-shadow 150ms cubic-bezier(0, 0, 0.58, 1);
      }
      &:hover {
        background: $pink;
        transform: translate(0, 0.25em);
        &::before {
          transform: translate3d(0, 0.5em, -1em);
        }
      }
      &:active {
        background: $pink;
        transform: translate(0em, 0.75em);
        &::before {
          transform: translate3d(0, 0, -1em);
        }
      }
    }
    &.instagram {
      font-weight: 600;
      color: $text;
      text-transform: uppercase;
      padding: 1em 1.5em;
      background: $light-pink;
      border: 2px solid $pink-border;
      border-radius: 0.75em;
      transform-style: preserve-3d;
      transition: transform 150ms cubic-bezier(0, 0, 0.58, 1), background 150ms cubic-bezier(0, 0, 0.58, 1);
      &::before {
        position: absolute;
        content: '';
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: $dark-pink;
        border-radius: inherit;
        transform: translate3d(0, 0.75em, -1em);
        transition: transform 150ms cubic-bezier(0, 0, 0.58, 1), box-shadow 150ms cubic-bezier(0, 0, 0.58, 1);
      }
      &:hover {
        background: $pink;
        transform: translate(0, 0.25em);
        &::before {
          transform: translate3d(0, 0.5em, -1em);
        }
      }
      &:active {
        background: $pink;
        transform: translate(0em, 0.75em);
        &::before {
          transform: translate3d(0, 0, -1em);
        }
      }
    }
  }
</style>
