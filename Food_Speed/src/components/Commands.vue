<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
    <div class="commands">
        <h1>Commandes</h1>
        <WelcomeItem
        title="Documentation"
        text="Find in-depth information about Vue features and API."
        >
        <DocumentationIcon />
        </WelcomeItem>
        <WelcomeItem
        title="Tooling"
        text="Discover tooling and recommendations on how to use them."
        >
        <ToolingIcon />
        </WelcomeItem>
        <WelcomeItem
        title="Ecosystem"
        text="Learn about the libraries and official projects that make up the Vue ecosystem."
        >
        <EcosystemIcon />
        </WelcomeItem>
        <WelcomeItem
        title="Community"
        text="Join a welcoming and diverse community."
        >
        <CommunityIcon />
        </WelcomeItem>
        <WelcomeItem
        title="Support"
        text="Find out how to get help from the community and maintainers."
        >
        <SupportIcon />
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