---
layout: default
---

<style>
/* Container grid for the six summary boxes */
.summary-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 15px;
  margin-bottom: 30px;
}

/* Summary pill style */
details > summary {
  list-style: none;
  padding: 15px 20px;
  border-radius: 20px;
  background-color: #7CFC00;
  cursor: pointer;
  font-weight: 600;
  text-align: center;
  transition: background-color 0.25s ease;
  display: inline-block;
  user-select: none;
  font-size: 0.95rem;
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

/* Expanded content box: full width under grid */
.detail-content {
  background-color: #7CFC00;
  border-radius: 20px;
  padding: 25px;
  margin-top: 10px;
  font-size: 1rem;
  line-height: 1.35;
}

/* Ensure the expanded content spans full container width */
.detail-wrapper {
  margin-bottom: 40px;
}

/* Responsive fallback: stack on narrow viewports */
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
  <div>
    <details id="about-me">
      <summary>🔐 ABOUT ME</summary>
    </details>
  </div>
  <div>
    <details id="education">
      <summary>🎓 EDUCATION</summary>
    </details>
  </div>
  <div>
    <details id="technical-skills">
      <summary>🛠️ TECHNICAL SKILLS</summary>
    </details>
  </div>
  <div>
    <details id="certifications">
      <summary>📜 CERTIFICATIONS</summary>
    </details>
  </div>
  <div>
    <details id="projects">
      <summary>📂 PROJECTS</summary>
    </details>
  </div>
  <div>
    <details id="contact">
      <summary>📫 CONTACT</summary>
    </details>
  </div>
</div>

<!-- Expanded content sections; users open each to reveal -->
<div class="detail-wrapper">
  <details open>
    <summary style="display:none;"></summary>
    <div class="detail-content">
      <strong>🔐 About Me</strong><br><br>
      I specialize in cybersecurity with a focus on threat detection, vulnerability assessment, and digital forensics. I’m passionate about helping individuals and organizations defend against evolving cyber threats.

      - 🧠 Areas of interest: Penetration Testing, Incident Response, SIEM, Malware Analysis  
      - 💼 Currently working at Santander bank as a Cybersecurity Analyst  
      - 🌍 Based in Guadalajara, Spain
    </div>
  </details>
</div>

<div class="detail-wrapper">
  <details>
    <summary style="display:none;"></summary>
    <div class="detail-content">
      <strong>🎓 Education</strong><br><br>
      - Computer Science Engineering  
      - Master on Cybersecurity
    </div>
  </details>
</div>

<div class="detail-wrapper">
  <details>
    <summary style="display:none;"></summary>
    <div class="detail-content">
      <strong>🛠️ Technical Skills</strong><br><br>
      - <strong>Security Tools:</strong> Wireshark, Metasploit, Burp Suite, Nmap, Nessus, CNAPP tools  
      - <strong>Languages:</strong> Python, Bash, PowerShell  
      - <strong>Frameworks & Platforms:</strong> Kali Linux  
      - <strong>Practices:</strong> Network Security, Endpoint Protection, Secure Code Review, Threat Hunting
    </div>
  </details>
</div>

<div class="detail-wrapper">
  <details>
    <summary style="display:none;"></summary>
    <div class="detail-content">
      <strong>📜 Certifications</strong><br><br>
      - Ethical Hacker (Cisco Networking Academy)  
      - Certificado de Ciberinteligencia y fuentes abiertas (CCN-CERT Centro Criptológico Nacional)  
      - Ethical Hacking and Penetration Tester (CyberLand Sec)  
      - Azure Fundamentals (Microsoft)
    </div>
  </details>
</div>

<div class="detail-wrapper">
  <details>
    <summary style="display:none;"></summary>
    <div class="detail-content">
      <strong>📂 Projects</strong><br><br>
      ### 🔍 Vulnerability Assessment Tool  
      *Description and repo coming soon.*
    </div>
  </details>
</div>

<div class="detail-wrapper">
  <details>
    <summary style="display:none;"></summary>
    <div class="detail-content">
      <strong>📫 Contact</strong><br><br>
      - 📧 Email: blanca.calderon@gmail.com  
      - 💼 [LinkedIn](https://www.linkedin.com/in/blanca-calder%C3%B3n-gonz%C3%A1lez-a28313252/)  
      - 🔒 [GitHub](https://github.com/BlancaCal)
    </div>
  </details>
</div>

---

> Thanks for visiting — stay safe out there! 🛡️
