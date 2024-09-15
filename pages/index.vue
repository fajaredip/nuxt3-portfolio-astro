<template>
	<div>
		<header
			class="w-full h-16 fixed top-0 my-5 text-white flex items-center justify-between"
		>
			<div
				class="container mx-auto px-8 py-4 flex items-center justify-between"
			>
				<div class="header-left flex items-center">
					<img src="public/img/logo.svg" alt="logo" />
					<nav class="ml-8 hidden md:block">
						<ul class="flex items-center justify-between gap-8">
							<li>Home</li>
							<li>Skills</li>
							<li>Project</li>
						</ul>
					</nav>
				</div>
				<div class="header-right hidden md:block">
					<button
						class="border-white border-2 px-4 py-2 rounded-md hover:bg-white hover:text-neutral-800"
					>
						Let's Connect
					</button>
				</div>
			</div>
		</header>
		<section
			class="w-full min-h-screen bg-[url('/img/banner-bg.png')] bg-cover text-white"
		>
			<div
				class="container min-h-screen mx-auto px-8 pt-24 pb-4 flex items-center justify-center lg:justify-between flex-col lg:flex-row-reverse gap-8"
			>
				<img
					class="md:size-96 lg:size-full"
					src="public/img/header-img.svg"
					alt=""
				/>
				<div class="hero-text text-center lg:text-left">
					<p class="text-base lg:text-2xl mb-5">Welcome to the Space</p>
					<h1 class="text-4xl lg:text-8xl mb-5">
						Hi, I'm an <span class="font-semibold">Astronaut</span>
					</h1>
					<p class="lg:text-2xl mb-3">
						I'm a passionate
						<span class="font-semibold">Frontend Developer</span> who loves
						Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt sit
						error ipsa consectetur assumenda voluptate libero nulla atque
						voluptatem sint quisquam labore magnam natus saepe ducimus
						consequatur, quaerat molestiae aperiam!
					</p>
					<button
						class="border-white border-2 px-4 py-2 rounded-md hover:bg-white hover:text-neutral-800"
					>
						Let's Connect
					</button>
				</div>
			</div>
		</section>
		<section class="w-full bg-zinc-800 text-center px-8 py-10 text-slate-400">
			<h1 class="text-white text-4xl font-semibold mb-5">Skills</h1>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Possimus
				temporibus, similique natus optio nihil consequatur ipsam nisi repellat
				hic, praesentium ducimus adipisci suscipit sequi odit. Libero debitis
				quod illum ex.
			</p>
			<div class="flex items-center justify-center gap-5 mt-10">
				<div>
					<img class="mb-3" src="public/img/meter1.svg" alt="" />
					Skill 1
				</div>
				<div>
					<img class="mb-3" src="public/img/meter2.svg" alt="" />
					Skill 2
				</div>
				<div>
					<img class="mb-3" src="public/img/meter3.svg" alt="" />
					Skill 3
				</div>
			</div>
		</section>
		<section class="w-full bg-black">
			<div
				class="container w-full mx-auto text-center px-8 py-10 text-slate-400"
			>
				<h1 class="text-white text-4xl font-semibold mb-5">Projects</h1>
				<p>
					Lorem ipsum dolor sit amet consectetur adipisicing elit. Possimus
					temporibus, similique natus optio nihil consequatur ipsam nisi
					repellat hic, praesentium ducimus adipisci suscipit sequi odit. Libero
					debitis quod illum ex.
				</p>
				<div
					class="flex items-center justify-center flex-col md:flex-row gap-5 mt-10"
				>
					<div class="w-full lg:w-1/3 rounded-lg">
						<img src="public/img/project-img1.png" alt="" />
					</div>
					<div class="w-full lg:w-1/3 rounded-lg">
						<img src="public/img/project-img2.png" alt="" />
					</div>
					<div class="w-full lg:w-1/3 rounded-lg">
						<img src="public/img/project-img3.png" alt="" />
					</div>
				</div>
			</div>
		</section>
		<section
			class="w-full bg-gradient-to-r from-[#a33783] to-[#5930b5] text-center px-8 py-10 text-slate-400"
		>
			<h1 class="text-white text-4xl font-semibold mb-5">Get In Touch</h1>
			<div class="container mx-auto flex items-center justify-between md:gap-10">
				<img
					class="w-1/2 hidden md:block"
					src="public/img/contact-img.svg"
					alt=""
				/>
				<div class="w-full flex items-end justify-center flex-col gap-1">
					<div class="w-full flex items-center flex-col md:flex-row gap-1">
						<input
							class="w-full md:w-1/2 rounded-lg p-3 text-black bg-white bg-opacity-30 border border-gray-600 placeholder-zinc-400"
							type="text"
							placeholder="First Name"
						/>
						<input
							class="w-full md:w-1/2 rounded-lg p-3 text-black bg-white bg-opacity-30 border border-gray-600 placeholder-zinc-400"
							type="text"
							placeholder="Last Name"
						/>
					</div>
					<div class="w-full flex items-center flex-col md:flex-row gap-1">
						<input
							class="w-full md:w-1/2 rounded-lg p-3 text-black bg-white bg-opacity-30 border border-gray-600 placeholder-zinc-400"
							type="text"
							placeholder="Email Address"
						/>
						<input
							class="w-full md:w-1/2 rounded-lg p-3 text-black bg-white bg-opacity-30 border border-gray-600 placeholder-zinc-400"
							type="text"
							placeholder="Phone No."
						/>
					</div>
					<textarea
						class="w-full rounded-lg p-3 text-black bg-white bg-opacity-30 border border-gray-600 placeholder-zinc-400 resize-none"
						placeholder="Message"
						rows="5"
					></textarea>
					<button class="bg-slate-400 text-black px-5 py-2 rounded-lg">
						Send
					</button>
				</div>
			</div>
		</section>
		<footer class="w-full bg-[url('/img/footer-bg.png')] bg-cover px-8 py-5">
			<div class="container mx-auto w-full flex items-end justify-between">
				<img src="public/img/logo.svg" alt="logo" />
				<div class="socials flex items-center justify-between gap-3">
					<button class="border-white border-2 p-2 rounded-md">
						<img src="public/img/nav-icon1.svg" alt="facebook" />
					</button>
					<button class="border-white border-2 p-2 rounded-md">
						<img src="public/img/nav-icon2.svg" alt="twitter" />
					</button>
					<button class="border-white border-2 p-2 rounded-md">
						<img src="public/img/nav-icon3.svg" alt="instagram" />
					</button>
				</div>
			</div>
		</footer>
	</div>
</template>
