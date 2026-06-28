* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
    color: #fff;
    overflow-x: hidden;
}

.page {
    display: block;
    animation: fadeIn 0.5s ease-in;
}

.page.hidden {
    display: none;
}

@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(10px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* ===== NAVBAR ===== */
.navbar {
    background: rgba(0, 0, 0, 0.8);
    backdrop-filter: blur(10px);
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 100;
    border-bottom: 2px solid #e94560;
}

.navbar-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 2rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 1.8rem;
    font-weight: bold;
    color: #e94560;
}

.nav-buttons {
    display: flex;
    gap: 1rem;
}

.btn-nav {
    padding: 0.7rem 1.5rem;
    background: transparent;
    color: #fff;
    border: 1px solid #fff;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    transition: 0.3s;
}

.btn-nav:hover {
    background: #fff;
    color: #1a1a2e;
}

.btn-nav-primary {
    background: #e94560;
    border-color: #e94560;
    color: #fff;
}

.btn-nav-primary:hover {
    background: #ff5a7e;
}

/* ===== HERO SECTION ===== */
.hero {
    max-width: 1200px;
    margin: 0 auto;
    padding: 4rem 2rem;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    align-items: center;
    min-height: 600px;
}

.hero-content h1 {
    font-size: 3.5rem;
    margin-bottom: 1rem;
    background: linear-gradient(135deg, #e94560, #ff5a7e);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.hero-content p {
    font-size: 1.2rem;
    color: #aaa;
    margin-bottom: 2rem;
}

.btn-primary {
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #e94560, #ff5a7e);
    color: #fff;
    border: none;
    border-radius: 5px;
    font-size: 1.1rem;
    cursor: pointer;
    transition: 0.3s;
}

.btn-primary:hover {
    transform: scale(1.05);
    box-shadow: 0 10px 30px rgba(233, 69, 96, 0.5);
}

.btn-full {
    width: 100%;
    margin-top: 1rem;
}

.video-preview {
    width: 100%;
    aspect-ratio: 16/9;
    background: linear-gradient(135deg, rgba(233, 69, 96, 0.2), rgba(255, 90, 126, 0.2));
    border-radius: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 2px solid #e94560;
}

.play-icon {
    font-size: 5rem;
    animation: pulse 1.5s infinite;
}

@keyframes pulse {
    0%, 100% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.1);
    }
}

/* ===== FEATURES ===== */
.features {
    max-width: 1200px;
    margin: 4rem auto;
    padding: 2rem;
}

.features h2 {
    font-size: 2.5rem;
    text-align: center;
    margin-bottom: 3rem;
    color: #e94560;
}

.features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
}

.feature-card {
    background: rgba(255, 255, 255, 0.05);
    padding: 2rem;
    border-radius: 10px;
    text-align: center;
    border: 1px solid rgba(233, 69, 96, 0.3);
    transition: 0.3s;
}

.feature-card:hover {
    background: rgba(233, 69, 96, 0.1);
    border-color: #e94560;
    transform: translateY(-10px);
}

.feature-icon {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.feature-card h3 {
    font-size: 1.3rem;
    margin-bottom: 0.5rem;
}

.feature-card p {
    color: #aaa;
}

/* ===== PLANS ===== */
.plans {
    max-width: 1200px;
    margin: 4rem auto;
    padding: 2rem;
}

.plans h2 {
    font-size: 2.5rem;
    text-align: center;
    margin-bottom: 3rem;
    color: #e94560;
}

.plans-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
}

.plan-card {
    background: rgba(255, 255, 255, 0.05);
    padding: 2rem;
    border-radius: 10px;
    border: 1px solid rgba(233, 69, 96, 0.3);
    text-align: center;
    transition: 0.3s;
    position: relative;
}

.plan-card.featured {
    background: rgba(233, 69, 96, 0.15);
    border-color: #e94560;
    transform: scale(1.05);
}

.badge {
    position: absolute;
    top: -12px;
    left: 50%;
    transform: translateX(-50%);
    background: #e94560;
    color: #fff;
    padding: 0.5rem 1rem;
    border-radius: 5px;
    font-size: 0.9rem;
    font-weight: bold;
}

.plan-card h3 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
}

.price {
    font-size: 2rem;
    color: #e94560;
    margin-bottom: 1.5rem;
    font-weight: bold;
}

.price span {
    font-size: 1rem;
    color: #aaa;
}

