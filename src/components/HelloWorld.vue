<template>
  <div class="hello">
    <img :src="require('@/assets/logo.png')">
    <svg>
      <g>
        <path d="M 50,100 A 1,1 0 0 1 50,0"/>
      </g>
      <g>
        <path d="M 50,75 A 1,1 0 0 0 50,-25"/>
      </g>
      <defs>
        <linearGradient id="gradient" x1="0%" y1="0%" x2="0%" y2="100%">
          <stop offset="0%" style="stop-color:#FF56A1;stop-opacity:1" />
          <stop offset="100%" style="stop-color:#FF9350;stop-opacity:1" />
        </linearGradient>
      </defs>
    </svg>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
