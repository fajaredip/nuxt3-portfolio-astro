<script setup>
	import { ref } from "vue";
	const isOpen = ref(false);
</script>

<template>
	<div>
		<header
			class="fixed top-0 z-10 flex items-center justify-between w-full my-0 text-white"
			:class="{ 'bg-neutral-800': isOpen }"
		>
			<div
				class="container flex items-center justify-between px-8 py-4 mx-auto"
			>
				<nav class="flex items-center justify-between w-full lg:justify-start">
					<div class="flex items-center">
						<img
							src="public/img/logo.svg"
							alt="logo"
							class="w-12 h-12 md:w-20 md:h-2w-20"
						/>
					</div>
					<div class="hidden space-x-10 lg:flex lg:ml-10">
						<a href="#home" class="transition-all duration-300 hover:text-indigo-400 hover:scale-105">Home</a>
						<a href="#skills" class="transition-all duration-300 hover:text-indigo-400 hover:scale-105">Skills</a>
						<a href="#projects" class="transition-all duration-300 hover:text-indigo-400 hover:scale-105">Projects</a>
					</div>
					<button
						@click="isOpen = !isOpen"
						class="px-3 py-1 border-2 border-white rounded-md lg:hidden transition-all duration-300 hover:bg-indigo-600 hover:border-indigo-600 hover:scale-105"
					>
						<i class="fa-solid fa-bars"></i>
					</button>
				</nav>
				<div class="hidden header-right lg:block">
					<button
						class="px-4 py-2 border-2 border-white rounded-md hover:bg-white hover:text-neutral-800 text-nowrap transition-all duration-300 hover:scale-105"
					>
						Let's Connect
					</button>
				</div>
			</div>
			<div
				v-if="isOpen"
				class="absolute left-0 flex flex-col w-full gap-2 p-5 space-y-2 text-center lg:hidden bg-neutral-800 top-16"
			>
				<a href="#home" class="transition-all duration-300 hover:text-indigo-400 hover:scale-105">Home</a>
				<a href="#skills" class="transition-all duration-300 hover:text-indigo-400 hover:scale-105">Skills</a>
				<a href="#projects" class="transition-all duration-300 hover:text-indigo-400 hover:scale-105">Projects</a>
				<button
					class="px-4 py-2 border-2 border-white rounded-md hover:bg-white hover:text-neutral-800 text-nowrap transition-all duration-300 hover:scale-105"
				>
					Let's Connect
				</button>
			</div>
		</header>
		<section
			id="home"
			class="w-full min-h-svh bg-[url('/img/banner-bg.png')] bg-cover text-white lg:pb-36"
		>
			<div class="container mx-auto min-h-svh">
				<div
					class="flex flex-col items-center justify-center gap-8 px-8 pt-10 pb-4 h-svh lg:justify-between lg:flex-row-reverse"
				>
					<img
						class="md:size-3/5 lg:size-96 xl:size-3/5 animate-float"
						src="public/img/header-img.svg"
						alt=""
					/>
					<div class="text-center hero-text lg:text-left lg:w-1/2 xl:w-4/6">
						<p class="mb-5 text-base lg:text-2xl">Welcome to the Space</p>
						<h1 class="mb-5 text-6xl xl:text-8xl">
							Hi, I'm an <span class="font-semibold text-indigo-400">Astronaut</span>
						</h1>
						<p class="mb-3 text-base lg:text-2xl">
							I'm a passionate
							<span class="font-semibold text-indigo-300">Frontend Developer</span> who loves
							Lorem ipsum dolor sit amet consectetur adipisicing elit.
						</p>
						<a
							href="#footer"
							class="block px-4 py-2 mx-auto my-4 border-2 border-white rounded-md hover:bg-white hover:text-neutral-800 w-fit lg:mx-0 transition-all duration-300 hover:scale-105"
						>
							Let's Connect <i class="ml-3 fa-regular fa-circle-down"></i>
						</a>
					</div>
				</div>
			</div>
		</section>
		<section id="skills" class="lg:relative">
			<div
				class="w-full px-8 py-10 text-center bg-zinc-800 text-slate-400 lg:absolute lg:-bottom-56 lg:left-1/2 lg:w-4/5 lg:rounded-3xl lg:transform lg:-translate-x-1/2"
			>
				<h1 class="mb-5 text-4xl font-semibold text-indigo-200">Skills</h1>
				<p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
				<p>
					Possimus temporibus, similique natus optio nihil consequatur ipsam
					nisi repellat hic, praesentium ducimus adipisci suscipit sequi odit.
					Libero debitis quod illum ex.
				</p>
				<div class="flex items-center justify-center gap-5 mt-10 md:gap-20">
					<div class="transition-transform duration-300 hover:scale-105">
						<img class="mb-3 md:size-40" src="public/img/meter1.svg" alt="" />
						Skill 1
					</div>
					<div class="transition-transform duration-300 hover:scale-105">
						<img class="mb-3 md:size-40" src="public/img/meter2.svg" alt="" />
						Skill 2
					</div>
					<div class="transition-transform duration-300 hover:scale-105">
						<img class="mb-3 md:size-40" src="public/img/meter3.svg" alt="" />
						Skill 3
					</div>
				</div>
			</div>
		</section>
		<section id="projects" class="w-full bg-black lg:pt-60">
			<div
				class="container w-full px-8 py-10 mx-auto text-center text-slate-400"
			>
				<h1 class="mb-5 text-4xl font-semibold text-indigo-200">Projects</h1>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Possimus
					temporibus, similique natus optio nihil consequatur ipsam nisi
					repellat hic, praesentium ducimus adipisci suscipit sequi odit. Libero
					debitis quod illum ex.
				</p>
				<div
					class="flex flex-col items-center justify-center gap-5 mt-10 md:flex-row"
				>
					<div class="w-full rounded-lg lg:w-1/3 transition-transform duration-300 hover:scale-105">
						<img src="public/img/project-img1.png" alt="" />
					</div>
					<div class="w-full rounded-lg lg:w-1/3 transition-transform duration-300 hover:scale-105">
						<img src="public/img/project-img2.png" alt="" />
					</div>
					<div class="w-full rounded-lg lg:w-1/3 transition-transform duration-300 hover:scale-105">
						<img src="public/img/project-img3.png" alt="" />
					</div>
				</div>
			</div>
		</section>
		<section
			id="contact"
			class="w-full bg-gradient-to-r from-[#a33783] to-[#5930b5] text-center text-slate-400"
		>
			<div
				class="container flex items-center justify-between px-8 py-10 mx-auto md:gap-10 lg:gap-20"
			>
				<img
					class="hidden w-1/2 lg:w-2/6 md:block"
					src="public/img/contact-img.svg"
					alt=""
				/>
				<div class="flex flex-col items-start justify-center w-full">
					<h1 class="mb-5 text-4xl font-semibold text-indigo-200">Get In Touch</h1>
					<div class="flex flex-col items-end justify-center w-full gap-1">
						<div class="flex flex-col items-center w-full gap-1 md:flex-row">
							<input
								class="w-full p-3 text-black bg-white border border-gray-600 rounded-lg md:w-1/2 bg-opacity-30 placeholder-zinc-400 focus:ring-2 focus:ring-indigo-500 transition-all duration-300"
								type="text"
								placeholder="First Name"
							/>
							<input
								class="w-full p-3 text-black bg-white border border-gray-600 rounded-lg md:w-1/2 bg-opacity-30 placeholder-zinc-400 focus:ring-2 focus:ring-indigo-500 transition-all duration-300"
								type="text"
								placeholder="Last Name"
							/>
						</div>
						<div class="flex flex-col items-center w-full gap-1 md:flex-row">
							<input
								class="w-full p-3 text-black bg-white border border-gray-600 rounded-lg md:w-1/2 bg-opacity-30 placeholder-zinc-400 focus:ring-2 focus:ring-indigo-500 transition-all duration-300"
								type="text"
								placeholder="Email Address"
							/>
							<input
								class="w-full p-3 text-black bg-white border border-gray-600 rounded-lg md:w-1/2 bg-opacity-30 placeholder-zinc-400 focus:ring-2 focus:ring-indigo-500 transition-all duration-300"
								type="text"
								placeholder="Phone No."
							/>
						</div>
						<textarea
							class="w-full p-3 text-black bg-white border border-gray-600 rounded-lg resize-none bg-opacity-30 placeholder-zinc-400 focus:ring-2 focus:ring-indigo-500 transition-all duration-300"
							placeholder="Message"
							rows="5"
						></textarea>
						<button class="px-5 py-2 text-black rounded-lg bg-slate-400">
							Send
						</button>
					</div>
				</div>
			</div>
		</section>
		<footer
			id="footer"
			class="w-full bg-[url('/img/footer-bg.png')] bg-cover px-8 py-5"
		>
			<div
				class="container flex items-center justify-between w-full mx-auto text-white"
			>
				<img
					src="public/img/logo.svg"
					alt="logo"
					class="w-12 h-12 md:w-20 md:h-2w-20"
				/>
				<div class="flex items-center justify-between gap-3 socials">
					<button class="p-2 border-2 border-white rounded-md transition-all duration-300 hover:bg-indigo-600 hover:scale-105">
						<img src="public/img/nav-icon1.svg" alt="facebook" />
					</button>
					<button class="p-2 border-2 border-white rounded-md transition-all duration-300 hover:bg-indigo-600 hover:scale-105">
						<img src="public/img/nav-icon2.svg" alt="twitter" />
					</button>
					<button class="p-2 border-2 border-white rounded-md transition-all duration-300 hover:bg-indigo-600 hover:scale-105">
						<img src="public/img/nav-icon3.svg" alt="instagram" />
					</button>
				</div>
			</div>
		</footer>
	</div>
</template>

<style scoped>
.animate-float {
	animation: float 3s ease-in-out infinite;
}
@keyframes float {
	0%, 100% {
		transform: translateY(0px);
	}
	50% {
		transform: translateY(-10px);
	}
}
</style>
