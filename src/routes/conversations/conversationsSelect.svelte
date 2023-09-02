<script>
  import { Avatar } from "@skeletonlabs/skeleton";
  import { fly, slide } from "svelte/transition";
  let conversations = [
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
    { name: "John Doe", label: "John Doe" },
    { name: "Jane Doe", label: "Jane Doe" },
  ];
</script>

<div
  class="grid grid-flow-row overflow-y-scroll h-full gap-2 p-2 border-2"
  tabindex="-1"
  in:fly={{ y: 100, duration: 500 }}
>
  {#each conversations as conversationUser, i}
    <div>
      <button type="button" class="w-full p-1 gap-3 rounded-md flex">
        <Avatar initials={conversationUser.name} width=" w-12" />
        <span class="place-self-center">{conversationUser.label}</span>
      </button>
    </div>
    <div data-popup="conversationOptions" />
  {/each}
</div>
