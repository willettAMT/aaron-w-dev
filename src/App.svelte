<div>

    <h1>aaron willett</h1>

    <p>I am a software engineer passionate about building efficient, developer-friendly systems. My current focus is on IoT,<br>
        embedded systems, and low-level programming, with a keen interest in tackling the "30 million line problem" as <br>
        described by Casey Muratori. I explore ways to make software more maintainable, performant, and secure<br>
        — especially in resource-constrained environments.<br><br>
        My current coursework includes embedded C, NASM, embedded rust, malware reverse engineering, and web and cloud security.<br>
        I also contribute to firmware development with the Portland State Aerospace Society. My interests span secure data<br>
        aggregation at the hardware level, securing wireless protocols, and optimizing system efficiency from the ground up.<br>
        If you'd like to chat about systems programming, embedded security, or anything tech-related, feel free to reach out!<br><br>

        Previously, I worked on an open source product, Svelvet, as a software engineer, where I conceptualized and developed a <br>
        component library for building flow-charts on the Svelte compiler. Check out our documentation page <a href="https://svelvet.io" target="_blank" rel="noreferrer"><i>Svelvet</i></a> for the playground!<br>
    </p>

    <h2 style="margin-top: 3rem; margin-bottom: 1rem; font-size: 2.5em;">projects</h2>
    
    <div class="project">
        <h3><a href="https://chrome.google.com/webstore/detail/job-tracker" target="_blank" rel="noreferrer"><i>Job Tracker Chrome Extension</i></a></h3>
        <p>
            Built a Chrome extension that automates job application tracking by extracting data from LinkedIn, Indeed, and other job sites, 
            then saving directly to Google Sheets with one click. Solves the tedious manual process of copy-pasting job details into spreadsheets.<br><br>
            
            <strong>Technical highlights:</strong> Chrome Extension API (Manifest V3), Google Sheets API integration, OAuth 2.0 authentication, 
            cross-device Chrome storage sync, dynamic DOM parsing with fallback selectors, privacy-first architecture with zero external servers.<br><br>
            
            <strong>Key challenge solved:</strong> Extension ID consistency across development machines — each unpacked extension gets a random ID, 
            breaking OAuth configuration when switching between devices. Implemented dual-ID OAuth client registration and extension packaging 
            with persistent private keys.<br><br>
            
            Live on Chrome Web Store • <a href="https://github.com/willettAMT/job-tracker" target="_blank" rel="noreferrer"><i>View source</i></a>
        </p>
    </div>

    <div class="project">
        <h3><a href="https://svelvet.io" target="_blank" rel="noreferrer"><i>Svelvet</i></a></h3>
        <p>
            Open source component library for building interactive flowcharts and node-based editors in Svelte. Contributed core architecture 
            and component development as part of the engineering team.<br><br>
            
            Check out the <a href="https://svelvet.io" target="_blank" rel="noreferrer"><i>documentation and playground</i></a>!
        </p>
    </div>

    <p style="margin-top: 3rem;">
        Check out my <a href="https://github.com/willettAMT" target="_blank" rel="noreferrer"><i>Github</i></a>, friends!<br>
        Find me on <a href="https://linkedin.com/in/willettAMT" target="_blank" rel="noreferrer"><i>LinkedIn</i></a>!
    </p>
</div>
<footer>
    <i>portfolio 0.0.4</i>
</footer>

<style>
    .project {
        margin-bottom: 2rem;
        padding-bottom: 1.5rem;
        border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    }
    
    .project:last-child {
        border-bottom: none;
    }
    
    .project h3 {
        margin-bottom: 0.5rem;
        font-size: 1.4em;
    }
    
    .project p {
        margin-bottom: 0;
        line-height: 1.6;
    }
    
    h2 {
        color: rgba(255, 255, 255, 0.87);
    }
</style>
