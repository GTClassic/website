<script lang="ts">
	import type { Snippet } from 'svelte';

	let {
		children,
		icon,
		classes = '',
		title = ''
	}: { children: Snippet; icon?: Snippet; classes?: string; title?: string } = $props();
</script>

<div
	class=" bg-white/75 border-black/50 shadow-black/50 shadow-lg border rounded-md w-fit overflow-clip {classes}"
>
	<div
		class="p-2 text-white font-bold text-shadow-black text-shadow-lg w-full bg-[linear-gradient(0deg,rgba(0,0,0,0.85)_0%,rgba(41,41,41,0.85)_50%,rgba(84,84,84,0.85)_50%,rgba(163,163,163,0.85)_100%)]"
	>
		<p class="flex items-center gap-2">
			{#if icon}
				{@render icon()}
			{/if}
			{title}
		</p>
	</div>
	<div class="p-2">
		{@render children()}
	</div>
</div>
