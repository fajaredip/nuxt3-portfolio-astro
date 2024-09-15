<script setup lang="ts">
useHead({
    title: "Astro Portfolio",
		link: [
			{
				rel: "stylesheet",
				href: "https://fonts.googleapis.com/css2?family=SUSE:wght@100..800&display=swap",
			},
		],
    script: [
			{
				crossorigin: "anonymous",
				src: "https://kit.fontawesome.com/0db2cbd175.js",
			},
		],
	});
</script>

<template>
	<NuxtLayout />
</template>