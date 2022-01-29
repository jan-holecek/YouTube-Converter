<template>
<main class="container">
	<h2>About BooperConverter</h2>
    <p>BooperConverter is the easiest and free service to convert and download youtube videos in the best available qualities. By using the BooperConverter, you can quickly convert and download your favorite youtube videos to mp3 audio format. It works for all browsers like Firefox, Chrome, Safari, Opera, etc. BooperConverter is the ultimate online tool to convert Youtube videos to mp3 for all devices like Computers, Mobile phones, and tablets. You can convert unlimited youtube videos without any registration, this is totally free and safe to use for your personal downloads.</p>
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
