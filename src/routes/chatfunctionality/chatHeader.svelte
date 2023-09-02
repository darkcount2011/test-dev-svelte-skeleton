<script>
  import { Avatar } from "@skeletonlabs/skeleton";
</script>

<div class="grid grid-cols-3">
  <div name="Avatar" class="flex gap-2">
    <Avatar initials="Ja" lass="" c background="bg-primary-500/30" />
    <div class="place-self-start">
      <span class="text-lg font-bold">Jane Doe</span>
      <p class="text-sm text-gray-500">(status)</p>
    </div>
  </div>
  <div>
    <slot />
  </div>
  <div class="grid place-self-center">
    <slot name="trail">(icons, whatsapp or sms ... phonecall?)</slot>
  </div>
</div>
