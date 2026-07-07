<script lang="ts">
	import Window from '$lib/components/Window.svelte';
</script>

<Window title="404s and Heartbreak" classes="flex-1 h-fit">
	<div class="text-shadow-black/5 text-shadow-md">
		<p class="text-2xl font-bold">Oops!</p>
		<p>The page you're looking for no longer exists or has been moved.</p>
		<a
			href="/"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black text-[#2b375a]"
			><img src="/icons/actions/go-home.svg" alt="Home Icon" class="w-4 h-4" />Go Home</a
		>
	</div>
</Window>
