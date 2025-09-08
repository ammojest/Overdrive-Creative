<script lang="ts">
	import '../app.css';
	let menuOpen = false;
	function toggleMenu() {
		menuOpen = !menuOpen;
	}
	let { children } = $props();
</script>

<header class="bg-opacity-90 flex items-center justify-between bg-black px-6 py-4 shadow">
	<div class="text-2xl font-bold text-white">Overdrive Creative</div>
	<nav class="relative">
		<button
			class="flex h-10 w-10 flex-col items-center justify-center focus:outline-none md:hidden"
			aria-label="Toggle menu"
			on:click={toggleMenu}
		>
			<span
				class="mb-1 block h-1 w-7 rounded bg-white transition-all duration-300"
				style:transform={menuOpen ? 'rotate(45deg) translateY(8px)' : ''}
			></span>
			<span
				class="mb-1 block h-1 w-7 rounded bg-white transition-all duration-300"
				style:opacity={menuOpen ? 0 : 1}
			></span>
			<span
				class="block h-1 w-7 rounded bg-white transition-all duration-300"
				style:transform={menuOpen ? 'rotate(-45deg) translateY(-8px)' : ''}
			></span>
		</button>
		<ul
			class="absolute top-12 right-0 flex flex-col gap-4 rounded bg-black px-8 py-4 text-lg text-white shadow-lg md:static md:flex-row md:items-center md:gap-8 md:bg-transparent md:px-0 md:py-0 md:text-base md:shadow-none"
			class:hidden={!menuOpen && window.innerWidth < 768}
			class:flex={menuOpen || window.innerWidth >= 768}
		>
			<li><a href="/" class="hover:text-purple-400">Home</a></li>
			<li><a href="#product" class="hover:text-purple-400">Product Photography</a></li>
			<li><a href="#portrait" class="hover:text-pink-400">Portrait Photography</a></li>
			<li><a href="#webdev" class="hover:text-blue-400">Web/App Development</a></li>
			<li><a href="#contact" class="hover:text-purple-400">Contact</a></li>
		</ul>
	</nav>
</header>

<main>
	{@render children()}
</main>

<footer class="mt-8 bg-gray-900 py-3 text-center text-sm text-gray-300">
	&copy; 2025 Overdrive Creative. All rights reserved.
</footer>
