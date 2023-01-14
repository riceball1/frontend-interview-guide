<template>
    <div class="container">
     <Header/>
      <CBox
        d="flex"
        flex-dir="column"
        justify-content="center"
      >
      FE System
      </CBox>
      <Footer/>
    </div>
  </template>
  
  <script lang="js">
  import { CBox, CButton, CFlex, CHeading } from "@chakra-ui/vue";
  
  export default {
    name: "system",
    components: {
      CBox,
      CButton,
      CFlex,
      CHeading,
    }
  }
 
  </script>
  