<script setup>
import { ref } from "vue";

let id = 0;

const thingToDo = ref("");
const addedThing = ref([
  { id: id++, text: "Bli bäst på front-end utveckling", completed: false },
]);

function addThingToDo() {
  addedThing.value.push({ id: id++, text: thingToDo.value, completed: false });
  thingToDo.value = "";
}

function removeThingToDo(activity) {
  addedThing.value = addedThing.value.filter((t) => t !== activity);
}
</script>

<template>
  <h1>Andreas att göra-lista</h1>
  <main>
    <div class="top">
      <input
        class="inputField"
        placeholder="Vad ska göras?"
        v-model="thingToDo"
        @keyup.enter="addThingToDo"
      />
      <button class="add" @click="addThingToDo">+</button>
    </div>
    <div class="listItem" v-for="activity in addedThing" :key="activity.id">
      <input class="done" type="checkbox" v-model="activity.completed" />
      <span :class="{ completed: activity.completed }">{{
        activity.text
      }}</span>
      <button class="delete" @click="removeThingToDo(activity)">❌</button>
    </div>
  </main>
</template>