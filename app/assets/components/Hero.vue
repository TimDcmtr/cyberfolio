<script setup>
import '~/assets/css/hero.css';
import me from '~/assets/images/me.png';
</script>

<template>

    <div class="h-bg grid-overlay">
        <div class="hero">
            <div class="h-hiring">
                <h1>⇀ Recherche un stage de 2 mois</h1>
            </div>

            <div class="h-name">
                <h1>leMecha</h1>
                <h3>Cybersecurity</h3>
            </div>
        </div>

        <img :src="me" alt="">
    </div>

</template>