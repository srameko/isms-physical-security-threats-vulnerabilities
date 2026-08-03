---
layout: default
---

# Co (záměrně) nepokrýváme

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
- Zařízení nikdy nenechávat bez dozoru na veřejnosti, ochrana obrazovky před nahlédnutím (např. ve vlaku)
- **Remote wipe a location tracking** – dálkové dohledání a smazání dat při ztrátě/krádeži

---
layout: default
---

# 7.10 Paměťová média

Životní cyklus paměťových médií: **pořízení → autorizace → použití → přeprava → likvidace/reuse**

- Politika pro použití vyměnitelných médií (USB, externí disky, pásky)
- **Šifrování jako výchozí stav** pro citlivá data na přenosných médiích
- Registrace a evidence vyměnitelných médií, omezení/blokace USB a SD slotů, pokud nejsou byznysově nutné
- Uložení v trezoru dle úrovně klasifikace informací
- Bezpečná likvidace — fyzická destrukce nebo certifikované smazání
- Kumulativní efekt: více "nekritických" médií dohromady může tvořit citlivý celek
- Poškozené zařízení s citlivými daty → risk assessment, zda opravit nebo zničit

---
layout: default
---

# 7.11 Podpůrné utility

Výpadek elektřiny, chlazení nebo konektivity může způsobit stejnou škodu jako kybernetický útok.

- Redundantní napájení (UPS, záložní generátor) a chlazení, oddělené přívodní trasy
- Pravidelné testování podpůrných systémů a alarmy při poruše
- **Síťová segregace** – zařízení podpůrných utilit (klimatizace, EZS) v samostatné síti oddělené od IT infrastruktury (nová povinnost v ISO 27001:2022)
- Připojení k internetu jen pokud je nezbytné, a vždy zabezpečené
- Nouzové vypínače/uzávěry elektřiny, vody a plynu v blízkosti výstupů, nouzové osvětlení

---
layout: default
---

# 7.12 Bezpečnost kabeláže

- Silové a datové/komunikační kabely vedeny oddělené, aby se předešlo rušení
- Uložení kabelů pod zemí nebo v pancéřovaných chráničkách, kde je to možné
- Kritické spoje: uzamčené rozvaděče/patch panely, alarmy na svorkovnicích, elektromagnetické stínění
- Pravidelné technické prohlídky (sweepy) — kontrola, že nikdo nenapojil odposlechové zařízení
- **Označení kabelů na začátku a konci** (zdroj a cíl) pro snadnou identifikaci a kontrolu (nová povinnost v ISO 27001:2022)

---
layout: default
---

# 7.13 – 7.14 Ve zkratce

<div class="icon-grid cols-2">
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
