<template>
  <div class="column">
    <NuxtLink :to="to">
      <div class="card">
        <header class="card-header">
          <p class="card-header-title">
            {{ title }}
          </p>
        </header>
        <div class="card-content">
          <div class="content has-text-centered">
            <b-icon :icon="icon" size="is-large" type="is-primary" />
          </div>
        </div>
        <footer class="card-footer">
          <div class="card-footer-item">
            <span>
              <slot />
            </span>
          </div>
        </footer>
      </div>
    </NuxtLink>
  </div>
</template>
<script>
export default {
  props: {
    to: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
    icon: {
      type: String,
      required: true,
    },
  },
}
</script>
<style scoped>
.card {
  transition: transform 0.2s ease;
}
.card:hover {
  transform: translateY(-4px);
}
</style>
