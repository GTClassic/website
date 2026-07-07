<script lang="ts">
	import Window from '$lib/components/Window.svelte';
</script>

<Window title="Howdy!" classes="flex-1">
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
			<button
				class="
                    flex items-center gap-2
                    text-white
                    bg-[#0064cd]
                    bg-[linear-gradient(to_bottom,#049cdb,#0064cd)]
                    bg-repeat-x
                    [text-shadow:0_-1px_0_rgba(0,0,0,0.25)]
                    border
                    border-[#0064cd]
                    border-b-[#003f81]
                    rounded-md
                    px-2.5 py-2
                    [box-shadow:inset_0_1px_0_rgba(255,255,255,0.1),inset_0_-1px_0_rgba(0,0,0,0.1)]
                    hover:bg-[linear-gradient(to_bottom,#0064cd,#049cdb)]
                    active:[box-shadow:inset_0_2px_4px_rgba(0,0,0,0.15)]
                "
			>
				<img src="/icons/actions/small/48x48/download.svg" alt="Downloads Icon" class="w-12 h-12" />
				<div class="flex flex-col text-left">
					<p class="text-lg font-bold m-0 p-0 leading-tight">Download GT:Classic Launcher</p>
					<p class="text-xs opacity-75 m-0 p-0 leading-tight block italic">1.0.0, Windows</p>
				</div>
			</button>
			<button
				class="
                    flex items-center gap-2
                    text-white
                    bg-[#4d4d4d]
                    bg-[linear-gradient(to_bottom,#666,#4d4d4d)]
                    bg-repeat-x
                    [text-shadow:0_-1px_0_rgba(0,0,0,0.25)]
                    border
                    border-[#4d4d4d]
                    border-b-[#333]
                    rounded-md
                    px-2.5 py-2
                    [box-shadow:inset_0_1px_0_rgba(255,255,255,0.1),inset_0_-1px_0_rgba(0,0,0,0.1)]
                    hover:bg-[linear-gradient(to_bottom,#4d4d4d,#666)]
                    active:[box-shadow:inset_0_2px_4px_rgba(0,0,0,0.15)]
                "
			>
				<img src="icons/places/network-server.svg" alt="Downloads Icon" class="w-12 h-12" />
				<div class="flex flex-col text-left">
					<p class="text-lg font-bold m-0 p-0 leading-tight">Download GT:Classic Game Server</p>
					<p class="text-xs opacity-75 m-0 p-0 leading-tight block italic">1.0.0, Windows</p>
				</div>
			</button>
		</div>
	</div>
</Window>
