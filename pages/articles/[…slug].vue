<template>
  <div>
    <main>
      <ContentDoc v-slot="{ doc }">
        <ContentRenderer :value="doc" />
      </ContentDoc>
    </main>
    <Footer />
  </div>
</template>
