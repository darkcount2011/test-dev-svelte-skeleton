<section class="max-h-full gap-1">
	<div class=" top-0 sticky card bg-surface-200-700-token rounded-none p-2 shadow-lg">
		<slot name="header" />
	</div>
	<div class="p-4 h-full">
		<slot />
	</div>
	<div class="w-full bottom-0 fixed border-l border-t border-surface-400/40">
		<slot name="footer" />
	</div>
</section>

<style language="postcss">
	.chat-window {
		background-color: --color-surface-800;
		background-image: radial-gradient(
				at 11% 14%,
				rgba(var(--color-secondary-500) / 0.2) 0px,
				transparent 50%
			),
			radial-gradient(at 11% 14%, rgba(var(--color-primary-500) / 0.1) 0px, transparent 50%);
	}
</style>
