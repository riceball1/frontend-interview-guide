<template>
  <footer>
    <p>Copyright &#169; 2023</p>
    <p>
      This is an open sourced document made free for all to use, please do not
      attempt to monetize any parts of the content. <br />
      These documents are meant to be open and free knowledge for sharing.
    </p>
    <p>
      <a href="https://github.com/riceball1/frontend-interview-guide"
        target="_blank">Github Repo</a
      >
    </p>
  </footer>
</template>

<style scoped>
/* sticky footer */
footer {
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  background-color: black;
  color: white;
  text-align: center;
  font-size: 0.8rem;
}
</style>

<script>
export default {
  name: "Footer",
};
</script>
