<template>
<main class="container">
		<h2>Jak převést YouTube video do MP3</h2>
		<ul class="cards grid">
			<li class="card-item grid-item grid-third">
				<div class="card-info">
					<h3 class="class-title">1. Zkopírujte adresu URL</h3>
					<p>Otevřete YouTube a zkopírujte adresu URL videa, které chcete stáhnout do zařízení.</p>
				</div>
			</li>
			<li class="card-item grid-item grid-third">
				<div class="card-info">
					<h3 class="Class-title">2. Vložte adresu URL do pole</h3>
					<p>Vložte zkopírovanou adresu URL do pole výše a vyberte formát MP3. Klikněte na tlačítko ODESLAT a chvíli počkejte.</p>
				</div>
			</li>
			<li class="card-item grid-item grid-third">
				<div class="card-info">
					<h3 class="class-title">3. Stáhněte si YouTube video jako MP3</h3>
					<p>Po načtení uvidíte video převedené do MP3. Nyní si jej můžete stáhnout do svého zařízení.</p>
				</div>
			</li>
		</ul>
</main>
</template>

<script>
export default {
  name: 'HowTo',
  props: {
    msg: String
  },
}
</script>

<style scoped>
ul {
	margin-top: 0;
	margin-bottom: 0;
}

p {
	margin-top: 10px;
	margin-bottom: 5px;
}

h1 {
	font-weight: normal;
	font-size: 35px;
	margin-top: 20px;
	margin-bottom: 20px;
}

h2 {
	font-weight: normal;
	margin-top: 20px;
	margin-bottom: 10px;
    font-size: 40px;
    font-weight: 400;
	color: #fff;
}

h3 {
	font-weight: 700;
	margin-top: 10px;
	margin-bottom: 10px;
	font-size: 1rem;
	color: #48bb78;
	text-transform: uppercase;
}

.container {
	padding: 10px;
	max-width: 900px;
	margin: 0 auto;
	text-align: center;
}

.list-noBullets {
	list-style: none;
	padding-left: 0;
}

.photo {
	border-radius: 300px;
	max-width: 200px;
	margin: 10px auto 20px auto;
	display: block;
	-webkit-filter: grayscale(100%);
    filter: grayscale(100%);
}

.cards {
	padding: 0;
	margin: 0;
}

.card-item {
	list-style: none;
	margin-bottom: 20px;
	background-color: #eeeeee;
}

.card-title {
	padding: 0px 10px 7px 10px;
	display: block;
	align-items: flex-start;
}

.card-info {
	font-size: 16px;
	min-height: 100px;
	padding: 20px;
}

.card-info .card-title {
	font-weight: 700;
}

.grid {
	overflow: hidden;
}

.grid-item {
	box-sizing: border-box;
	margin: 1%;
	float: left;
	width: 100%;
}

.grid-item:hover {
	transform: scale(0.98);
}

@media all and (min-width: 480px) {
	.card-info {
		min-height: 200px;
	}

	.grid-item {
		width: 48%;
	}
}
@media all and (min-width: 592px) {

	.grid {
		display: flex; 	
		flex-wrap: wrap;
	}

	h1 {
		font-size: 60px;
		margin-top: 30px;
		margin-bottom: 30px;
	}

	.grid-item {
		width: auto;
	}

	.grid-whole {
		width: 98%;
	}

	.grid-half {
		width: 48%;
	}

	.grid-third {
		width: 31.3%;
	}

	.grid-quarter {
		width: 23%;
	}
}
</style>
