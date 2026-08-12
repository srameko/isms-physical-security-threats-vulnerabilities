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

---
layout: default
---

# Nejčastější chyby – Fyzická bezpečnost

<div class="callout warning">
Karta bývalého zaměstnance nebo dodavatele, která ještě rok po odchodu otvírá dveře do serverovny — jeden z nejčastějších nálezů fyzického auditu.
</div>

- Přístupová oprávnění se nikdy nepřezkoumávají – karty bývalých zaměstnanců/dodavatelů zůstávají aktivní
- Fyzická bezpečnost řešena odděleně od IT – žádná síťová segregace pro EZS, kamery či klimatizaci
- Serverovna bez monitoringu teploty a vlhkosti → postupné selhání disků, dokud si toho někdo nevšimne
- Clear desk / clear screen politika existuje jen na papíře, v praxi nevynucována
- Návštěvníci a dodavatelé bez dohledu v prostorách s omezeným přístupem
- Chybějící nebo nepravidelné kontroly kabeláže a rozvaděčů (sweepy)
- Mobilní zařízení mimo prostory bez šifrování disku a bez možnosti remote wipe
