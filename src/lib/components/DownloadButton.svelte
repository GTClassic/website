<script lang="ts">
	let {
		icon,
		label,
		subtitle,
		variant = 'secondary',
		onclick
	}: {
		icon: string;
		label: string;
		subtitle: string;
		variant?: 'primary' | 'secondary';
		onclick?: () => void;
	} = $props();

	const variants = {
		primary:
			'bg-[#0064cd] bg-[linear-gradient(to_bottom,#049cdb,#0064cd)] border-[#0064cd] border-b-[#003f81] hover:bg-[linear-gradient(to_bottom,#0064cd,#049cdb)]',
		secondary:
			'bg-[#4d4d4d] bg-[linear-gradient(to_bottom,#666,#4d4d4d)] border-[#4d4d4d] border-b-[#333] hover:bg-[linear-gradient(to_bottom,#4d4d4d,#666)]'
	};
</script>

<button
	{onclick}
	class="
        flex items-center gap-2
        text-white
        bg-repeat-x
        [text-shadow:0_-1px_0_rgba(0,0,0,0.25)]
        border
        rounded-md
        px-2.5 py-2
        [box-shadow:inset_0_1px_0_rgba(255,255,255,0.1),inset_0_-1px_0_rgba(0,0,0,0.1)]
        active:[box-shadow:inset_0_2px_4px_rgba(0,0,0,0.15)]
        {variants[variant]}
    "
>
	<img src={icon} alt="{label} Icon" class="w-12 h-12" />
	<div class="flex flex-col text-left">
		<p class="text-lg font-bold m-0 p-0 leading-tight">{label}</p>
		<p class="text-xs opacity-75 m-0 p-0 leading-tight block italic">{subtitle}</p>
	</div>
</button>
