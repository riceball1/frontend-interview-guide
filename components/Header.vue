<template>
  <header>
    <CBox p="10">
      <CHeading as="h1" text-align="center" m="4">
        ⚡️ Frontend Interview Guide
      </CHeading>
      <NuxtLink to="/" v-if="!disableBackButton"> Go to Main Page </NuxtLink>
    </CBox>
  </header>
</template>

<script lang="js">
import { CBox, CButton, CFlex, CHeading } from "@chakra-ui/vue";

export default {
  name: "Header",
  components: {
    CBox,
    CButton,
    CFlex,
    CHeading,
  },
  props: {
    disableBackButton: {
      type: Boolean,
      default: false
    }
  },

};
</script>
