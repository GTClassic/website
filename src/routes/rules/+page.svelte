<script lang="ts">
	import Window from '$lib/components/Window.svelte';
</script>

<Window title="Rules" classes="flex-1 h-fit  w-full">
	{#snippet icon()}
		<img src="/icons/actions/small/48x48/help-about.svg" alt="Error Icon" class="w-6 h-6" />
	{/snippet}
	<div class="text-shadow-black/5 text-shadow-md">
		<p class="text-2xl font-bold">Rules</p>
		<p>
			Generally it is a good idea to follow the in-game code of conduct as to not get yourself
			kicked or banned from servers, but we also have rules specific to hosting servers, which can be seen in-game.
		</p>
		<!--
		<hr class="my-2" />

		<p class="text-xl">Master server rules</p>

		<ul>
			<li>No slurs or offensive language in your server name.</li>
			<li>to be continued idfk</li>
			TODO: agree on a set of rules for server hosting
		</ul>
		-->
	</div>
</Window>
