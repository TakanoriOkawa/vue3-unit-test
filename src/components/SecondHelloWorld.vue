<script setup>
import { ref, reactive } from "vue";

const num = ref(0);

const state = reactive({
  count: 1,
});

const numUp = () => {
  num.value++;
};

const stateUp = () => {
  state.count++;
}
</script>

<template>
  <h2>初めてのコンポーネント</h2>
  <p>Ref Count: {{ num }}</p>
  <p>Reactive Count: {{ state.count }}</p>
  <button @click="numUp">カウントアップボタン</button>
  <button @click="stateUp">ステート管理アップボタン</button>
</template>
