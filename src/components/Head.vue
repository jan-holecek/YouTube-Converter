<template>
<header>
<div class="head-message">
    <h1>YouTube downloader</h1>
    <p>Stahujte a převádějte videa do MP3 z Youtube</p>
  <div class="search-box" id="SBox">
    <div class="error">
    </div>
    <input id="search" placeholder="Sem vložte odkaz..." type="text" required>
  </div>
  <div class="buttons">
    <select class="form-control format">
      <option selected disabled>Formát</option>
      <option value="mp3">Mp3</option>
    </select>
  <button class="also search-link send" id="searchclick">Odeslat</button>
  <div class="message"></div>
  </div>
</div>
</header>
</template>

<script>
const $ = require('jquery')

export default {
  name: 'Head',
  props: {
    msg: String
  },
  mounted() {
  $(".also").click(function(){
    let link = $("#search").val();
    let format = $(".form-control").children("option:selected").val();
    format = "mp3";

  if(link === "") {
    $('.error').html('<p style="  font-size: 15px;color: rgb(255, 0, 0);position: relative;left: 50%;transform: translateX(-66%);" class="error-msg">Zadejte platný odkaz na video</p>');
  } else {
    $('.error').html('');
    downloadVideo(link,format);
  }
  
  });
  function downloadVideo(link,format) {
    $('.message').html('<iframe href="#" style="width:100%;height:60px;border:0;overflow:hidden;" scrolling="no" src="https://loader.to/api/button/?url='+link+'&f='+format+'"></iframe>');
  }
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Cookie');
@import url('https://fonts.googleapis.com/css?family=Open+Sans:400,600,700');
@import url('https://netdna.bootstrapcdn.com/font-awesome/4.0.3/css/font-awesome.css');

select {
  color: #000;
  height: 48px;
  width: 150px;
  background-color: #fff;
  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
  cursor: pointer;
  position: relative;
  outline: 0;
  border-radius: 5px;
  margin: 0 auto;
  top: 50px;
  margin-right: 50px;
}

header {
  position: relative;
  background: #28363A;
  width: 100%;
  height: 80vh;
  min-height: 18rem;
  /* -webkit-clip-path: polygon(0 0, 100% 0%, 100% 100%, 0 90%); */
  z-index: 0;
}

header .head-message {
  padding-top: 5rem;
  vertical-align: middle;
  text-align: center;
  color: white;
}

header .head-message h1 {
  font-size: 2.7rem;
  color: white;
  font-weight: 400;
}

header .head-message p {
  font-size: 15px;
}

header .head-message h2 {
  font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
  font-weight: 300;
  color: rgba(255,255,255,0.75);
}

.search-box {
  width: 100%;
  position: relative;
  top: 25px;
  height: 48px;
  transition: opacity 0.4s linear ,visibility 0.4s linear 0s;
  margin: 0 auto;
}

.search-box > #search {
  width: 640px;
  height: 48px;
  border-radius: 6px;
}

input , input:focus {
  border: none;
  box-shadow: none;
  background-color: none;
  outline: 0;
  font-size: 16px;
  font-family: 'Open Sans';
  color: #28363A;
  padding: 0px 12px;
}

.message {
  position: relative;
  top: 80px;
}

button {
  font-family: Arial, Helvetica, sans-serif;
  color: #fff;
  background-color: #48bb78;
  height: 48px;
  width: 150px;
  text-align: center;
  cursor: pointer;
  border-left: 1px solid #48bb78;
  position: relative;
  border: none;
  border-radius: 5px;
  margin: 0 auto;
  top: 50px;
}

.search-link:hover {
  background: #28c469;
  transition: 0.3s;
}

@media screen and (max-width: 637px) {
  .search-box > #search { 
    width: calc(100% - 10%);
  }
}

@media screen and (max-width: 349px) {
  select, button {
    margin: 10px;
    margin-bottom: 10px;
  }
}
</style>
