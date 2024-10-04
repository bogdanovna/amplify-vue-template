<script setup lang="ts">
import { Authenticator } from "@aws-amplify/ui-vue";
import "@aws-amplify/ui-vue/styles.css";
</script>

<template>
  <fieldset>
    <legend>Free Content</legend>
    <details>
      <summary>hello</summary>
      <h1>world!</h1>
    </details>
  </fieldset>
  <hr />
  <fieldset>
    <legend>Private Content</legend>
    <details>
      <summary>I'm ready</summary>
      <authenticator>
        <template v-slot="{ signOut }">
          <button @click="signOut">Sign Out</button>
        </template>
      </authenticator>
    </details>
  </fieldset>
</template>
