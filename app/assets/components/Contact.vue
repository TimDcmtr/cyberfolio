<script setup>

import '~/assets/css/contact.css';

const contactMethods = [
  { icon: '📧', label: 'Email', value: 'contact@tim-d.fr', link: 'mailto:contact@tim-d.fr' },
  { icon: '💼', label: 'LinkedIn', value: '/in/timeo.d', link: 'https://linkedin.com/in/timeo-d' },
  { icon: '🐙', label: 'GitHub', value: 'TimDcmtr', link: 'https://github.com/TimDcmtr' },
  { icon: '📱', label: 'Signal', value: '@tim.34', link: 'https://signal.me/#eu/9lzMrtoBd0Suj5qj7_llAIghzrS0X7vi-wncC0mESylzXBXbKnJB1bCPo5qlQlN7' }
];

</script>

<template>

    <div class="contact">
        <div class="c-container">
            <div class="c-header">
                <h1 class="c-title">Restons en contact</h1>
                <div class="c-subtitle">N'hésitez pas à me contacter pour discuter de cybersécurité, de projets ou
                    d'opportunités</div>
            </div>

            <div class="c-content">
                <div class="c-info-card">
                    <div class="card-glow"></div>
                    <div class="c-intro">
                        <h2>📬 Contactez-moi</h2>
                        <p>
                            Je suis toujours intéressé par de nouvelles opportunités, des collaborations sur des projets
                            de sécurité, ou simplement échanger sur les dernières vulnérabilités découvertes.
                        </p>
                        <p>
                            Actuellement en recherche active d'un <span class="highlight">stage de 2 mois</span> pour
                            mettre en pratique mes compétences en environnement professionnel.
                        </p>
                    </div>

                    <div class="c-availability">
                        <div class="status-indicator"></div>
                        <span>Disponible immédiatement</span>
                    </div>
                </div>

                <div class="c-methods">
                    <a v-for="method in contactMethods" :key="method.label" :href="method.link" target="_blank"
                        class="c-method">
                        <div class="method-icon">{{ method.icon }}</div>
                        <div class="method-details">
                            <div class="method-label">{{ method.label }}</div>
                            <div class="method-value">{{ method.value }}</div>
                        </div>
                        <div class="method-arrow">→</div>
                        <div class="method-glow"></div>
                    </a>
                </div>
            </div>



            <div class="c-footer">
                <div class="footer-text">
                    Développé avec <span class="heart">❤️</span> et beaucoup de <span class="highlight">caféine</span>
                </div>
                <div class="footer-copyright">
                    © 2025 tim-d.fr • Portfolio Cybersécurité
                </div>
            </div>
        </div>
    </div>

</template>