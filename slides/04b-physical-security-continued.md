---
layout: default
---

# Fyzická bezpečnost – co dnes (záměrně) nepokrýváme

<div class="callout">
Dnes jsme probrali opatření 7.1–7.7. Annex A 7 má celkem <strong>14 opatření</strong> — zbytek si zaslouží vlastní pozornost, minimálně na úrovni přehledu.
</div>

| Opatření | Co řeší |
|----------|---------|
| **7.8** Umístění a ochrana zařízení | Bezpečné umístění serverů/obrazovek, ochrana proti prostředí (teplota, vlhkost, EM záření) |
| **7.9** Zabezpečení aktiv mimo prostory | Notebooky, telefony mimo kancelář — návaznost na VPN a remote access (8.20) |
| **7.10** Paměťová média | Životní cyklus USB/HDD/pásek — pořízení, šifrování, likvidace |
| **7.11** Podpůrné utility | Elektřina, chlazení, telekomunikace |
| **7.12** Bezpečnost kabeláže | Ochrana síťové a napájecí kabeláže proti odposlechu a poškození |
| **7.13** Údržba zařízení | Bezpečná údržba bez zavedení nových rizik |
| **7.14** Bezpečná likvidace/reuse zařízení | Bezpečné smazání dat před vyřazením nebo opětovným použitím |

---
layout: default
---

# 7.8 Umístění a ochrana zařízení

Cíl: zabránit ztrátě, poškození, krádeži nebo kompromitaci zařízení a přerušení provozu organizace.

- Kritické zařízení v **kontrolovaných oblastech** — serverovny, uzamčené racky, ne v chodbách
- Obrazovky se zpracováním citlivých dat nejsou viditelné kolemjdoucím (shoulder surfing)
- Ochrana proti prostředí: požár, voda, prach, elektromagnetické rušení
- Monitoring teploty a vlhkosti s alertingem
- Přepěťová a bleskosvodná ochrana na budovách a vstupních vedeních

<div class="callout warning">
Typický scénář incidentu: výpadek klimatizace v nesledované serverovně → postupné selhání disků, dokud si toho někdo nevšimne.
</div>

---
layout: default
---

# 7.9 Zabezpečení aktiv mimo prostory

Zařízení mimo firemní prostory (notebooky, telefony, přenosná média) čelí zvýšenému riziku ztráty, krádeže či kompromitace — firemní fyzická ochrana už neplatí.

- Autorizace a evidence vynášeného zařízení
- Šifrování disků jako standard pro mobilní zařízení
- Zabezpečený vzdálený přístup (**návaznost na 8.20 – VPN, MFA**)
- Zásady pro práci z kavárny, hotelu, veřejné WiFi

---
layout: default
---

# 7.10 Paměťová média

Životní cyklus paměťových médií: **pořízení → autorizace → použití → přeprava → likvidace/reuse**

- Politika pro použití vyměnitelných médií (USB, externí disky, pásky)
- **Šifrování jako výchozí stav** pro citlivá data na přenosných médiích
- Bezpečná likvidace — fyzická destrukce nebo certifikované smazání
- Kumulativní efekt: více "nekritických" médií dohromady může tvořit citlivý celek
- Poškozené zařízení s citlivými daty → risk assessment, zda opravit nebo zničit

---
layout: default
---

# 7.11 – 7.14 Ve zkratce

<div class="icon-grid">
  <div class="icon-card">
    <div class="icon">🔌</div>
    <div class="label"><strong>7.11 Podpůrné utility</strong><br/>Záložní napájení (UPS), redundantní chlazení a konektivita</div>
  </div>
  <div class="icon-card">
    <div class="icon">🔗</div>
    <div class="label"><strong>7.12 Kabeláž</strong><br/>Ochrana proti odposlechu, poškození a neoprávněnému přístupu k vedení</div>
  </div>
  <div class="icon-card">
    <div class="icon">🛠️</div>
    <div class="label"><strong>7.13 Údržba</strong><br/>Údržba jen oprávněnými osobami, bez vytvoření nových zranitelností</div>
  </div>
  <div class="icon-card">
    <div class="icon">🗑️</div>
    <div class="label"><strong>7.14 Likvidace/reuse</strong><br/>Bezpečné smazání dat před vyřazením — návaznost na 8.10 (Information Deletion)</div>
  </div>
</div>

<div class="callout">
Tato opatření budou detailněji součástí navazující lekce.
</div>
