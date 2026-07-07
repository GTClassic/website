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
			GT:Classic is a community-first, self-hostable fork of Gorilla Tag v1.0.8 + accompanying
			software. Players and creatives should be of upmost importance, not profit margins.
		</p>
		<div class="mb-2"></div>
		<p class="text-2xl font-bold">But, why?</p>
		<p>
			Gorilla Tag was supposed to be, well, a game about tag. Over the past few years, Another Axiom
			has been destroying any semblance of the game's former glory by adding unneeded content,
			microtransactions and generally making the game unfun. For this reason, we've decided to make
			a fork of the game which brings the game back to its former glory.
		</p>
		<p class="text-2xl font-bold">What sets you apart from clones?</p>
		<p>
			The Oculus store is flooded with low quality ripped Gorilla Tag versions, bloated with mod
			menus, maps, and other bullshit. We want to seperate ourselves from such clones in a couple
			ways:
		</p>
		<p class="text-xl font-semibold">Minimal Bloat</p>
		<p>
			No mod menus, no extra maps, nothing. GT:Classic is meant to be as close to the base game as
			possible, barring some QoL features.
		</p>
		<p class="text-xl font-semibold">Selfhostable Servers</p>
		<p>
			Rather than having a centralised cluster of servers, GT:Classic lets players host their own
			servers, with their own rules, their own settings, and their own mods. We host a "Master
			Server" which acts as a server list. Selfhosting is made as easy as possible, so that anyone
			can do it. (you run one file!)
		</p>
		<p class="text-2xl font-bold">Ready to try?</p>
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
	</div>
</Window>
