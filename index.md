---
layout: default
---

<style>
  :root {
    --accent: #38b000;
    --accent-hover: #6be000;
    --accent-open: #2e8b57;
    --radius: 20px;
    --transition: 0.25s ease;
    --bg: #0f111a;
    --card-bg: #1f2333;
    --text: #f0f4fa;
    --muted: #b0b8d9;
    font-family: system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  }

  body {
    background: var(--bg);
    color: var(--text);
    margin: 0;
    padding: 0;
    line-height: 1.45;
  }

  a {
    color: var(--accent);
    text-decoration: none;
  }
  a:hover {
    text-decoration: underline;
  }

  .container {
    max-width: 1100px;
    margin: auto;
    padding: 1.5rem;
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
  }

  .hero {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    align-items: center;
    justify-content: space-between;
    padding: 1rem 1rem 1.5rem;
    background: rgba(255,255,255,0.03);
    border-radius: var(--radius);
    position: relative;
  }

  .hero-title {
    margin: 0;
    font-size: 1.9rem;
    font-weight: 700;
  }

  .hero-sub {
    margin: 0.25rem 0 1rem;
    color: var(--muted);
  }

  .cta-group {
    display: flex;
    gap: 0.75rem;
    flex-wrap: wrap;
    margin-top: 0.5rem;
  }

  .btn {
    padding: 0.65rem 1.1rem;
    border-radius: 12px;
    font-weight: 600;
    background: var(--accent);
    border: none;
    cursor: pointer;
    color: #fff;
    transition: background var(--transition);
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
    font-size: 0.9rem;
    text-decoration: none;
  }
  .btn:hover {
    background: var(--accent-hover);
  }
  .btn-secondary {
    background: transparent;
    border: 2px solid var(--accent);
    color: var(--accent);
  }
  .btn-secondary:hover {
    background: rgba(56, 176, 0, 0.08);
  }

  .summary-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    margin-bottom: 30px;
  }

  @media (max-width: 1100px) {
    .summary-grid {
      grid-template-columns: repeat(2, 1fr);
    }
  }
  @media (max-width: 800px) {
    .summary-grid {
      grid-template-columns: 1fr;
    }
  }

  .details-wrapper {
    display: flex;
    flex-direction: column;
  }

  details {
    background: var(--card-bg);
    border-radius: var(--radius);
    overflow: hidden;
    position: relative;
    box-shadow: 0 14px 50px -10px rgba(0,0,0,0.35);
  }

  details > summary {
    list-style: none;
    padding: 16px 20px;
    cursor: pointer;
    font-weight: 600;
    font-size: 0.95rem;
    background: var(--accent);
    color: #fff;
    border-radius: var(--radius);
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 6px;
    transition: background var(--transition);
    user-select: none;
  }

  details > summary::-webkit-details-marker {
    display: none;
  }

  details:hover > summary {
    background: var(--accent-hover);
  }
  details[open] > summary {
    background: var(--accent-open);
  }

  .details-inner {
    padding: 18px 20px;
    font-size: 0.95rem;
    line-height: 1.4;
    color: var(--text);
  }

  .details-inner ul {
    padding-left: 1.1em;
    margin: 0;
  }

  .badge {
    display: inline-block;
    background: rgba(255,255,255,0.08);
    padding: 4px 10px;
    border-radius: 999px;
    font-size: 0.65rem;
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-right: 6px;
  }

  .project-title {
    margin: 0 0 6px;
    font-weight: 700;
    font-size: 1rem;
  }

  .footer {
    margin-top: 2rem;
    padding: 1rem 0;
    text-align: center;
    font-size: 0.9rem;
    color: var(--muted);
  }

  .link-row a {
    margin-right: 1rem;
  }

  .small {
    font-size: 0.8rem;
    color: var(--muted);
  }
</style>

