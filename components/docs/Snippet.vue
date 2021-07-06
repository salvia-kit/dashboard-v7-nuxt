<template>
  <pre
    class="
      font-mono
      text-sm
      px-4
      py-1
      rounded
      overflow-x-auto
      max-w-full
      bg-gray-100
      text-blue-600
      border
    "
  >
    {{ snippets }}
  </pre>
</template>

<script>
export default {
  name: 'Snippet',
  data() {
    return {
      snippets: `<sidenav-items-section name="Applications">
      <sidenav-item title="Users" to="/">
        <users-icon />
      </sidenav-item>

      <sidenav-item title="Medias" to="/admin/medias">
        <medias-icon />
      </sidenav-item>
    </sidenav-items-section>`,
    }
  },
}
</script>
