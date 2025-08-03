---
layout: default
---

<style>
.summary-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 15px;
  margin-bottom: 30px;
}

details > summary {
  list-style: none;
  padding: 15px 20px;
  border-radius: 20px;
  background-color: #38b000;
  cursor: pointer;
  font-weight: 600;
  text-align: center;
  transition: background-color 0.25s ease;
  user-select: none;
  font-size: 0.95rem;
  position: relative;
}
details > summary::-webkit-details-marker {
  display: none;
}
details:hover > summary {
  background-color: #6BE000;
}
details[open] > summary {
  background-color: #2E8B57;
  color: white;
}

/* Content box under each summary */
.details-inner {
  background-color: #38b000;
  border-radius: 20px;
  padding: 20px;
  margin-top: 10px;
  font-size: 0.95rem;
  line-height: 1.35;
}

/* Make the summary pill and its expanded content span full width of its grid cell */
.details-wrapper {
  display: flex;
  flex-direction: column;
}

/* Responsive fallback */
@media (max-width: 900px) {
  .summary-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}
</style>

# 🛡️ Welcome to My Cybersecurity Portfolio

Hi! I'm **Blanca**, a cybersecurity enthusiast and practitioner dedicated to securing systems, networks, and applications.

---

<div class="summary-grid">
  <div class="details-wrapper">
    <details id="about-me">
      <summary>🔐 ABOUT ME</summary>
      <div class="details-inner">
      <ul style="padding-left:1em; margin:0;">
        I specialize in cybersecurity with a focus on threat detection, vulnerability assessment, and digital forensics.<br>
        <li><strong>🧠 Areas of interest:</strong> Penetration Testing, Incident Response, Digital Forensics, Malware Analysis, Secure Code Development, Vulnerability assesment</li>
      </ul>
      </div>
    </details>
  </div>

  <div class="details-wrapper">
    <details id="education">
      <summary>🎓 EDUCATION</summary>
      <div class="details-inner">
      <ul style="padding-left:1em; margin:0;">
        <li>Bachelor’s Degree in Computer Science Engineering</li>
        <li>Master’s Degree in Cybersecurity</li>
        <li>English: C1 – Advanced professional proficiency</li>
      </ul>  
      </div>
    </details>
  </div>

  <div class="details-wrapper">
    <details id="technical-skills">
      <summary>🛠️ TECHNICAL SKILLS</summary>
      <div class="details-inner">
      <ul style="padding-left:1em; margin:0;">
        <li><strong>Security Tools:</strong> Metasploit, Burp Suite, Nmap, Nessus, CNAPP tools, Fortify, Wireshark, OWASP ZAP</li>  
        <li><strong>Forensic Tools:</strong> FTK imager, Autopsy, Wondershare DR. Phone</li>
        <li><strong>OSINT Tools:</strong> Maltego, Google Dorks, Foca, Shodan, The Harvester</li>
        <li><strong>Languages:</strong> Python, Bash, PowerShell, Java</li>
        <li><strong>Frameworks & Platforms:</strong> Kali Linux</li>  
        <li><strong>Practices:</strong> Secure Code Review, Threat Hunting, Ethical Hacking, Attack Surface Management, Security Hardening, Endpoint Protection </li>
      </ul> 
      </div>
    </details>
  </div>

  <div class="details-wrapper">
    <details id="certifications">
      <summary>📜 CERTIFICATIONS</summary>
      <div class="details-inner">
      <ul style="padding-left:1em; margin:0;">
        <li> <a href="https://www.credly.com/badges/f271ee76-5012-409a-804e-84ee6423206a" target="_blank" rel="noopener">Ethical Hacker by Cisco Networking Academy </a></li>  
        <li> Cyber Intelligence and Open Source Intelligence (OSINT) by CCN-CERT Centro Criptológico Nacional</li>  
        <li><a href="https://cyberlandsec.com/certificate/22d40978/" target="_blank" rel="noopener">Certified Ethical Hacking and Penetration Tester (CEHPT) by CyberLand Sec</a></li>  
        <li><a href="https://www.credly.com/badges/863e20e5-b2ba-4729-b816-abb2eca382b2/public_url" target="_blank" rel="noopener">Azure Fundamentals by Microsoft</a></li>
      </ul>
      </div>
    </details>
  </div>

  <div class="details-wrapper">
    <details id="projects">
      <summary>📂 PROJECTS</summary>
      <div class="details-inner">
      <ul style="padding-left:1em; margin:0;">
        <li><strong>Vulnerability Detection Tool on code </strong></li>
      </ul>
      </div>
    </details>
  </div>

  <div class="details-wrapper">
    <details id="contact">
      <summary>📫 CONTACT</summary>
      <div class="details-inner">
        <ul style="padding-left:1em; margin:0;">
          <li>📧 Email: <a href="mailto:blancacaldgonz@gmail.com" target="_blank" rel="noopener">blancacaldgonz@gmail.com</a></li>
          <li>💼 <a href="https://www.linkedin.com/in/blanca-calder%C3%B3n-gonz%C3%A1lez-a28313252/" target="_blank" rel="noopener">LinkedIn</a></li>
          <li>🔒 <a href="https://github.com/BlancaCal" target="_blank" rel="noopener">GitHub</a></li>
        </ul>
      </div>
    </details>
  </div>
</div>
---

> Thanks for visiting — stay safe out there! 🛡️
