<script setup lang="ts">
definePageMeta({
  layout: false,
});
useHead({
  title: 'My App',
  meta: [
    { name: 'description', content: 'My amazing site.' }
  ],
  bodyAttrs: {
    class: 'test'
  },
  script: [ { innerHTML: 'console.log(\'Hello world\')' } ]
});
</script>

<template>
  <div>
    <NuxtLayout name="custom">

        <template #header><p class="text-7xl font-bold pt-5">Homepage</p></template>
        <template #main> 
            <p class="text-3xl">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vestibulum erat eu leo malesuada, eu semper nibh ultrices. Suspendisse leo felis, viverra a urna quis, lobortis dictum dui. Vestibulum semper arcu odio, et pharetra leo varius nec. In sem sem, tempus a felis eu, sodales mattis lectus. In quis placerat ipsum. Vivamus at diam imperdiet ligula lacinia condimentum eget eu urna. Sed nisi risus, interdum ut faucibus vitae, tempor euismod justo. Mauris non pretium magna. Praesent ex diam, rutrum ac libero eget, pretium scelerisque elit. Curabitur mollis tortor id velit venenatis tristique.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur vestibulum erat eu leo malesuada, eu semper nibh ultrices. Suspendisse leo felis, viverra a urna quis, lobortis dictum dui. Vestibulum semper arcu odio, et pharetra leo varius nec. In sem sem, tempus a felis eu, sodales mattis lectus. In quis placerat ipsum. Vivamus at diam imperdiet ligula lacinia condimentum eget eu urna. Sed nisi risus, interdum ut faucibus vitae, tempor euismod justo. Mauris non pretium magna. Praesent ex diam, rutrum ac libero eget, pretium scelerisque elit. Curabitur mollis tortor id velit venenatis tristique.</p>

        </template>
        <template #footer> The footer of the page </template>

    </NuxtLayout>
  </div>
</template>