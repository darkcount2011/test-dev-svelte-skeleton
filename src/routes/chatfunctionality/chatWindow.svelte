<script>

	// big list of messages (30)
	 let messages = ['hey', 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Vitae congue mauris rhoncus aenean vel. Enim sed faucibus turpis in eu mi bibendum. Tristique magna sit amet purus gravida. Tellus cras adipiscing enim eu turpis egestas pretium aenean pharetra. Blandit volutpat maecenas volutpat blandit aliquam etiam erat velit. Mattis rhoncus urna neque viverra justo nec ultrices. Vitae turpis massa sed elementum tempus egestas sed. Curabitur gravida arcu ac tortor dignissim convallis aenean et. Vel pharetra vel turpis nunc eget. Tellus at urna condimentum mattis pellentesque id nibh tortor id. Cras adipiscing enim eu turpis egestas pretium aenean pharetra.'];

</script>

<div class="grid ">
	{#each messages as message, i}
			<div class="place-self-end lg:max-w-xl max-w-md">
				<div class=" p-4 rounded-tr-none rounded-3xl bg-primary-500/30">
					<header class="flex justify-between items-center" />
					<p>{message}{message}{message}</p>
				</div>
			</div>
			<div class="place-self-start lg:max-w-4xl max-w-md">
				<div class=" p-4 rounded-tl-none rounded-3xl bg-surface-400/30">
					<header class="flex justify-between items-center" />
					<p>{message}{message}{message}</p>
				</div>
			</div>
	{/each}
</div>
