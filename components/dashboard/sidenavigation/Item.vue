<template>
  <router-link :to="to">
    <span
      class="
        flex
        items-center
        text-gray-200
        justify-start
        my-2
        p-3
        w-full
        hover:text-white
      "
      :class="
        $route.path === to &&
        'border-l-4 border-white lg:border-l-0 lg:border-r-4'
      "
    >
      <span>
        <slot />
      </span>
      <span class="mx-4 text-sm">
        {{ title }}
      </span>
    </span>
  </router-link>
</template>

<script>
export default {
  name: 'SidenavItem',
  props: {
    to: {
      type: String,
      default: '',
    },
    title: {
      type: String,
      default: '',
    },
  },
}
</script>
