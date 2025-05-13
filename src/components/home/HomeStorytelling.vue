<template>
  <div class="storytelling">
    <base-block
      v-for="(item, i) in stories"
      :key="i"
      variant="tertiary"
      class="storytelling__card"
      offset="offset"
    >
      <h3>{{ item.title }}</h3>
      <p>{{ item.description }}</p>
    </base-block>
  </div>
  <base-block
    variant="tertiary"
    class="mental"
    offset="offset"
  >
    <h3>Siła fizyczna przemija, ale siła charakteru zostaje - Moje 5 zasad mentalnych</h3>
    <ol>
      <li>Pokora – zawsze ucz się, nawet jako mistrz.</li>
      <li>Konsekwencja – nie musisz być szybki, ale musisz być wytrwały.</li>
      <li>Szacunek – do rywala, trenera, samego siebie.</li>
      <li>Obecność – każdy trening to spotkanie ze sobą.</li>
      <li>Wdzięczność – za możliwość bycia lepszym niż wczoraj.</li>
    </ol>
  </base-block>
</template>

<script lang="ts" setup>
import { BaseBlock } from '@/components/base';

const stories = [
  {
    title: 'Czym jest dla mnie sport',
    description:
      'Sport to nie tylko rywalizacja. To przede wszystkim samodyscyplina, szacunek i codzienna praca nad sobą. Przez lata nauczyłem się, że największe zwycięstwa rozgrywają się wewnątrz nas.',
  },
  {
    title: 'Jak trenuję innych',
    description:
      'Każdy z nas ma inny cel i inną drogę. Moim zadaniem jest pomóc Ci ją odnaleźć i przejść. Niezależnie od wieku, poziomu czy doświadczenia — stawiam na indywidualne podejście i wzmacnianie nie tylko ciała, ale i charakteru.',
  },
  {
    title: 'Dlaczego warto mi zaufać',
    description:
      '30 lat na ringu. Mistrz świata. Trener z pasją. Ale przede wszystkim — człowiek, który nie przestaje się uczyć i słuchać innych. Sukces to nie przypadek – to konsekwencja wartości, które wyznaję od początku.',
  },
];
</script>

<style scoped lang="sass">
.storytelling
  display: flex
  flex-direction: column
  gap: 1.5rem

  &__card
    width: 100%
    display: flex
    flex-direction: column
    gap: 1.5rem
    justify-content: space-between

.mental
  h3
    margin-bottom: 1.5rem

  li
    margin-bottom: .5rem
</style>
