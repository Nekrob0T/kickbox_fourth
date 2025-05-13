<template>
  <base-block
    class="contact"
    variant="tertiary"
  >
    <h3>Masz pytanie? Chcesz rozpocząć trening?</h3>
    <form @submit.prevent="submitForm">
      <input
        type="text"
        required
        name="name"
        placeholder="Twoje imię"
      >
      <input
        type="email"
        required
        name="email"
        placeholder="Twój email"
      >
      <textarea
        name="comment"
        required
        placeholder="Twoje pytanie"
      />
      <base-button
        type="submit"
        label="Napisz mnie"
      />
    </form>
  </base-block>
</template>

<script setup lang="ts">
import { BaseBlock, BaseButton } from '@/components/base';

function submitForm() {
  alert('Odesłano');
}
</script>

<style scoped lang="sass">
.contact
  display: flex
  flex-direction: column
  gap: 1.5rem

  form
    display: flex
    flex-direction: column
    gap: 1.5rem

  input,
  textarea
    font-size: 1.5rem
    line-height: 1.5rem
    border-radius: .25rem
    padding: .75rem

  input
    height: 40px

  textarea
    resize: none
    height: 200px

  :deep(.base-button)
    color: white
</style>
