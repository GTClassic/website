<script lang="ts">
	import Window from '$lib/components/Window.svelte';
	import DownloadButton from '$lib/components/DownloadButton.svelte';
</script>

<Window title="Downloads" classes="flex-1 h-fit w-full">
	<div class="text-shadow-black/5 text-shadow-md">
		<p class="text-2xl font-bold">Downloads for GTClassic 1.0.0</p>
		<p class="italic text-black/50 text-shadow-black/10 text-shadow-lg">
			tl:dr; you probably want the launcher.
		</p>
		<p class="text-xl">What are all the downloads?</p>

		<ul>
			<li>Launcher - The game itself. Download this one if you want to play GT:Classic.</li>
			<li>
				Game Server - Download this one if you wish to host a server for other people to play on.
			</li>
			<li>
				Master Server - Acts as essentially a server list, and is how people will discover your
				server. Not recommended to host for multiple reasons.
			</li>
		</ul>
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
			<DownloadButton
				icon="icons/places/network-server-database.svg"
				label="Download GT:Classic Master Server"
				subtitle="1.0.0, Windows"
			/>
		</div>
	</div>
</Window>
