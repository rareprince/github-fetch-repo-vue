<template>
<div>
          <input type="text" v-model="username" placeholder="username" />
        </div>
        <div>
          <button @click="fetchRepo" :disabled="!username">Fetch Repository</button>
        </div>

</template>

<script>
import { ref } from 'vue';
export default {
    setup() {
        const username = ref("");

        return { username }
    }
};

</script>