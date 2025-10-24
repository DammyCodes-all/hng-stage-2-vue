<script setup lang="ts">
import { ref } from "vue";

const newTask = ref<string>("");
const submitTask = () => {
  console.log(newTask.value);
};
</script>

<template>
  <main class="max-w-[1440px] mx-auto min-h-dvh">
    <section class="w-1/2 mx-auto bg-gray-500 p-4">
      <h1>Task App</h1>
      <p>New Task</p>
      <form
        class="flex w-full gap-2 justify-between items-center"
        @submit.prevent="submitTask"
      >
        <input
          v-model="newTask"
          type="text"
          class="h-10 bg-transparent border-2 border-blue-700 outline-0 p-2 w-full"
        />
        <button class="cursor-pointer" type="submit">Add</button>
      </form>
    </section>
  </main>
</template>
