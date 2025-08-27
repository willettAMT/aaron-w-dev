<script>
    let showModal = false;

    function openModal() {
        showModal = true;
        document.body.style.overflow = 'hidden'; // Prevent background scrolling
    }

    function closeModal() {
        showModal = false;
        document.body.style.overflow = 'auto'; // Restore scrolling
    }

    // Close modal on Escape key
    function handleKeydown(event) {
        if (event.key === 'Escape' && showModal) {
            closeModal();
        }
    }
</script>

<svelte:window on:keydown={handleKeydown} />

<div class="container">
    <header class="hero">
        <div class="hero-content">
            <h1 class="hero-title">aaron willett</h1>
            <div class="hero-subtitle">software engineer</div>
            <div class="hero-tagline">building efficient systems • tackling complexity • securing the future</div>
            <button class="resume-btn" on:click={openModal}>View Resume</button>
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
                    <div class="project-status">Under Review</div>
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
                        Chrome Store - Pending Approval
                    </a>
                    <a href="https://github.com/willettAMT/job-tracker-extension" class="btn btn-secondary" target="_blank" rel="noreferrer">
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

            <div class="project-card">
                <div class="project-header">
                    <div class="project-icon">NV</div>
                    <div class="project-meta">
                        <h3 class="project-title">Neovim Config</h3>
                        <div class="project-type">Development Environment</div>
                    </div>
                    <div class="project-status daily-use">Daily Use</div>
                </div>
                
                <p class="project-description">
                    Custom Neovim configuration optimized for systems programming and embedded development. 
                    Cross-platform setup supporting ArchOS and MacOS with nvim >=0.11.0.
                </p>
                
                <div class="tech-stack">
                    <span class="tech-tag">Lua</span>
                    <span class="tech-tag">Neovim</span>
                    <span class="tech-tag">LSP</span>
                </div>
                
                <div class="project-links">
                    <a href="https://github.com/willettAMT/nvim" class="btn btn-secondary" target="_blank" rel="noreferrer">
                        View Config
                    </a>
                </div>
            </div>

            <div class="project-card">
                <div class="project-header">
                    <div class="project-icon">CA</div>
                    <div class="project-meta">
                        <h3 class="project-title">ChocAn System</h3>
                        <div class="project-type">Healthcare Platform</div>
                    </div>
                    <div class="project-status academic">Academic</div>
                </div>
                
                <p class="project-description">
                    Production-grade healthcare provider platform built in C++ with PostgreSQL. 
                    Multi-tier architecture with secure data access layer, advanced reporting, and compliance features.
                </p>
                
                <div class="tech-stack">
                    <span class="tech-tag">C++</span>
                    <span class="tech-tag">PostgreSQL</span>
                    <span class="tech-tag">Multi-tier Architecture</span>
                    <span class="tech-tag">Security</span>
                </div>
                
                <div class="project-highlight">
                    <strong>Key Features/Contributions:</strong>I personally designed and implemented Secure DAL with 
                    parameterized queries, DTOs and base DAOs for standardized database operations, prepared
                    statements for large datasets, advanced analytics reporting.
                </div>
                
                <div class="project-links">
                    <a href="https://github.com/willettAMT/chocAn" class="btn btn-secondary" target="_blank" rel="noreferrer">
                        View Code
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

    <!-- Resume Modal -->
    {#if showModal}
        <div class="modal-backdrop" on:click={closeModal}>
            <div class="modal-content" on:click|stopPropagation>
                <div class="modal-header">
                    <h3>Resume - Aaron Willett</h3>
                    <button class="modal-close" on:click={closeModal}>&times;</button>
                </div>
                <div class="modal-body">
                    <iframe 
                        src="/summer24_res.pdf" 
                        title="Aaron Willett Resume"
                        class="pdf-viewer">
                    </iframe>
                </div>
                <div class="modal-footer">
                    <a href="/summer24_res.pdf" download="aaron-willett-resume.pdf" class="btn btn-primary">
                        Download PDF
                    </a>
                    <button class="btn btn-secondary" on:click={closeModal}>Close</button>
                </div>
            </div>
        </div>
    {/if}
</div>

<style>
    /* Custom Color Scheme */
    :root {
        --black: #0a0a0a;
        --dark-green: #1a3b36;
        --forest-green: #2d5a27;
        --purple: #7c3aed;
        --purple-light: #8b5cf6;
        --purple-dark: #6d28d9;
        --orange: #f97316;
        --orange-light: #fb923c;
        --dark-blue: #1e3a8a;
        --dark-blue-light: #3b82f6;
        
        /* Text colors */
        --text-primary: #f8fafc;
        --text-secondary: #cbd5e1;
        --text-muted: #94a3b8;
    }

    body {
        margin: 0;
        background: linear-gradient(135deg, var(--black) 0%, var(--dark-green) 100%);
        color: var(--text-primary);
        min-height: 100vh;
        font-family: Inter, system-ui, Avenir, Helvetica, Arial, sans-serif;
        line-height: 1.5;
    }

    a {
        color: var(--purple-light);
        text-decoration: none;
        transition: color 0.3s ease;
    }

    a:hover {
        color: var(--purple);
    }

    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 2rem;
    }

    /* Hero Section */
    .hero {
        text-align: center;
        padding: 4rem 0 6rem 0;
        background: linear-gradient(135deg, var(--dark-green) 0%, var(--forest-green) 50%, var(--dark-blue) 100%);
        border-radius: 20px;
        margin-bottom: 4rem;
        position: relative;
        overflow: hidden;
        border: 1px solid rgba(124, 58, 237, 0.2);
    }

    .hero::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: radial-gradient(circle at 30% 20%, rgba(124, 58, 237, 0.15) 0%, transparent 50%);
        pointer-events: none;
    }

    .hero-content {
        position: relative;
        z-index: 1;
    }

    .hero-title {
        font-size: clamp(3rem, 8vw, 5.2rem);
        margin: 0 0 1rem 0;
        color: var(--text-primary);
        text-shadow: 0 0 30px rgba(124, 58, 237, 0.5);
    }

    .hero-subtitle {
        font-size: 1.5rem;
        color: var(--purple-light);
        margin-bottom: 0.5rem;
        font-weight: 500;
    }

    .hero-tagline {
        font-size: 1.1rem;
        color: var(--text-secondary);
        font-style: italic;
        margin-bottom: 2rem;
    }

    .resume-btn {
        background: linear-gradient(135deg, var(--purple) 0%, var(--purple-dark) 100%);
        color: white;
        border: none;
        padding: 1rem 2rem;
        border-radius: 12px;
        font-size: 1.1rem;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s ease;
        margin-top: 1rem;
        border: 1px solid var(--purple-light);
    }

    .resume-btn:hover {
        background: linear-gradient(135deg, var(--purple-light) 0%, var(--purple) 100%);
        transform: translateY(-2px);
        box-shadow: 0 10px 25px rgba(124, 58, 237, 0.4);
    }

    /* Sections */
    .section-title {
        font-size: 2.5rem;
        margin-bottom: 2rem;
        color: var(--text-primary);
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
        background: linear-gradient(90deg, var(--purple), var(--orange));
        border-radius: 2px;
    }

    /* About Section */
    .about {
        margin-bottom: 4rem;
    }

    .about-card {
        background: linear-gradient(135deg, var(--dark-green) 0%, var(--forest-green) 100%);
        backdrop-filter: blur(10px);
        border: 1px solid rgba(124, 58, 237, 0.2);
        border-radius: 16px;
        padding: 2.5rem;
        transition: all 0.3s ease;
    }

    .about-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
        border-color: var(--purple-light);
    }

    .about-card p {
        line-height: 1.7;
        margin-bottom: 1.5rem;
        color: var(--text-secondary);
    }

    .about-card strong {
        color: var(--purple-light);
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
        background: linear-gradient(135deg, var(--dark-green) 0%, var(--forest-green) 100%);
        backdrop-filter: blur(10px);
        border: 1px solid rgba(124, 58, 237, 0.2);
        border-radius: 20px;
        padding: 2rem;
        transition: all 0.3s ease;
        position: relative;
        overflow: hidden;
    }

    .project-card.featured {
        border: 1px solid var(--purple);
        background: linear-gradient(135deg, var(--dark-green) 0%, var(--dark-blue) 100%);
        box-shadow: 0 0 20px rgba(124, 58, 237, 0.2);
    }

    .project-card:hover {
        transform: translateY(-8px);
        box-shadow: 0 25px 50px rgba(0, 0, 0, 0.4);
        border-color: var(--purple-light);
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
        background: linear-gradient(135deg, var(--purple) 0%, var(--purple-dark) 100%);
        border-radius: 12px;
        padding: 0.5rem;
        display: flex;
        align-items: center;
        justify-content: center;
        min-width: 60px;
        height: 60px;
        color: white;
        border: 2px solid var(--purple-light);
    }

    .project-meta {
        flex: 1;
    }

    .project-title {
        font-size: 1.4rem;
        margin: 0 0 0.3rem 0;
        color: var(--text-primary);
    }

    .project-type {
        color: var(--purple-light);
        font-size: 0.9rem;
        font-weight: 500;
    }

    .project-status {
        background: linear-gradient(135deg, var(--forest-green), var(--dark-green));
        color: white;
        padding: 0.3rem 0.8rem;
        border-radius: 20px;
        font-size: 0.8rem;
        font-weight: 600;
        text-transform: uppercase;
        letter-spacing: 0.5px;
        border: 1px solid var(--purple);
    }

    .project-status.daily-use {
        background: linear-gradient(135deg, var(--orange), var(--orange-light));
        border-color: var(--orange);
    }

    .project-status.academic {
        background: linear-gradient(135deg, var(--dark-blue), var(--dark-blue-light));
        border-color: var(--dark-blue-light);
    }

    .project-description {
        color: var(--text-secondary);
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
        background: linear-gradient(135deg, var(--dark-blue) 0%, var(--purple-dark) 100%);
        color: var(--text-primary);
        padding: 0.4rem 0.8rem;
        border-radius: 20px;
        font-size: 0.8rem;
        font-weight: 500;
        border: 1px solid var(--purple);
    }

    .project-highlight {
        background: linear-gradient(135deg, var(--orange) 10%, var(--forest-green) 100%);
        border: 1px solid var(--orange);
        border-radius: 10px;
        padding: 1rem;
        margin-bottom: 1.5rem;
        font-size: 0.9rem;
        color: var(--text-primary);
    }

    .project-highlight strong {
        color: var(--orange-light);
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
        border: none;
        cursor: pointer;
    }

    .btn-primary {
        background: linear-gradient(135deg, var(--purple), var(--purple-dark));
        color: white;
    }

    .btn-primary:hover {
        background: linear-gradient(135deg, var(--purple-light), var(--purple));
        transform: translateY(-2px);
        box-shadow: 0 10px 20px rgba(124, 58, 237, 0.3);
    }

    .btn-secondary {
        background: linear-gradient(135deg, var(--dark-blue), var(--forest-green));
        color: var(--text-primary);
        border: 1px solid var(--purple);
    }

    .btn-secondary:hover {
        background: linear-gradient(135deg, var(--forest-green), var(--dark-blue));
        transform: translateY(-2px);
        border-color: var(--purple-light);
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
        background: linear-gradient(135deg, var(--dark-green) 0%, var(--forest-green) 100%);
        backdrop-filter: blur(10px);
        border: 1px solid rgba(124, 58, 237, 0.2);
        border-radius: 16px;
        padding: 2rem;
        text-decoration: none;
        color: var(--text-secondary);
        transition: all 0.3s ease;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1rem;
    }

    .connect-card:hover {
        transform: translateY(-5px);
        background: linear-gradient(135deg, var(--purple) 10%, var(--dark-green) 100%);
        border-color: var(--purple-light);
        color: var(--text-primary);
    }

    .connect-icon {
        font-size: 1.5rem;
        font-weight: 700;
        color: var(--purple-light);
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

    /* Modal Styles */
    .modal-backdrop {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.8);
        backdrop-filter: blur(5px);
        display: flex;
        align-items: center;
        justify-content: center;
        z-index: 1000;
        padding: 1rem;
    }

    .modal-content {
        background: rgba(36, 36, 36, 0.95);
        backdrop-filter: blur(20px);
        border: 1px solid rgba(255, 255, 255, 0.1);
        border-radius: 20px;
        width: 90%;
        max-width: 900px;
        height: 90%;
        max-height: 800px;
        display: flex;
        flex-direction: column;
        overflow: hidden;
        box-shadow: 0 25px 50px rgba(0, 0, 0, 0.5);
    }

    .modal-header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1.5rem 2rem;
        border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    }

    .modal-header h3 {
        margin: 0;
        color: rgba(255, 255, 255, 0.95);
        font-size: 1.3rem;
    }

    .modal-close {
        background: none;
        border: none;
        color: rgba(255, 255, 255, 0.7);
        font-size: 2rem;
        cursor: pointer;
        padding: 0;
        width: 40px;
        height: 40px;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 50%;
        transition: all 0.3s ease;
    }

    .modal-close:hover {
        background: rgba(255, 255, 255, 0.1);
        color: white;
    }

    .modal-body {
        flex: 1;
        padding: 0;
        overflow: hidden;
    }

    .pdf-viewer {
        width: 100%;
        height: 100%;
        border: none;
        background: white;
    }

    .modal-footer {
        display: flex;
        gap: 1rem;
        padding: 1.5rem 2rem;
        border-top: 1px solid rgba(255, 255, 255, 0.1);
        justify-content: flex-end;
    }

    @media (max-width: 768px) {
        .modal-content {
            width: 95%;
            height: 95%;
        }

        .modal-header {
            padding: 1rem;
        }

        .modal-footer {
            padding: 1rem;
            flex-direction: column;
        }

        .resume-btn {
            padding: 0.8rem 1.5rem;
            font-size: 1rem;
        }
    }

    /* Force dark mode - override system preferences */
    @media (prefers-color-scheme: light) {
        :root {
            color: rgba(255, 255, 255, 0.87) !important;
            background-color: #242424 !important;
        }
        
        body {
            background-color: #242424 !important;
            color: rgba(255, 255, 255, 0.87) !important;
        }
        
        a:hover {
            color: #535bf2 !important;
        }
        
        button {
            background-color: #1a1a1a !important;
        }
    }
</style>
