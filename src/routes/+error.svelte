<script lang="ts">
	import { page } from '$app/state'; // SvelteKit 2.12+; use '$app/stores' + $page store for older
	import Window from '$lib/components/Window.svelte';

	const messages: Record<number, { title: string; body: string }> = {
		404: {
			title: 'Not Found',
			body: "The page you're looking for no longer exists or has been moved."
		},
		403: {
			title: 'Forbidden',
			body: "You don't have permission to access this page."
		},
		500: {
			title: 'Internal Server Error',
			body: 'An unexpected error occurred on our end.'
		}
	};

	let status = $derived(page.status);
	let info = $derived(
		messages[status] ?? {
			title: `Error ${status}`,
			body: page.error?.message ?? 'Something went wrong.'
		}
	);
</script>

<Window title={info.title} classes="flex-1 h-fit w-full">
	{#snippet icon()}
		<img src="/icons/error.png" alt="Error Icon" class="w-6 h-6" />
	{/snippet}
	<div class="text-shadow-black/5 text-shadow-md">
		<p class="text-2xl font-bold">Oops!</p>
		<p>{info.body}</p>
		<a
			href="/"
			class="flex gap-1 items-center underline hover:no-underline hover:text-black dark:hover:text-white text-[#2b375a] dark:text-white"
			><img src="/icons/actions/go-home.svg" alt="Home Icon" class="w-4 h-4" />Go Home</a
		>
	</div>
</Window>
