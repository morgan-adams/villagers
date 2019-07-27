<template>
  <div id="card" v-if="display">
    <div id="villager-image"><img :src=img></div>
    <div id="species">{{ species }}</div>
    <div id="name">{{ name }}</div>
  </div>
</template>

<script>
  export default {
    name: "VillagerCard",
    props: {
      name: String,
      img: String,
      species: String
    },
    computed: {
      display: function() {
        return true;
      }
    }
  }
</script>

<style scoped>
  #villager-image {
    height: 200px;
    display: block;
    text-align: center;
    position: relative;
  }

  #card {
    display: inline-block;
    margin: 10px;
    border-radius: 25px;
    background: #42ad6b;
    padding: 20px;
    width: 200px;
    /*background: rgba(29,130,101,1);*/
    background: -moz-linear-gradient(top, rgba(29,130,101,1) 0%, rgba(103,191,147,1) 100%);
    background: -webkit-gradient(left top, left bottom, color-stop(0%, rgba(29,130,101,1)), color-stop(100%, rgba(103,191,147,1)));
    background: -webkit-linear-gradient(top, rgba(29,130,101,1) 0%, rgba(103,191,147,1) 100%);
    background: -o-linear-gradient(top, rgba(29,130,101,1) 0%, rgba(103,191,147,1) 100%);
    background: -ms-linear-gradient(top, rgba(29,130,101,1) 0%, rgba(103,191,147,1) 100%);
    background: linear-gradient(to bottom, rgba(29,130,101,1) 0%, rgba(103,191,147,1) 100%);
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#1d8265', endColorstr='#67bf93', GradientType=0 );
  }

  #name {
    color: white;
    font-size: 28px;
    font-weight: bold;
  }

  #species {
    font-variant: small-caps;
    font-size: 22px;
    color: white;
    opacity: 0.5;
    font-weight: bold;
  }

  img {
    max-width:100%;
    max-height:100%;
    width: 100px;
    object-fit: contain;
    position: absolute;
    bottom: 0px;
    margin-left: -50px;

  }
</style>