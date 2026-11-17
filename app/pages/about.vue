<!-- About page: proves the same header/footer appear on a different page -->
<template>
  <section>
    <h1>About</h1>

    <div class="grid">
      <InfoCard
        title="Purpose"
        description="A simple site that demonstrates component-based development."
      />
      <InfoCard
        title="Components Used"
        description="AppHeader, AppFooter, StudentCard, InfoCard, and AppButton."
      />
    </div>

    <div class="actions">
      <AppButton label="Delete (red demo)" color="red" />
      <AppButton label="Save (blue demo)" color="green" />
    </div>
  </section>
</template>

<style scoped>
.actions { margin-top: 24px; display: flex; gap: 12px; }
</style>
