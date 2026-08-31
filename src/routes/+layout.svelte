<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.png';
	import Window from '$lib/components/Window.svelte';

	let { children } = $props();

	let dark = $state(true);

	function toggleTheme() {
		dark = !dark;
		document.documentElement.classList.toggle('dark', dark);
	}
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
<div class="grid grid-cols-1 gap-2 md:grid-cols-[auto_1fr_auto]">
	<Window title="Links" classes="!w-full md:!w-48 h-fit order-1 md:order-none">
		{#snippet icon()}
			<img src="/icons/emblem-symbolic-link.png" alt="Links Icon" class="w-6 h-6" />
		{/snippet}
		<div class="flex flex-wrap gap-x-4 gap-y-1 md:flex-col md:flex-nowrap">
			<a
				href="/"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img src="/icons/actions/go-home.svg" alt="Home Icon" class="w-4 h-4" />Home</a
			>
			<a
				href="/downloads"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img
					src="/icons/actions/small/48x48/download.svg"
					alt="Downloads Icon"
					class="w-4 h-4"
				/>Downloads</a
			>
			<a
				href="/credits"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img
					src="/icons/categories/system-users.svg"
					alt="People Icon"
					class="w-4 h-4"
				/>Credits</a
			>
			<a
				href="/changelog"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img src="/icons/apps/knewsticker.svg" alt="News Icon" class="w-4 h-4" />Changelog</a
			>
			<a
				href="/rules"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img
					src="/icons/actions/small/48x48/help-about.svg"
					alt="Info Icon"
					class="w-4 h-4"
				/>Rules</a
			>
			<a
				href="/faq"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img src="/icons/actions/help-hint.svg" alt="Lightbulb Icon" class="w-4 h-4" />FAQ</a
			>
			<a
				href="/support"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img src="/icons/apps/help-browser.svg" alt="Life Buoy Icon" class="w-4 h-4" />Support</a
			>
			<hr class="hidden md:block my-2" />
			<a
				href="https://discord.gg/YJxVwHmrrt"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img src="/icons/discord.svg" alt="Discord Icon" class="w-4 h-4" />Discord</a
			>
			<a
				href="https://git.soweli.uk/GTClassic"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img src="/icons/forgejo.svg" alt="Forgejo Icon" class="w-4 h-4" />Git</a
			>
		</div>
	</Window>
	<div class="order-2 md:order-none">
		{@render children()}
	</div>
	<div class="order-3 md:order-none">
		<Window title="Downloads n' stuff" classes="w-full md:w-fit h-fit">
			{#snippet icon()}
				<img src="/icons/download-later.png" alt="Downloads Icon" class="w-6 h-6" />
			{/snippet}
			<p>Not available yet!</p>
			<!--
			<a
				href="/"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img
					src="/icons/actions/small/48x48/download.svg"
					alt="Downloads Icon"
					class="w-4 h-4"
				/>Download GT:Classic 1.0.0</a
			>
			<a
				href="/"
				class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				><img src="/icons/places/network-server.svg" alt="Downloads Icon" class="w-4 h-4" />Download
				GT:Classic Server</a
			>
			-->
		</Window>
		<div class="mt-2">
			<Window title="Lightswitch" classes="w-full md:w-fit h-fit">
				{#snippet icon()}
					<img
						src={dark ? '/icons/lightsoff.png' : '/icons/lightson.png'}
						alt="Lightswitch Icon"
						class="w-6 h-6"
					/>
				{/snippet}
				<button
					onclick={toggleTheme}
					class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white cursor-pointer"
					><img
						src={dark ? '/icons/lightsoff.png' : '/icons/lightson.png'}
						alt="Lightswitch Icon"
						class="w-4 h-4"
					/>{dark ? 'Switch to Light mode' : 'Switch to Dark mode'}</button
				>
			</Window>
		</div>
	</div>
</div>
<p
	class="text-center mt-auto pt-2 text-white/35 text-shadow-black/10 text-shadow-lg"
	title="Now, these points of data make a beautiful line
And we're out of beta, we're releasing on time
So I'm GLaD I got burned, think of all the things we learned
For the people who are Still Alive"
>
	© 2026 The Gorilla Tag: Classic Team <br /> Not affiliated with Another Axiom
</p>
