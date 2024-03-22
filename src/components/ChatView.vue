<template>

  <deep-chat
    :demo="true"
    :textInput="{ placeholder: { text: 'Type here...' } }"
    :initialMessages="initialMessages"
  />
</template>

<script>
import "deep-chat";

export default {
  name: "ChatView",
  data() {
    return {
      initialMessages: [
        { role: "ai", text: "Good morning! Can I help you with a clinical question?" },
      ],
    };
  },
};
</script>

<style>
div {
  font-family: sans-serif;
  text-align: center;
  justify-content: center;
  display: grid;
}
</style>
