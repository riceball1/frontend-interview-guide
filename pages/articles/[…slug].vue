<template>
  <div>
    <main>
      <ContentDoc v-slot="{ doc }">
        <div class="mb-12 border-b-2 border-neutral-700">
          <h1 class="text-5xl">{{ doc.title }}</h1>
          <p>{{ doc.description }}</p>
          <NuxtLink to="/">Back Home</NuxtLink>
        </div>

        <ContentRenderer :value="doc" />
      </ContentDoc>
    </main>
    <Footer />
  </div>
</template>
