<script lang="ts">
	import Window from '$lib/components/Window.svelte';
</script>

<Window title="Downloads" classes="flex-1 h-fit">
	<div class="text-shadow-black/5 text-shadow-md">
		<p class="text-2xl font-bold">Downloads for GTClassic 1.0.0</p>
		<p>
			You probably want the launcher. Although there is the option to host a master server, its
			really not recommended.
		</p>
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
				<img
					src="icons/places/network-server-database.svg"
					alt="Downloads Icon"
					class="w-12 h-12"
				/>
				<div class="flex flex-col text-left">
					<p class="text-lg font-bold m-0 p-0 leading-tight">Download GT:Classic Master Server</p>
					<p class="text-xs opacity-75 m-0 p-0 leading-tight block italic">1.0.0, Windows</p>
				</div>
			</button>
		</div>
	</div>
</Window>
