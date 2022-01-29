<template>
<main class="container">
	<h2>Co je BooperConverter</h2>
  <p>BooperConverter je nejjednodušší a bezplatná služba pro konverzi a stahování videí z youtube v nejlepších dostupných kvalitách. Pomocí BooperConverter můžete rychle převádět a stahovat svá oblíbená videa z youtube do zvukového formátu mp3. Funguje pro všechny prohlížeče, jako je Firefox, Chrome, Safari, Opera atd. BooperConverter je dokonalý online nástroj pro převod videí z Youtube do mp3 pro všechna zařízení, jako jsou počítače, mobilní telefony a tablety. Můžete převádět neomezený počet videí z youtube bez registrace, je to zcela zdarma a bezpečné pro vaše osobní stahování.</p>
</main>
</template>

<script>
export default {
  name: 'About',
  props: {
    msg: String
  },
}
</script>

<style scoped>
p {
	margin-top: 10px;
	margin-bottom: 5px;
}

h2 {
	font-weight: normal;
	margin-top: 20px;
	margin-bottom: 10px;
    font-size: 40px;
    font-weight: 400;
}

.container {
	padding: 10px;
	max-width: 900px;
	margin: 0 auto;
	text-align: center;
}

@media screen and (max-width: 333px) {
  h2 {
    font-size: 34px;
  }
}
</style>
