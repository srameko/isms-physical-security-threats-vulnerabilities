---
layout: section
subtitle: ISO 27001 — Opatření 5.7
---

# Threat Intelligence

---
layout: default
---

# Proč by vás TI měl zajímat?

- **Jako bezpečnostní analytička** – budete denně pracovat s IoC a analyzovat alerty
- **Jako GRC specialistka** – využijete TI pro argumentaci, proč investovat do bezpečnosti
- **V incident response** – pochopíte, kdo útočí a jak, což zrychlí reakci

<div class="callout warning">

**Příklad z praxe: FN Brno (2020)** — ransomwarový útok během covidu, obnova trvala měsíce a stála přes 300 mil. Kč. Příčinou bylo otevření věrohodně vypadajícího e-mailu. Kvalitní Threat Intelligence by upozornila, že skupina Defray cílí na zdravotnictví.

</div>

---
layout: default
---

# Threat Intelligence – k čemu slouží?

- Poskytuje povědomí o možných hrozbách, kterým organizace může čelit
- Díky povědomí o těchto hrozbách organizace může:
  - vytvořit taková opatření, aby organizace neutrpěla újmu
  - snížit dopad takových hrozeb
- Někdy nazývána jako **CTI – Cyber Threat Intelligence** – CTI lze outsourcovat jako službu

---
layout: default
---

# Pojmy

**Indicators of Compromise (IoC)** – data, která naznačují, že by systém mohl být infiltrován kybernetickou hrozbou

- Neobvyklý provoz sítí – především odchozí
- Neobvyklé přihlašovací pokusy
- Elevace oprávnění (privilege escalation)
- Změny v nastavení systému
- Neočekávané instalace softwaru a updaty
- Mnohonásobná žádost o jeden a ten samý soubor

Zdroj: [microsoft.com – What are Indicators of Compromise](https://www.microsoft.com/en-us/security/business/security-101/what-are-indicators-of-compromise-ioc)

---
layout: default
---

# Pojmy

**Indicators of Attack (IoA)** – na rozdíl od IoC se nezaměřují na stopy po útoku, ale na chování a záměr útočníka **v reálném čase** (např. sled: spuštění kódu → persistence → lateral movement)

- Umožňují zachytit útok ještě před dokončením – proaktivní obrana, ne jen forenzní analýza
- Nezávislé na konkrétním malwaru – zaměřené na taktiky a techniky (TTPs)

Zdroj: [crowdstrike.com – Indicators of Attack (IOA)](https://www.crowdstrike.com/en-us/cybersecurity-101/threat-intelligence/indicators-of-attack-ioa/)

---
layout: default
---

# Pojmy

- **Zranitelnost (Vulnerability)** – slabé místo v IT systému, kterým útočník dokáže proniknout do systému a zaútočit
  - chyba v kódu nebo návrhu
- **Hrozba (Threat)** – záměrná nebo nahodilá událost, která může ohrozit bezpečnost informačního systému
- **Riziko (Risk)** – pravděpodobnost, že útočník využije existující zranitelnosti, která povede ke ztrátě či poškození informačního systému

---
layout: default
---

# Mitre ATT&CK

Encyklopedie útočníků – databáze taktik, technik a procedur (TTP):

- **Taktika** = proč útočník něco dělá (např. Initial Access, Persistence)
- **Technika** = jak to dělá (např. Phishing, Valid Accounts)
- **Procedura** = konkrétní implementace techniky

Standardizovaný jazyk pro komunikaci o hrozbách, např.:
- `T1566.001` = Phishing s přílohou
- `T1566.002` = Phishing s odkazem

Volně dostupné online: [attack.mitre.org](https://attack.mitre.org/)

---
layout: default
---

# 3 úrovně Threat Intelligence

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">🌍</div>
    <div class="label"><strong>Strategická</strong><br/>Pochopení celkového prostředí hrozeb a jeho vývoje na nejvyšší úrovni. Zahrnuje geopolitické, ekonomické a oborově specifické faktory. Napomáhá tvořit dlouhodobé bezpečnostní strategie.</div>
  </div>
  <div class="icon-card">
    <div class="icon">🎯</div>
    <div class="label"><strong>Taktická</strong><br/>Detailnější než strategická úroveň. Soustředí se na konkrétní taktiky, techniky a procedury útočníků (TTP). Slouží k tvorbě bezpečnostních kontrol, incident response plánů a zlepšení detekce.</div>
  </div>
  <div class="icon-card">
    <div class="icon">⚙️</div>
    <div class="label"><strong>Operativní</strong><br/>Práce s informacemi v reálném čase na konkrétních IoC a zranitelnostech. Pomáhá detekovat bezpečnostní incidenty – každodenní práce.</div>
  </div>
</div>

---
layout: default
---

# Threat Intelligence – zdroje

Operativní úroveň (vnitřní), např.:

- **SIEM** (Security Information and Event Management)
- **EDR** (Endpoint Detection and Response)
- **IPS** (Intrusion Prevention System)
- **Vulnerability Management**
- **SOAR** (Security Orchestration, Automation and Response)

---
layout: default
---

# Threat Intelligence – zdroje

Taktická a strategická úroveň (vnější) – **OSINT** (Open Source Intelligence):

- vše, co je veřejně dohledatelné
- webové stránky dodavatelů softwaru
- různé národní agentury a organizace
- sociální sítě
- OSINT report speciálně pro vaši organizaci (např. i dark web)
- [Have I Been Pwned](https://haveibeenpwned.com/): kontrola, zda byl váš e-mail vystaven v úniku dat

---
layout: default
---

# Threat Intelligence – zdroje

- [misp-project.org](https://www.misp-project.org/) – MISP, platforma pro sdílení IoC
- [cisa.gov – Resources & Tools](https://www.cisa.gov/resources-tools/all-resources-tools)
- [cisa.gov – Cybersecurity Advisories](https://www.cisa.gov/news-events/cybersecurity-advisories)
- [cisa.gov – Advisory AA24-249A](https://www.cisa.gov/news-events/cybersecurity-advisories/aa24-249a)
- [cisa.gov – Known Exploited Vulnerabilities (KEV) Catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog) – zranitelnosti reálně zneužívané útočníky

---
layout: default
---

# Threat Intelligence – druhy zdrojů

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">💼</div>
    <div class="label"><strong>Komerční zdroje</strong><br/>Mandiant Threat Intelligence Report · Recorded Future · CrowdStrike</div>
  </div>
  <div class="icon-card">
    <div class="icon">🏛️</div>
    <div class="label"><strong>Vládní a mezinárodní zdroje</strong><br/>NUKIB (nukib.gov.cz) – varování a doporučení pro ČR · ENISA (agentura EU pro kybernetickou bezpečnost) · CISA (USA) – cisa.gov/cybersecurity-advisories</div>
  </div>
  <div class="icon-card">
    <div class="icon">🤝</div>
    <div class="label"><strong>Komunitní a open-source</strong><br/>MISP – platforma pro sdílení IoC · ISAC – oborové sdílení informací (finance, zdravotnictví…) · VirusTotal, AlienVault OTX</div>
  </div>
</div>
