<script>

  import AddParticipant from "./addParticipant.svelte";
  import ChatHeader from "./chatHeader.svelte";
  import ChatWindow from "./chatWindow.svelte";
  import ChatWindowLayout from "./chatWindowLayout.svelte";
  import SendMessage from "./sendMessage.svelte";
</script>

<ChatWindowLayout>
  <svelte:fragment slot="header">
    <ChatHeader>
      <slot:fragment slot="trail"> <AddParticipant /></slot:fragment>
    </ChatHeader>
  </svelte:fragment>
  <ChatWindow />
  <svelte:fragment slot="footer">
    <SendMessage />
  </svelte:fragment>
</ChatWindowLayout>