<div class="container">
  <!-- Hero / Intro -->
  <section class="hero" aria-label="Introduction">
    <div style="flex:1; min-width:250px;">
      <h1 class="hero-title">Blanca Calderón</h1>
      <p class="hero-sub">Cybersecurity Analyst | Penetration Testing · Digital Forensics · Vulnerability Assessment</p>
      <div class="cta-group">
        <a class="btn" href="#projects">View Projects</a>
        <a class="btn btn-secondary" href="/resume.pdf" target="_blank" rel="noopener">Download Résumé</a>
        <a class="btn" href="https://blancacal.github.io/portfolio/" target="_blank" rel="noopener">Portfolio</a>
      </div>
    </div>
    <div style="min-width:120px; display:flex; align-items:center; justify-content:center;">
      <!-- Placeholder for avatar or icon -->
      <div style="width:100px; height:100px; border-radius:50%; background:rgba(255,255,255,0.08); display:flex; align-items:center; justify-content:center; font-size:0.6rem; text-align:center;">
        Avatar
      </div>
    </div>
  </section>

  <!-- Summary Grid -->
  <div class="summary-grid" aria-label="Profile sections">
    <div class="details-wrapper">
      <details id="about-me">
        <summary>🔐 About Me</summary>
        <div class="details-inner">
          <p>I’m a Cybersecurity Analyst and Master’s candidate in Cybersecurity with a background in Computer Engineering. I focus on penetration testing, vulnerability assessment, digital forensics, and threat detection. I continually grow my expertise through hands-on research, industry engagement, and building tools to improve security postures.</p>
          <p><strong>Areas of interest:</strong> Penetration Testing, Incident Response, Digital Forensics, Malware Analysis, Secure Code Development, Vulnerability Assessment.</p>
        </div>
      </details>
    </div>
    <div class="details-wrapper">
      <details id="education">
        <summary>🎓 Education</summary>
        <div class="details-inner">
          <ul>
            <li>Bachelor’s Degree in Computer Engineering – University of Alcalá de Henares</li>
            <li>Master’s Degree in Cybersecurity (in progress)</li>
            <li>English: C1 – Advanced Professional Proficiency</li>
          </ul>
        </div>
      </details>
    </div>
    <div class="details-wrapper">
      <details id="technical-skills">
        <summary>🛠️ Technical Skills</summary>
        <div class="details-inner">
          <ul>
            <li><strong>Security & Testing:</strong> Metasploit, Burp Suite, OWASP ZAP, Nessus, Fortify, CNAPP tools</li>
            <li><strong>Forensics & Monitoring:</strong> Autopsy, FTK Imager, Wireshark</li>
            <li><strong>OSINT:</strong> Maltego, Google Dorks, FOCA, Shodan, TheHarvester</li>
            <li><strong>Languages & Scripting:</strong> Python, Bash, PowerShell, Java</li>
            <li><strong>Platforms & Practices:</strong> Kali Linux, Threat Hunting, Secure Code Review, Ethical Hacking, Attack Surface Management, Security Hardening, Endpoint Protection</li>
          </ul>
        </div>
      </details>
    </div>
    <div class="details-wrapper">
      <details id="certifications">
        <summary>📜 Certifications</summary>
        <div class="details-inner">
          <ul>
            <li>
              <span class="badge">Badge</span>
              <a href="https://www.credly.com/badges/f271ee76-5012-409a-804e-84ee6423206a" target="_blank" rel="noopener">
                Ethical Hacker – Cisco Networking Academy
              </a>
            </li>
            <li>
              <span class="badge">Certificate</span>
              Cyber Intelligence & Open Source Intelligence (OSINT) – CCN-CERT, Centro Criptológico Nacional
            </li>
            <li>
              <span class="badge">Certificate</span>
              <a href="https://cyberlandsec.com/certificate/22d40978/" target="_blank" rel="noopener">
                Certified Ethical Hacking and Penetration Tester (CEHPT) – CyberLand Sec
              </a>
            </li>
            <li>
              <span class="badge">Badge</span>
              <a href="https://www.credly.com/badges/863e20e5-b2ba-4729-b816-abb2eca382b2/public_url" target="_blank" rel="noopener">
                Azure Fundamentals – Microsoft
              </a>
            </li>
          </ul>
        </div>
      </details>
    </div>
    <div class="details-wrapper">
      <details id="projects">
        <summary>📂 Projects</summary>
        <div class="details-inner">
          <div class="project">
            <h3 class="project-title">Vulnerability Detection Tool</h3>
            <p>Developed an automated system to detect, classify, and report web application vulnerabilities using custom heuristics and open-source scanners.</p>
            <p class="small"><strong>Tech stack:</strong> Python, Nmap, API integration, custom reporting.</p>
            <p class="small"><strong>Role:</strong> Full-stack security developer and analyst.</p>
            <p class="small"><strong>Outcome:</strong> Reduced manual triage time and produced actionable reports for remediation.</p>
            <p><a href="https://github.com/BlancaCal/vulnerability-detection-tool" target="_blank" rel="noopener">View on GitHub</a></p>
          </div>
          <!-- Additional projects can follow the same structure -->
        </div>
      </details>
    </div>
    <div class="details-wrapper">
      <details id="contact">
        <summary>📫 Contact</summary>
        <div class="details-inner">
          <ul>
            <li>📧 Email: <a href="mailto:blancacaldgonz@gmail.com">blancacaldgonz@gmail.com</a></li>
            <li>💼 <a href="https://www.linkedin.com/in/blanca-calder%C3%B3n-gonz%C3%A1lez-a28313252/" target="_blank" rel="noopener">LinkedIn</a></li>
            <li>🔒 <a href="https://github.com/BlancaCal" target="_blank" rel="noopener">GitHub</a></li>
          </ul>
        </div>
      </details>
    </div>
  </div>

  <div class="footer">
    <p>Thanks for visiting — committed to securing systems and empowering users through informed defense. 🛡️</p>
  </div>
</div>
