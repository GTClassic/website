<script lang="ts">
	import Window from '$lib/components/Window.svelte';
	import DownloadButton from '$lib/components/DownloadButton.svelte';
</script>

<Window title="Howdy!" classes="flex-1  w-full">
	{#snippet icon()}
		<img src="/icons/face-smile.png" alt="Smile Icon" class="w-6 h-6" />
	{/snippet}
	<div class="text-shadow-black/5 text-shadow-md">
		<p class="text-2xl font-bold">Welcome to Gorilla Tag: Classic!</p>
		<p>
			Gorilla Tag: Classic is a community-first, self-hostable fork of Gorilla Tag v1.0.8 + accompanying
			software. It is inspired by long-running, community-ran multiplayer gaming communities
			among the likes of Source Engine, Minecraft, Doom, and Quake.
		</p>
		<div class="mb-2"></div>
		<p class="text-2xl font-bold">But, why?</p>
		<p>
			Gorilla Tag was supposed to be a game about tag. Over time, as profit took a top priority, Another Axiom
			has distracted from Gorilla Tag's core game-play ideologies by adding unneeded content,
			microtransactions, and generally making the game unfun. For this reason, we've decided to make
			a fork of the game designed to focus on the core tag experience while providing further flexibility to its community.
		</p>
		<p class="text-2xl font-bold">What sets you apart from clones?</p>
		<p>
			The Oculus store is flooded with low quality ripped Gorilla Tag versions.
			We want to seperate ourselves from such clones in a couple ways:
		</p>
		<p class="text-xl font-semibold">Minimal Bloat</p>
		<p>
			No mod menus or extra maps as part of the base game. Gorilla Tag: Classic is meant to harness the
			simplicity of 2021-era Gorilla Tag.
		</p>
		<p class="text-xl font-semibold">Selfhostable Servers</p>
		<p>
			Rather than having a centralised cluster of servers, GT:Classic lets players host their own
			servers, with their own rules, their own settings, and their own mods. We host a "Master
			Server" which acts as a server list. Selfhosting is made as easy as possible, so that anyone
			can do it. <span class="opacity-50 italic">(you run one file!)</span>
		</p>
		<hr class="my-2" />

		<p class="text-2xl font-bold">Ready to try?</p>
		<p>
			Unfortunately, GT:Classic is still a work in progress. Although you can't play <span
				class="italic">yet</span
			>, you can still
			<a
				href="https://discord.gg/YJxVwHmrrt"
				class="underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white">join our Discord</a
			>
			to get pinged once a beta is available, or the game releases!
			<br />
		</p>
		<!--
		<p>Download GT:Classic here!</p>
		<hr class="my-2" />

		<div class="flex gap-2">
			<DownloadButton
				icon="/icons/actions/small/48x48/download.svg"
				label="Download GT:Classic Launcher"
				subtitle="1.0.0, Windows"
				variant="primary"
			/>
			<DownloadButton
				icon="icons/places/network-server.svg"
				label="Download GT:Classic Game Server"
				subtitle="1.0.0, Windows"
			/>
		</div>
		-->
	</div>
</Window>
