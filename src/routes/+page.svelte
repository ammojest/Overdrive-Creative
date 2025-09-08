<section class="relative flex h-[80vh] flex-col items-center justify-start pt-16">
	<img
		src="/leather-jacket.png"
		alt="Leather Jacket"
		class="absolute top-0 left-0 z-0 h-full w-full object-cover"
	/>
	<div class="relative z-10 flex w-full flex-col items-center">
		<div class="bg-opacity-30 mt-0 flex flex-col items-center rounded-lg bg-black px-8 py-12">
			<h1 class="mb-4 text-5xl font-extrabold text-white drop-shadow-lg">Overdrive Creative</h1>
			<p class="text-lg text-white opacity-80 drop-shadow">
				A new creative experience is coming soon.
			</p>
		</div>
	</div>
</section>

<section class="mx-auto grid max-w-4xl grid-cols-1 gap-8 py-12 md:grid-cols-3">
	<div class="rounded-lg bg-white p-6 text-center shadow">
		<h2 class="mb-2 text-2xl font-bold text-purple-700">Product Photography</h2>
		<p class="text-gray-700">
			Showcase your products with stunning, high-quality images that capture every detail.
		</p>
	</div>
	<div class="rounded-lg bg-white p-6 text-center shadow">
		<h2 class="mb-2 text-2xl font-bold text-pink-600">Portrait Photography</h2>
		<p class="text-gray-700">
			Professional portraits for individuals, teams, and events, tailored to your style.
		</p>
	</div>
	<div class="rounded-lg bg-white p-6 text-center shadow">
		<h2 class="mb-2 text-2xl font-bold text-blue-600">Web & App Development</h2>
		<p class="text-gray-700">
			Modern websites and applications designed to elevate your brand and engage your audience.
		</p>
	</div>
</section>

<section class="mx-auto max-w-2xl py-12">
	<h2 class="mb-6 text-center text-3xl font-bold text-purple-700">Contact Us</h2>
	<form class="flex flex-col gap-4 rounded-lg bg-white p-8 shadow">
		<input
			type="text"
			name="name"
			placeholder="Your Name"
			class="rounded border px-4 py-2"
			required
		/>
		<input
			type="email"
			name="email"
			placeholder="Your Email"
			class="rounded border px-4 py-2"
			required
		/>
		<textarea
			name="message"
			placeholder="Your Message"
			class="rounded border px-4 py-2"
			rows="4"
			required
		></textarea>
		<button
			type="submit"
			class="rounded bg-purple-600 py-2 font-bold text-white transition hover:bg-purple-700"
			>Send Message</button
		>
	</form>
</section>
