<script setup>
import '~/assets/css/skills.css';

const skillsList = [{ name: '🔒 Security', desc: ['Pentest', 'OSINT', 'DevSecOps', 'Forensic'] },
{ name: '💻 Development', desc: ['Node.JS', 'HTML/CSS/JS', 'Bash', 'Python'] },
{ name: '☁️ Cloud', desc: ['MySQL', 'MongoDB', 'Stormshield', 'pfSense'] },
{ name: '🛠️ Tools', desc: ['Docker', 'Git', 'GNS3', 'Cisco Packet Tracer'] },

];

</script>


<template>


    <div class="skills">
        <h1 class="s-title">Compétences</h1>
        <div class="s-list">
            <div class="s-item" v-for="c in skillsList">
                <h3>{{ c.name }}</h3>
                <div class="s-desc">
                    <span v-for="n in c.desc">{{ n }}</span>
                </div>
            </div>
        </div>
    </div>

</template>