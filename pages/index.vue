<template>
  <div class="container">
    <Header disableBackButton />
    <!-- <CBox mb="3">
        <CIconButton
          mr="3"
          :icon="colorMode === 'light' ? 'moon' : 'sun'"
          :aria-label="`Switch to ${
            colorMode === 'light' ? 'dark' : 'light'
          } mode`"
          @click="toggleColorMode"
        />
      </CBox> -->
    <!-- </CFlex> -->
    <CBox d="flex" flex-dir="column" justify-content="center">
      <CFlex mb="3" justify="space-evenly" wrap="wrap">
        <CBox m="4">
          <CHeading text-align="center" as="h2"> Interview Topics </CHeading>
          <ul>
            <li>Frontend Coding Challenges</li>
            <li>
              <NuxtLink to="/system"> Frontend System Design </NuxtLink>
            </li>
            <li>Frontend Technical Behavioral</li>
            <li>Frontend Take-Home Assignments</li>
            <li>General DSA and Algo Coding Challenges</li>
          </ul>
        </CBox>
        <CBox>
          <CHeading text-align="center" as="h2"> Other Topics </CHeading>

          <ul>
            <li>Resources List</li>
            <li>Data Structures and Algorithms</li>
            <li>Frontend Performance</li>
          </ul>
        </CBox>
      </CFlex>
    </CBox>
    <Footer />
  </div>
</template>

<style scoped>
/* home route and active route will show in bold as it matches / and /about */
a.nuxt-link-active {
  font-weight: bold;
}
/* exact link will show the primary color for only the exact matching link */
a.nuxt-link-exact-active {
  color: #00c58e;
}
</style>

<script lang="js">
import { CBox, CButton, CFlex, CHeading, CIconButton } from "@chakra-ui/vue";

export default {
  name: "IndexPage",
  components: {
    CBox,
    CButton,
    CFlex,
    CHeading,
  },
  inject: ["$chakraColorMode", "$toggleColorMode"],
    data() {
      return {
        showModal: false,
        mainStyles: {
          dark: {
            bg: "gray.700",
            color: "whiteAlpha.900",
          },
          light: {
            bg: "whiteAlpha.100",
            color: "gray.900",
          },
        },
      };
    },
    computed: {
      colorMode() {
        return this.$chakraColorMode();
      },
      theme() {
        return this.$chakraTheme();
      },
      toggleColorMode() {
        console.log('toggle colorMode')
        // return this.$toggleColorMode;
      },
    },
};
</script>
