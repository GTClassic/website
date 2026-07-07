<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.png';
	import Window from '$lib/components/Window.svelte';

	let { children } = $props();
</script>

<svelte:head
	><link rel="icon" href={favicon} />
	<title>Gorilla Tag: Classic</title></svelte:head
>
<img
	src="https://raw.githubusercontent.com/GTClassic/branding/main/gt-classic-wordmark.png"
	alt="Gorilla Tag: Classic Logo"
	class="w-72 [image-rendering:pixelated] mb-2"
/>
<div class="flex gap-2">
	<Window title="Links" classes="!w-48 h-fit">
		<a
			href="/"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
			><img src="/icons/actions/go-home.svg" alt="Home Icon" class="w-4 h-4" />Home</a
		>
		<a
			href="/downloads"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
			><img
				src="/icons/actions/small/48x48/download.svg"
				alt="Downloads Icon"
				class="w-4 h-4"
			/>Downloads</a
		>
		<a
			href="/credits"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
			><img src="/icons/categories/system-users.svg" alt="People Icon" class="w-4 h-4" />Credits</a
		>
		<a
			href="/changelog"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
			><img src="/icons/apps/knewsticker.svg" alt="News Icon" class="w-4 h-4" />Changelog</a
		>
		<a
			href="/rules"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
			><img
				src="/icons/actions/small/48x48/help-about.svg"
				alt="Info Icon"
				class="w-4 h-4"
			/>Rules</a
		>
		<a
			href="/faq"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
			><img src="/icons/actions/help-hint.svg" alt="Lightbulb Icon" class="w-4 h-4" />FAQ</a
		>
		<a
			href="/support"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
			><img src="/icons/apps/help-browser.svg" alt="Life Buoy Icon" class="w-4 h-4" />Support</a
		>
		<hr class="my-2" />
		<a
			href="/"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
			><img src="/icons/discord.svg" alt="Discord Icon" class="w-4 h-4" />Discord</a
		>
		<a
			href="/"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
			><img src="/icons/github.svg" alt="GitHub Icon" class="w-4 h-4" />GitHub</a
		>
	</Window>
	{@render children()}
	<div class="flex-col">
		<Window title="Downloads n' stuff" classes="h-fit">
			<a
				href="/"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
				><img
					src="/icons/actions/small/48x48/download.svg"
					alt="Downloads Icon"
					class="w-4 h-4"
				/>Download GT:Classic 1.0.0</a
			>
			<a
				href="/"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
				><img src="/icons/places/network-server.svg" alt="Downloads Icon" class="w-4 h-4" />Download
				GT:Classic Server</a
			>
		</Window>
		<p class="text-center mt-1 text-white/35 text-shadow-black/10 text-shadow-lg">
			website by xenon
		</p>
	</div>
</div>
