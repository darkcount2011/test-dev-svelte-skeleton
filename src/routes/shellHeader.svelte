<script>
  import { AppBar, LightSwitch } from "@skeletonlabs/skeleton";
</script>

<div>
  <AppBar
    gridColumns="grid-cols-3"
    slotDefault="place-self-center"
    slotTrail="place-content-end"
    slotLead="place-content-start"
    border="border-b-1 border-surface-600-300-token shadow-lg"
  >
    <svelte:fragment slot="lead">
      <div class="grid grid-flow-col gap-4">
        <a href="/"><div class="hidden md:grid" /> </a>
      </div></svelte:fragment
    >
    <svelte:fragment slot="default">
      <!-- <div>
			<button class="btn variant-ghost-tertiary" on:click={mockCall}
			>{$incomingCall ? 'Mock incoming call' : 'Mock incoming call off'}</button
			>
			<button class="btn variant-ghost-tertiary" on:click={mockActiveCall}
			>{$activeCall ? 'mock active call' : 'Mock inactive call'}</button
			>
		</div> -->
    </svelte:fragment>
    <svelte:fragment slot="trail">
      <button class="btn variant-filled-secondary">Call Window </button>
      <button class="btn variant-filled-primary animate-pulse"
        >Incoming Call</button
      >
      <div class="grid grid-flow-col gap-3">
        <LightSwitch />
      </div>
    </svelte:fragment>
  </AppBar>
</div>

<style lang="postcss">
  .btn {
    @apply text-sm;
  }
</style>
