<template>
  <ul class="mt-6 md:pl-6">
    <li>
      <div class="mb-10">
        <div class="font-thin pl-5 text-white mb-6 uppercase lg:pl-6">
          {{ name }}
        </div>
        <slot />
      </div>
    </li>
  </ul>
</template>

<script>
export default {
  name: 'SidenavItemsSection',
  props: {
    name: {
      type: String,
      default: '',
    },
  },
}
</script>
