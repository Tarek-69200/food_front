<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'

</script>

<template>
    <div class="commands">
        <WelcomeItem
        title="Documentation"
        text="Find in-depth information about Vue features and API."
        >
        </WelcomeItem>
        
    </div>
</template>

<style>

@media (min-width: 1024px) {
    .commands {
        min-height: 100vh;
        display: flex;
        align-items: center;
    }
}

</style>