.plan-card ul {
    list-style: none;
    margin-bottom: 2rem;
    text-align: left;
}

.plan-card li {
    padding: 0.5rem 0;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.btn-plan {
    width: 100%;
    padding: 0.8rem;
    background: transparent;
    color: #e94560;
    border: 2px solid #e94560;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    transition: 0.3s;
}

.btn-plan:hover {
    background: #e94560;
    color: #fff;
}

.btn-plan-primary {
    background: #e94560;
    color: #fff;
}

.btn-plan-primary:hover {
    background: #ff5a7e;
    border-color: #ff5a7e;
}

/* ===== FOOTER ===== */
.footer {
    max-width: 1200px;
    margin: 4rem auto 0;
    padding: 2rem;
    text-align: center;
    border-top: 1px solid rgba(233, 69, 96, 0.3);
    color: #aaa;
}

.footer-links {
    margin-top: 1rem;
    display: flex;
    justify-content: center;
    gap: 2rem;
}

.footer-links a {
    color: #e94560;
    text-decoration: none;
    transition: 0.3s;
}

.footer-links a:hover {
    text-decoration: underline;
}

/* ===== AUTH PAGES ===== */
.auth-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    padding: 2rem;
}

.btn-back {
    align-self: flex-start;
    padding: 0.7rem 1.5rem;
    background: transparent;
    color: #e94560;
    border: 1px solid #e94560;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    margin-bottom: 2rem;
    transition: 0.3s;
}

.btn-back:hover {
    background: #e94560;
    color: #fff;
}

.auth-box {
    background: rgba(0, 0, 0, 0.6);
    padding: 3rem 2rem;
    border-radius: 10px;
    border: 1px solid rgba(233, 69, 96, 0.5);
    width: 100%;
    max-width: 400px;
}

.auth-box h2 {
    text-align: center;
    margin-bottom: 2rem;
    color: #e94560;
}

.input-field {
    width: 100%;
    padding: 1rem;
    margin-bottom: 1rem;
    background: rgba(255, 255, 255, 0.1);
    border: 1px solid rgba(233, 69, 96, 0.3);
    border-radius: 5px;
    color: #fff;
    font-size: 1rem;
    transition: 0.3s;
}

.input-field:focus {
    outline: none;
    border-color: #e94560;
    background: rgba(233, 69, 96, 0.1);
}

.input-field::placeholder {
    color: #aaa;
}

.strength {
    width: 100%;
    height: 5px;
    background: transparent;
    border-radius: 5px;
    margin-bottom: 0.5rem;
}

.strength.weak {
    background: #ff4444;
}

.strength.medium {
    background: #ffaa00;
}

.strength.strong {
    background: #44ff44;
}

.strength-text {
    font-size: 0.85rem;
    margin-bottom: 1rem;
    font-weight: bold;
}

.error {
    color: #ff4444;
    text-align: center;
    margin-bottom: 1rem;
}

.auth-link {
    text-align: center;
    margin-top: 1.5rem;
    color: #aaa;
}

.auth-link a {
    color: #e94560;
    cursor: pointer;
    text-decoration: underline;
    transition: 0.3s;
}

.auth-link a:hover {
    color: #ff5a7e;
}

/* ===== PLAYER PAGE ===== */
.navbar-player {
    background: rgba(0, 0, 0, 0.9);
    border-bottom: 2px solid #e94560;
    padding: 1rem 0;
}

.user-info {
    display: flex;
    align-items: center;
    gap: 1.5rem;
}

.btn-logout {
    padding: 0.7rem 1.5rem;
    background: #e94560;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: 0.3s;
}

.btn-logout:hover {
    background: #ff5a7e;
}

.player-container {
    max-width: 1200px;
    margin: 2rem auto;
    padding: 2rem;
}

#videoPlayer {
    width: 100%;
    border-radius: 10px;
    background: #000;
}

/* ===== RESPONSIVO ===== */
@media (max-width: 768px) {
    .hero {
        grid-template-columns: 1fr;
        padding: 2rem 1rem;
    }

    .hero-content h1 {
        font-size: 2rem;
    }

    .features-grid, .plans-grid {
        grid-template-columns: 1fr;
    }

    .plan-card.featured {
        transform: scale(1);
    }

    .nav-buttons {
        gap: 0.5rem;
    }

    .btn-nav {
        padding: 0.5rem 1rem;
        font-size: 0.9rem;
    }

    .user-info {
        flex-direction: column;
        gap: 1rem;
    }
}
