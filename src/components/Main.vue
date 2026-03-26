<script setup lang="ts">
import { ref } from "vue";

const array = ref([
  {
    ajdective: "Lightweight",
    description:
      "I am incredibly small and fast! My core library is only around 30KB, so I won't slow you down.",
  },
  {
    ajdective: "Approachable",
    description:
      "Easy to learn and use, even for beginners. I have a gentle learning curve, clear documentation, and a supportive community.",
  },
  {
    ajdective: "Versatile",
    description:
      "I can handle everything from simple interactive elements to complex single-page applications. I'm great for small projects and large-scale applications alike.",
  },
]);
</script>

<template>
  <main>
    <section>
      <h2>
        I'm <span class="highlight">{{ array[0]?.ajdective }}</span>
      </h2>
      <p>
        {{ array[0]?.description }}
      </p>
    </section>
    <section>
      <h2>
        I'm <span class="highlight">{{ array[1]?.ajdective }}</span>
      </h2>
      <p>
        {{ array[1]?.description }}
      </p>
    </section>
    <section>
      <h2>
        I'm <span class="highlight">{{ array[2]?.ajdective }}</span>
      </h2>
      <p>
        {{ array[2]?.description }}
      </p>
    </section>
  </main>
</template>

<style scoped>
/* MAIN CSS */
main {
  margin-top: 15px;
}

section {
  margin-top: 25px;
}

h2 {
  font-size: 1.3rem;
  color: #34495e;
  margin-bottom: 3px;
}

p {
  font-size: 0.9rem;
  color: #555;
}
/**********/
</style>
