<template>
  <div id="app">
    <div class="card container ">
      <div class="row no-gutters">
        <ul class="col-4 d-flex align-items-center flex-column">
            <li class="logo" >logo</li>
            <li class="dist ">{{ dist }}</li>
            <li class="splogo ">splogo</li>
        </ul>
        <ul class="col-8  d-flex flex-column justify-content-between" >
            <li class="rd">{{ rd }}</li>
            <div class="other">
              <li class="rd2">{{ rd2 }}</li>
              <li class="no">{{ no }}</li>
              <li class="small">{{ small }}</li>
              <li class="no2">{{ no2 }}</li>
            </div>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'app',
  data(){
    return{
      dist:"萬里區",
      rd:"新北大道一段",
      rd2:"199巷10弄",
      no:"10",
      small:"之",
      no2:"4"
    }
  }
}
</script>

<style>
.card{
  width: 634px;
  height: 414px;
  background-color:rgb(16,153,123);
  border-radius: 30px;
  overflow: hidden;
}
ul{
  padding-top: 20px;
  list-style-type: none;
}
.logo{
  width: 130px;
  height: 130px;
  font-size: 0;
  background-size: cover;
  background-image: url("./assets/logo.png");
}
.dist{
  font-size : 3em;
  color:white;
}
.splogo{
  width: 200px;
  height: 200px;
  font-size: 0;
  background-size:cover;
  background-image: url("./assets/splogo.png");
}
.rd{
  font-size: 3.5em;
  color:white;
  font:italic;
}
.other{
  background: #fff;
  border-radius: 30px;
  color:rgb(16,153,123);
  height: 250px;
  width: 400px;
  margin-bottom: 30px;
  text-align: center;
}
.rd2{
  font-size: 3.0em;
}
.no{
  font-size: 8em;
  display: inline-block;
}
.small{
  font-size: 2em;
  display: inline-block;
}
.no2{
  font-size: 3.5em;
  display: inline-block;
}
</style>
