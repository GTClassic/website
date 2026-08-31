<script lang="ts">
	import Window from '$lib/components/Window.svelte';
</script>

<Window title="FAQ" classes="flex-1 h-fit  w-full">
	{#snippet icon()}
		<img src="/icons/actions/help-hint.svg" alt="Lightbulb Icon" class="w-6 h-6" />
	{/snippet}
	<div class="text-shadow-black/5 text-shadow-md">
		<p class="text-2xl font-bold">FAQ</p>

		<p class="text-xl font-semibold">What is GT:Classic?</p>
		<p>
			Gorilla Tag: Classic is a community-first, self-hostable fork of Gorilla Tag v1.0.8 and its accompanying
			software. It aims to bring the game back to its roots, without microtransactions, mod menus,
			or unneeded content.
		</p>

		<p class="text-xl font-semibold">Is it legal?</p>
		<p>
			Gorilla Tag: Classic is built on Gorilla Tag v1.0.8, released in mid-June 2021. We don't sell anything,
			we don't run ads, and we don't make money off it. Gorilla Tag: Classic is a fan-made project and isn't
			affiliated with or endorsed by Another Axiom. We only distribute patches, never the full game.
			You will need to own the game on Steam to play.
		</p>

		<p class="text-xl font-semibold">Is there a download?</p>
		<p>
			Not yet! Gorilla Tag: Classic is still a work in progress. When a beta is available we'll post it on the
			<a
				href="https://discord.gg/YJxVwHmrrt"
				class="underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white">Discord</a
			>
			and on the downloads page. Join the server to get pinged the moment it releases.
		</p>

		<p class="text-xl font-semibold">Does it have extra maps or mods?</p>
		<p>
			Not included as part of the base game. Gorilla Tag: Classic is meant to harness the simplicity
			of this era of Gorilla Tag, and thus extra content like this is encouraged to thrive in community modding efforts instead.
		</p>

		<p class="text-xl font-semibold">How do servers work?</p>
		<p>
			Instead of a centralised cluster of servers, anyone can host their own server with their own
			rules, settings, and mods. We run a "Master Server" that acts as a server list, which is how
			people discover your server. Selfhosting is meant to be as easy as possible -- you just run a
			single file.
		</p>

		<p class="text-xl font-semibold">Do the rules apply to me?</p>
		<p>
			In-game, it's a good idea to follow the code of conduct so you don't get kicked or banned. If
			you host a server and want it listed on our master server, you also have to follow our
			<a href="/rules" class="underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
				>server rules</a
			>.
		</p>

		<p class="text-xl font-semibold">Will it work on my headset?</p>
		<p>Probably. GT:Classic has been tested on:</p>
		<ul>
			<li>• Oculus Quest 3</li>
			<li>• Oculus Quest 3s</li>
			<li>• Oculus Quest 2</li>
			<li>• Oculus Quest 1</li>
			<li>• Valve Index</li>
		</ul>
		If your headset isn't on this list, tell us whether it works in the<a
			href="https://discord.gg/YJxVwHmrrt"
			class="underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white">Discord</a
		>
		and we'll add it to the list!

		<p class="text-xl font-semibold">How can I help?</p>
		<p>
			We're always happy to have contributors! Once the game releases you can stop by the
			<a
				href="https://discord.gg/YJxVwHmrrt"
				class="underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white">Discord</a
			>
			, or the
			<a
				href="https://git.soweli.uk/GTClassic"
				class="underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white">Git</a
			> if you'd like to contribute!
		</p>
		<p class="text-xl font-semibold">Is there a standalone build?</p>
		<p>
			A standalone build is planned. You will need to sideload it, since we will not release it on
			the Oculus store.
		</p>
	</div>
</Window>
