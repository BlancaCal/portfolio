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
  
  .badge-card {
    display: inline-block;
    margin: 8px;
    border-radius: 12px;
    overflow: hidden;
    transition: transform .25s ease, box-shadow .25s ease;
  }
  
  .badge-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 20px 60px -10px rgba(56,176,0,0.6);
  }
  
</style>

<div class="container">
  <!-- Hero / Intro -->
  <section class="hero" aria-label="Introduction">
    <div style="flex:1; min-width:250px;">
      <h1 class="hero-title">Blanca Calderón</h1>
      <p class="hero-sub">Cybersecurity Analyst | Penetration Testing · Digital Forensics · Vulnerability Assessment · Attack Surface Management</p>
      <div class="cta-group">
        <a class="btn" href="https://github.com/BlancaCal?tab=repositories" target="_blank" rel="noopener">View Projects</a>
         <a class="btn" href="https://www.linkedin.com/in/blanca-calder%C3%B3n-gonz%C3%A1lez-a28313252?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3Bh6%2BYRnehQsquyU%2BbhmLa1Q%3D%3D" target="_blank" rel="noopener">Linkedin profile</a>
      </div>
    </div>
    <div style="min-width:120px; display:flex; align-items:center; justify-content:center;">
    </div>
  </section>

  <!-- Summary Grid -->
  <div class="summary-grid" aria-label="Profile sections">
    <div class="details-wrapper">
      <details id="about-me">
        <summary>🔐 About Me</summary>
        <div class="details-inner">
          <p>I’m a Cybersecurity Analyst and Master’s graduate in Cybersecurity with a Computer Engineering Degree.<br><br>
            I focus on penetration testing, vulnerability assessment, digital forensics, threat detection and attack surface management.<br><br>
            I continually grow my expertise through hands-on research, industry engagement, and building tools to improve security postures.</p>
          <p><strong>Areas of interest:</strong> Penetration Testing, Incident Response, Digital Forensics, Malware Analysis, Secure Code Development and Vulnerability Assessment.</p>
        </div>
      </details>
    </div>
    <div class="details-wrapper">
      <details id="education">
        <summary>🎓 Education</summary>
        <div class="details-inner">
          <ul>
            <li>Bachelor’s Degree in Computer Engineering – University of Alcalá de Henares</li>
            <li>Master’s Degree in Cybersecurity - University of Rioja</li>
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
                Certified Ethical Hacker - Cisco Networking Academy
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
            <p>Developed Visual Studio Code plugin to detect, classify and explain vulnerabilities on code.</p>
            <p class="small"><strong>Tech stack:</strong> Python, JavaScript, API integration, custom reporting.</p>
            <p class="small"><strong>Role:</strong> Full-stack security developer and analyst.</p>
            <p class="small"><strong>Outcome:</strong> Reduced manual triage time and produced actionable reports for remediation.</p>
            <!--<p><a href="https://github.com/BlancaCal/vulnerability-detection-tool" target="_blank" rel="noopener">View on GitHub</a></p> -->
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
        <li>
          <a href="mailto:blancacaldgonz@gmail.com" style="display:inline-flex; align-items:center; gap:6px;" target="_blank" rel="noopener">
            <!-- Gmail SVG icon -->
            <svg aria-hidden="true" width="20" height="20" viewBox="0 0 512 512" fill="currentColor" style="flex-shrink:0;">
              <path fill="#EA4335" d="M502.3 190.8L327.4 338.3 502.3 461.5V190.8z"/>
              <path fill="#34A853" d="M502.3 190.8L327.4 338.3 502.3 461.5V190.8zM9.7 190.8v270.7l174.9-123.2L9.7 190.8z"/>
              <path fill="#FBBC04" d="M9.7 190.8v270.7l174.9-123.2L9.7 190.8z"/>
              <path fill="#4285F4" d="M502.3 51.5H9.7C4.3 51.5 0 55.8 0 61.2v38.5c0 5.4 4.3 9.7 9.7 9.7h492.6c5.4 0 9.7-4.3 9.7-9.7V61.2c0-5.4-4.3-9.7-9.7-9.7z"/>
              <path fill="#EA4335" d="M9.7 190.8l246.3 174.5 246.3-174.5V61.2c0-5.4-4.3-9.7-9.7-9.7H19.4c-5.4 0-9.7 4.3-9.7 9.7v129.6z"/>
            </svg>
            Gmail
          </a>
        </li>
        <li>
          <a href="https://www.linkedin.com/in/blanca-calder%C3%B3n-gonz%C3%A1lez-a28313252/" target="_blank" rel="noopener" style="display:inline-flex; align-items:center; gap:6px;">
            <!-- LinkedIn SVG icon -->
            <svg aria-hidden="true" width="20" height="20" viewBox="0 0 24 24" fill="currentColor" style="flex-shrink:0;">
              <path d="M4.98 3.5C4.98 4.88071 3.88071 6 2.5 6C1.11929 6 0 4.88071 0 3.5C0 2.11929 1.11929 1 2.5 1C3.88071 1 4.98 2.11929 4.98 3.5ZM0.5 8H4.5V24H0.5V8ZM7.5 8H11.1V10.17H11.16C11.78 9.01 13.24 7.8 15.48 7.8C20.04 7.8 21 10.93 21 15.22V24H17V15.92C17 13.56 16.96 10.78 14.04 10.78C11.08 10.78 10.64 13.14 10.64 15.76V24H6.64V8H7.5Z" />
            </svg>
            LinkedIn
          </a>
        </li>
        <li>
          <a href="https://github.com/BlancaCal" target="_blank" rel="noopener" style="display:inline-flex; align-items:center; gap:6px;">
            <!-- GitHub SVG icon -->
            <svg aria-hidden="true" width="20" height="20" viewBox="0 0 24 24" fill="currentColor" style="flex-shrink:0;">
              <path d="M12 0.297C5.373 0.297 0 5.67 0 12.297C0 17.63 3.438 22.09 8.205 23.682C8.805 23.793 9.025 23.438 9.025 23.125C9.025 22.843 9.015 22.143 9.01 21.243C5.672 21.943 4.968 19.653 4.968 19.653C4.422 18.243 3.633 17.843 3.633 17.843C2.546 17.043 3.717 17.058 3.717 17.058C4.922 17.148 5.555 18.313 5.555 18.313C6.633 20.098 8.388 19.618 9.075 19.313C9.185 18.543 9.5 17.993 9.85 17.693C7.155 17.393 4.344 16.333 4.344 11.653C4.344 10.323 4.797 9.223 5.555 8.363C5.425 8.063 5.045 6.823 5.665 5.123C5.665 5.123 6.695 4.803 8.995 6.353C9.985 6.083 11.045 5.95 12.105 5.945C13.165 5.95 14.225 6.083 15.215 6.353C17.515 4.803 18.545 5.123 18.545 5.123C19.165 6.823 18.785 8.063 18.655 8.363C19.415 9.223 19.865 10.323 19.865 11.653C19.865 16.345 17.05 17.392 14.345 17.692C14.805 18.073 15.225 18.833 15.225 20.003C15.225 21.693 15.215 22.843 15.215 23.125C15.215 23.438 15.435 23.8 16.045 23.682C20.81 22.09 24.25 17.63 24.25 12.297C24.25 5.67 18.877 0.297 12.25 0.297H12Z" />
            </svg>
            GitHub
          </a>
        </li>
      </ul>
    </div>
  </details>
</div>
  </div>

  <div class="footer">
    <p>Thanks for visiting — committed to securing systems and empowering users through informed defense. 🛡️</p>
  </div>
</div>
