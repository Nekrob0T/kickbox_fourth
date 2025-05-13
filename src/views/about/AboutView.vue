<template>
  <base-block
    offset="responsive"
    class="content"
  >
    <h1>Nie urodziłem się mistrzem – stałem się nim dzięki pracy, pasji i determinacji.</h1>
    <p>
      Nazywam się <strong>Piotr Siegoczyński</strong> i od ponad trzech dekad jestem związany ze sportami walki. Moja
      przygoda z kickboxingiem zaczęła się w czasach, gdy ten sport dopiero raczkował w Polsce. Nie było wtedy kamer,
      transmisji na żywo, trenerów personalnych ani mediów społecznościowych. Były tylko maty, rękawice, pot na
      treningach i ogromne marzenia.
    </p>
    <p>
      Od pierwszego treningu wiedziałem, że to nie będzie tylko przygoda — to będzie moje życie. Z każdym kolejnym
      krokiem na sali treningowej budowałem nie tylko technikę, ale charakter. Uczyłem się dyscypliny, pokory, szacunku
      do przeciwnika, i co najważniejsze — walki z samym sobą.
    </p>
    <p>
      Przez lata miałem zaszczyt reprezentować Polskę na najważniejszych arenach międzynarodowych. Zdobywałem tytuły
      <strong>Mistrza Świata, Mistrza Europy</strong> i wielokrotnie <strong>Mistrza Polski</strong>. Każdy z tych
      sukcesów to efekt tysięcy godzin spędzonych na treningach — tych, na które miałem siłę, i tych, na które musiałem
      znaleźć siłę.
    </p>
    <p>
      Ale sport to nie tylko medale. To także momenty zwątpienia, kontuzje, przegrane walki i ciężkie decyzje. Dziś
      wiem, że to właśnie te momenty były najważniejsze. Bo nie ma rozwoju bez kryzysów. Nie ma zwycięstwa bez porażek.
    </p>
    <p>
      Kickboxing nauczył mnie, że najważniejsze walki to te, które toczymy w sobie — ze zmęczeniem, z wymówkami, z
      lenistwem, z brakiem wiary w siebie.
    </p>
    <p>
      Po zakończeniu kariery zawodniczej nie odszedłem ze świata sportu. Dziś jako trener, mentor i motywator pomagam
      innym odnaleźć w sobie siłę, której często nawet nie wiedzą, że posiadają. Pracuję z młodymi zawodnikami,
      amatorami, osobami, które chcą po prostu poczuć się silniejsze — fizycznie i psychicznie.
    </p>
  </base-block>
</template>

<script setup lang="ts">
import { BaseBlock } from '@/components/base';
import { useMeta } from '@/composable/useMeta.ts';

const { titleAuthor } = useMeta();

titleAuthor('Moja droga do mistrzostwa');
</script>

<style scoped lang="sass">
p
  margin-top: 3rem
  font-size: 1.5rem
  line-height: 2rem
</style>
