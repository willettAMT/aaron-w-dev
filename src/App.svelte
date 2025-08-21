<div class="container">
    <header class="hero">
        <div class="hero-content">
            <h1 class="hero-title">aaron willett</h1>
            <div class="hero-subtitle">software engineer</div>
            <div class="hero-tagline">building efficient systems • tackling complexity • securing the future</div>
        </div>
    </header>

    <section class="about">
        <div class="about-card">
            <h2 class="section-title">about</h2>
            <p>
                Passionate about building efficient, developer-friendly systems with a focus on <strong>IoT, embedded systems, scalable backend systems, and low-level programming</strong>. 
                Currently exploring ways to make software more maintainable, performant, and secure—especially in resource-constrained environments.
            </p>
            <p>
                <strong>Current coursework:</strong> System design, performance optimization, cloud security, and systems programming. 
                Contributing to firmware development with Portland State Aerospace Society, with interests spanning secure data aggregation at the hardware level, 
                securing wireless protocols, and optimizing system efficiency from the ground up.
            </p>
            <p>
                If you'd like to chat about anything tech-related, feel free to reach out!
            </p>
        </div>
    </section>

    <section class="projects">
        <h2 class="section-title">featured projects</h2>
        
        <div class="project-grid">
            <div class="project-card featured">
                <div class="project-header">
                    <div class="project-icon">JT</div>
                    <div class="project-meta">
                        <h3 class="project-title">Job Tracker</h3>
                        <div class="project-type">Chrome Extension</div>
                    </div>
                    <div class="project-status">Live</div>
                </div>
                
                <p class="project-description">
                    Automates job application tracking by extracting data from LinkedIn, Indeed, and other job sites, 
                    saving directly to Google Sheets with one click. Eliminates tedious manual spreadsheet entry.
                </p>
                
                <div class="tech-stack">
                    <span class="tech-tag">Chrome APIs</span>
                    <span class="tech-tag">OAuth 2.0</span>
                    <span class="tech-tag">Google Sheets API</span>
                    <span class="tech-tag">Manifest V3</span>
                </div>
                
                <div class="project-highlight">
                    <strong>Key Challenge:</strong> Extension ID consistency across development machines — solved with 
                    dual-ID OAuth configuration and persistent private key packaging.
                </div>
                
                <div class="project-links">
                    <a href="https://chrome.google.com/webstore/detail/job-tracker" class="btn btn-primary" target="_blank" rel="noreferrer">
                        Chrome Store
                    </a>
                    <a href="https://github.com/willettAMT/job-tracker" class="btn btn-secondary" target="_blank" rel="noreferrer">
                        Source Code
                    </a>
                </div>
            </div>

            <div class="project-card">
                <div class="project-header">
                    <div class="project-icon">SV</div>
                    <div class="project-meta">
                        <h3 class="project-title">Svelvet</h3>
                        <div class="project-type">Open Source Library</div>
                    </div>
                    <div class="project-status">Active</div>
                </div>
                
                <p class="project-description">
                    Component library for building interactive flowcharts and node-based editors in Svelte. 
                    Contributed core architecture and component development.
                </p>
                
                <div class="tech-stack">
                    <span class="tech-tag">Svelte</span>
                    <span class="tech-tag">TypeScript</span>
                    <span class="tech-tag">Component Library</span>
                </div>
                
                <div class="project-links">
                    <a href="https://svelvet.io" class="btn btn-primary" target="_blank" rel="noreferrer">
                        Playground
                    </a>
                </div>
            </div>
        </div>
    </section>

    <section class="connect">
        <h2 class="section-title">connect</h2>
        <div class="connect-grid">
            <a href="https://github.com/willettAMT" class="connect-card" target="_blank" rel="noreferrer">
                <div class="connect-icon">GH</div>
                <div class="connect-text">GitHub</div>
            </a>
            <a href="https://linkedin.com/in/willettAMT" class="connect-card" target="_blank" rel="noreferrer">
                <div class="connect-icon">LI</div>
                <div class="connect-text">LinkedIn</div>
            </a>
        </div>
    </section>

    <footer class="footer">
        <i>portfolio v0.1.0 • built with svelte</i>
    </footer>
