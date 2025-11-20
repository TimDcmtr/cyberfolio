<script setup>
import '~/assets/css/style.css'
import icon from '~/assets/images/icon.png';

useHead({
  title: "leMecha - Portfolio",
  link: [
    { rel: 'icon', type: 'image/png', href: icon }
  ]
})
</script>

<template>
    <div>
        <AppHeader />
        <slot />
        <AppFooter />
    </div>
</template>
