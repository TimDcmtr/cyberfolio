<script setup>
import '~/assets/css/style.css'

useHead({
  title: "leMecha - Portfolio",
})
</script>

<template>
    <div>
        <AppHeader />
        <slot />
        <AppFooter />
    </div>
</template>