</div>

<style>
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 2rem;
    }

    /* Hero Section */
    .hero {
        text-align: center;
        padding: 4rem 0 6rem 0;
        background: linear-gradient(135deg, rgba(100, 108, 255, 0.1) 0%, rgba(83, 91, 242, 0.1) 100%);
        border-radius: 20px;
        margin-bottom: 4rem;
        position: relative;
        overflow: hidden;
    }

    .hero::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: radial-gradient(circle at 30% 20%, rgba(100, 108, 255, 0.15) 0%, transparent 50%);
        pointer-events: none;
    }

    .hero-content {
        position: relative;
        z-index: 1;
    }

    .hero-title {
        font-size: clamp(3rem, 8vw, 5.2rem);
        margin: 0 0 1rem 0;
        color: rgba(255, 255, 255, 0.95);
        text-shadow: 0 0 30px rgba(100, 108, 255, 0.5);
    }

    .hero-subtitle {
        font-size: 1.5rem;
        color: #646cff;
        margin-bottom: 0.5rem;
        font-weight: 500;
    }

    .hero-tagline {
        font-size: 1.1rem;
        color: rgba(255, 255, 255, 0.7);
        font-style: italic;
    }

    /* Sections */
    .section-title {
        font-size: 2.5rem;
        margin-bottom: 2rem;
        color: rgba(255, 255, 255, 0.95);
        position: relative;
        display: inline-block;
    }

    .section-title::after {
        content: '';
        position: absolute;
        bottom: -8px;
        left: 0;
        width: 60px;
        height: 3px;
        background: linear-gradient(90deg, #646cff, #535bf2);
        border-radius: 2px;
    }

    /* About Section */
    .about {
        margin-bottom: 4rem;
    }

    .about-card {
        background: rgba(255, 255, 255, 0.05);
        backdrop-filter: blur(10px);
        border: 1px solid rgba(255, 255, 255, 0.1);
        border-radius: 16px;
        padding: 2.5rem;
        transition: all 0.3s ease;
    }

    .about-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    }

    .about-card p {
        line-height: 1.7;
        margin-bottom: 1.5rem;
        color: rgba(255, 255, 255, 0.9);
    }

    .about-card strong {
        color: #646cff;
    }

    /* Projects Section */
    .projects {
        margin-bottom: 4rem;
    }

    .project-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
        gap: 2rem;
    }

    .project-card {
        background: rgba(255, 255, 255, 0.05);
        backdrop-filter: blur(10px);
        border: 1px solid rgba(255, 255, 255, 0.1);
        border-radius: 20px;
        padding: 2rem;
        transition: all 0.3s ease;
        position: relative;
        overflow: hidden;
    }

    .project-card.featured {
        border: 1px solid rgba(100, 108, 255, 0.3);
        background: rgba(100, 108, 255, 0.08);
    }

    .project-card:hover {
        transform: translateY(-8px);
        box-shadow: 0 25px 50px rgba(0, 0, 0, 0.4);
        border-color: rgba(100, 108, 255, 0.5);
    }

    .project-header {
        display: flex;
        align-items: flex-start;
        gap: 1rem;
        margin-bottom: 1.5rem;
    }

    .project-icon {
        font-size: 1.2rem;
        font-weight: 700;
        background: rgba(100, 108, 255, 0.2);
        border-radius: 12px;
        padding: 0.5rem;
        display: flex;
        align-items: center;
        justify-content: center;
        min-width: 60px;
        height: 60px;
        color: #646cff;
        border: 2px solid rgba(100, 108, 255, 0.3);
    }

    .project-meta {
        flex: 1;
    }

    .project-title {
        font-size: 1.4rem;
        margin: 0 0 0.3rem 0;
        color: rgba(255, 255, 255, 0.95);
    }

    .project-type {
        color: #646cff;
        font-size: 0.9rem;
        font-weight: 500;
    }

    .project-status {
        background: linear-gradient(135deg, #27ae60, #2ecc71);
        color: white;
        padding: 0.3rem 0.8rem;
        border-radius: 20px;
        font-size: 0.8rem;
        font-weight: 600;
        text-transform: uppercase;
        letter-spacing: 0.5px;
    }

    .project-description {
        color: rgba(255, 255, 255, 0.8);
        line-height: 1.6;
        margin-bottom: 1.5rem;
    }

    .tech-stack {
        display: flex;
        flex-wrap: wrap;
        gap: 0.5rem;
        margin-bottom: 1.5rem;
    }

    .tech-tag {
        background: rgba(100, 108, 255, 0.2);
        color: #646cff;
        padding: 0.4rem 0.8rem;
        border-radius: 20px;
        font-size: 0.8rem;
        font-weight: 500;
        border: 1px solid rgba(100, 108, 255, 0.3);
    }

    .project-highlight {
        background: rgba(255, 193, 7, 0.1);
        border: 1px solid rgba(255, 193, 7, 0.3);
        border-radius: 10px;
        padding: 1rem;
        margin-bottom: 1.5rem;
        font-size: 0.9rem;
        color: rgba(255, 255, 255, 0.9);
    }

    .project-highlight strong {
        color: #ffc107;
    }

    .project-links {
        display: flex;
        gap: 1rem;
        flex-wrap: wrap;
    }

    .btn {
        text-decoration: none;
        padding: 0.8rem 1.5rem;
        border-radius: 10px;
        font-weight: 600;
        font-size: 0.9rem;
        transition: all 0.3s ease;
        display: inline-flex;
        align-items: center;
        gap: 0.5rem;
    }

    .btn-primary {
        background: linear-gradient(135deg, #646cff, #535bf2);
        color: white;
    }

    .btn-primary:hover {
        background: linear-gradient(135deg, #535bf2, #4c46d6);
        transform: translateY(-2px);
        box-shadow: 0 10px 20px rgba(100, 108, 255, 0.3);
    }

    .btn-secondary {
        background: rgba(255, 255, 255, 0.1);
        color: rgba(255, 255, 255, 0.9);
        border: 1px solid rgba(255, 255, 255, 0.2);
    }

    .btn-secondary:hover {
        background: rgba(255, 255, 255, 0.2);
        transform: translateY(-2px);
    }

    /* Connect Section */
    .connect {
        margin-bottom: 4rem;
    }

    .connect-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 1.5rem;
    }

    .connect-card {
        background: rgba(255, 255, 255, 0.05);
        backdrop-filter: blur(10px);
        border: 1px solid rgba(255, 255, 255, 0.1);
        border-radius: 16px;
        padding: 2rem;
        text-decoration: none;
        color: rgba(255, 255, 255, 0.9);
        transition: all 0.3s ease;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1rem;
    }

    .connect-card:hover {
        transform: translateY(-5px);
        background: rgba(100, 108, 255, 0.1);
        border-color: rgba(100, 108, 255, 0.3);
        color: white;
    }

    .connect-icon {
        font-size: 1.5rem;
        font-weight: 700;
        color: #646cff;
    }

    .connect-text {
        font-weight: 600;
        font-size: 1.1rem;
    }

    /* Footer */
    .footer {
        text-align: center;
        padding: 2rem 0;
        color: rgba(255, 255, 255, 0.5);
        border-top: 1px solid rgba(255, 255, 255, 0.1);
    }

    /* Responsive */
    @media (max-width: 768px) {
        .container {
            padding: 1rem;
        }
        
        .hero {
            padding: 3rem 1rem 4rem 1rem;
            margin-bottom: 3rem;
        }

        .about-card {
            padding: 2rem;
        }

        .project-grid {
            grid-template-columns: 1fr;
        }

        .project-card {
            padding: 1.5rem;
        }

        .project-links {
            flex-direction: column;
        }

        .btn {
            justify-content: center;
        }
    }
</style>
