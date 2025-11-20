<script setup>
import '~/assets/css/about.css';

const stats = [
    { number: '500+', label: 'Heures de pratique', icon: '⏱️' },
    { number: '+45', label: 'CTF complétés', icon: '🚩' },
    { number: '15', label: 'Projets réalisés', icon: '🎯' },
    { number: '∞', label: 'Motivation', icon: '🔥' }
];

</script>

<template>

    <div class="about grid-overlay">
        <div class="a-container">
            <div class="a-header">
                <h1 class="a-title">A propos de moi</h1>
                <div class="a-subtitle">Passionné par la sécurité offensive et la protection des systèmes</div>
            </div>

            <div class="a-grid">
                <div class="a-card a-main">
                    <div class="card-glow"></div>
                    <div class="a-text">
                        <h2>🛡️ Mon parcours</h2>
                        <p>
                            Depuis mes débuts dans le monde de la cybersécurité, j'ai développé une passion dévorante
                            pour le <span class="highlight">pentesting</span> et le <span
                                class="highlight">renseignement</span>.
                            Chaque CTF est une nouvelle énigme à résoudre, chaque système une forteresse à comprendre.
                        </p>
                        <p>
                            Ma philosophie : <strong>comprendre pour mieux protéger</strong>. Je ne me contente pas
                            d'apprendre
                            les outils, je cherche à maîtriser les concepts fondamentaux qui régissent la sécurité
                            informatique.
                        </p>
                    </div>
                </div>

                <div class="a-stats-grid">
                    <div class="a-stat" v-for="stat in stats" :key="stat.label">
                        <div class="stat-icon">{{ stat.icon }}</div>
                        <div class="stat-number">{{ stat.number }}</div>
                        <div class="stat-label">{{ stat.label }}</div>
                        <div class="stat-glow"></div>
                    </div>
                </div>

                <div class="a-card a-goals">
                    <div class="card-glow"></div>
                    <h2>🎯 Objectifs</h2>
                    <div class="goals-list">
                        <div class="goal-item">
                            <span class="goal-bullet">›</span>
                            <span>Réussir une intrusion physique simulée (avec autorisation)</span>
                        </div>
                        <div class="goal-item">
                            <span class="goal-bullet">›</span>
                            <span>Contribuer à des projets open-source en cybersécurité</span>
                        </div>
                        <div class="goal-item">
                            <span class="goal-bullet">›</span>
                            <span>Concevoir et assembler un toolkit de pentesting complet et portable</span>
                        </div>
                        <div class="goal-item">
                            <span class="goal-bullet">›</span>
                            <span>Créer et animer un atelier sur la cybersécurité.</span>
                        </div>
                    </div>
                </div>

                <div class="a-card a-interests">
                    <div class="card-glow"></div>
                    <h2>⚡ Centres d'intérêt</h2>
                    <div class="interests-tags">
                        <span class="interest-tag">OSINT</span>
                        <span class="interest-tag">Forensic</span>
                        <span class="interest-tag">Web Security</span>
                        <span class="interest-tag">Network Analysis</span>
                        <span class="interest-tag">Pentesting</span>
                        <span class="interest-tag">Teaching</span>
                        <span class="interest-tag">Developement</span>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>