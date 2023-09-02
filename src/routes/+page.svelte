<script>
  import ConversationInitializer from "./chatfunctionality/conversationInitializer.svelte";
  import ConversationOptionsHeader from "./conversations/conversationOptionsHeader.svelte";
  import ConversationTabSwitch from "./conversations/conversationTabSwitch.svelte";
  import ConversationsSelect from "./conversations/conversationsSelect.svelte";
  import SearchHeader from "./conversations/searchHeader.svelte";
  import SelectPhoneNumber from "./conversations/selectPhoneNumber.svelte";
  import ConversationsLayout from "./conversationsLayout.svelte";
</script>

<ConversationsLayout>
  <svelte:fragment slot="left">
    <ConversationOptionsHeader>
      <slot:fragment slot="lead">
        <h2 class="text-2xl text-center">Chats</h2>
      </slot:fragment>

    </ConversationOptionsHeader>
    <SelectPhoneNumber />
    <ConversationTabSwitch />
    <SearchHeader />
    <ConversationsSelect />
  </svelte:fragment>
  <svelte:fragment slot="right">
    <ConversationInitializer />
  </svelte:fragment>
</ConversationsLayout>
