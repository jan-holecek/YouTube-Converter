<template>
		<nav class="bg-white shadow-lg">
				<div class="flex justify-between">
					<div class="flex space-x-9">
						<div>
							<a href="#" class="flex items-center py-4 px-2">
								<span class="font-semibold text-green-500 text-xl">Booper</span><span class="font-semibold text-gray-800 text-xl">Converter</span>
							</a>
						</div>
					</div>
                    <div class="hidden md:flex items-center space-x-3">
						<a href="" class="py-4 px-2 text-green-500 border-b-4 border-green-500 font-semibold ">Home</a>
					</div>
					<div class="md:hidden flex items-center pr-4">
						<button class="outline-none mobile-menu-button">
						<svg class=" w-6 h-6 text-gray-800 hover:text-green-500"
							x-show="!showMenu"
							fill="none"
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							viewBox="0 0 24 24"
							stroke="currentColor"
						>
							<path d="M4 6h16M4 12h16M4 18h16"></path>
						</svg>
					</button>
					</div>
				</div>
			<div class="hidden mobile-menu">
				<ul class="text-center">
					<li class="active"><a href="" class="border-b-2 border-gray-200 block text-sm px-2 py-4 text-white bg-green-500 font-semibold">Home</a></li>
				</ul>
			</div>
		</nav>
</template>

<script>
export default {
  name: 'Navbar',
  props: {
    msg: String
  },
  mounted() {
    const btn = document.querySelector("button.mobile-menu-button");
	const menu = document.querySelector(".mobile-menu");

	btn.addEventListener("click", () => {
		menu.classList.toggle("hidden");
	});
  }
}

</script>

<style scoped>
</style>
