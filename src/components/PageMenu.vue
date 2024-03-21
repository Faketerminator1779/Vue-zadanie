<template>
    <section class="menu">
        <PageCard img="1" title="Branches" alt="Branches" content="Abstract Branches lets you manage version, and document your designs in one place."/>
        <PageCard img="2" title="Manage your account" alt="Manage your account" content="Configure your account settings, such as yout email, profile details, and password."/>
        <PageCard img="3" title="Manage organizations, teams, and projects" alt="Manage organizations, teams, and projects" content="Use Abstract organizations, teams, and projects to organize your people and your work."/>
        <PageCard img="4" title="Manage biling" alt="Manage biling" content="Change subscriptions and payment details."/>
        <PageCard img="5" title="Authenticate to Abstract" alt="Authenticate to Abstract" content="Set up and Configure SSO, SCIM, and Just-in-Time provisioning."/>
        <PageCard img="6" title="Abstract support" alt="Abstract support" content="Get in touch with a human."/>
    </section>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import PageCard from './PageCard.vue'

@Options({
  components: {
    PageCard,
  },
})
export default class App extends Vue {}
</script>