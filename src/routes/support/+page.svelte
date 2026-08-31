<script lang="ts">
	import Window from '$lib/components/Window.svelte';
</script>

<Window title="Support" classes="flex-1 h-fit w-full">
	{#snippet icon()}
		<img src="/icons/apps/help-browser.svg" alt="Life Buoy Icon" class="w-6 h-6" />
	{/snippet}
	<div class="text-shadow-black/5 text-shadow-md">
		<p class="text-2xl font-bold">Support</p>
		<p>
			Need a hand? The best place to get help is our
			<a
				href="https://discord.gg/YJxVwHmrrt"
				class="underline hover:no-underline hover:text-black text-[#2b375a]">Discord server</a
			>. That's where the community and the devs hang out, and where you're most likely to get a
			quick answer to whatever's going wrong.
		</p>

		<p class="text-xl font-semibold">Bugs &amp; issues</p>
		<p>
			Found a bug? Hop into Discord and let us know! Screenshots, logs, and the steps to reproduce
			it all help us track it down.
		</p>

		<p class="text-xl font-semibold">Hosting a server</p>
		<p>
			Stuck setting up your own server? The docs and the community are a great starting point, and
			folks in Discord are happy to walk you through it. If your server isn't showing up on the
			master server list, double check that you're following the
			<a href="/rules" class="underline hover:no-underline hover:text-black text-[#2b375a]"
				>server rules</a
			>.
		</p>

		<p class="text-xl font-semibold">Moderation &amp; reports</p>
		<p>
			Moderation is entirely up to server owners. Since there are no accounts, we cannot globally
			ban anyone.
		</p>

		<p class="text-xl font-semibold">Donate</p>
		<p>
			GT:Classic is a community project and always will be. We don't charge for anything and we
			never will. If you'd like to keep things running, the best help is spreading the word and
			contributing. We do not accept donations.
		</p>
	</div>
</Window>
