---
layout: section
subtitle: ISO 27001 — Opatření 7.1–7.7
---

# Fyzická bezpečnost

---
layout: default
---

# Proč by vás fyzická bezpečnost měla zajímat?

<div class="callout warning">
Kybernetická bezpečnost ZAČÍNÁ fyzickou bezpečností! Sebelepší firewally nepomohou, když někdo odnese disk ze serverovny.
</div>

- ISO 27001 vyžaduje řešit fyzickou bezpečnost (kapitoly 7.1–7.8)

Vaše budoucí role:
- spolupráce s facility managementem – kdo má kam přístup?
- navrhování opatření – kde potřebujeme kamery, čtečky karet?
- řešení incidentů – ztracená karta, podezřelá osoba
- auditování – kontrola souladu s normou

---
layout: default
---

# Fyzická bezpečnost – kontextové rozdíly

<div class="icon-grid cols-2">
  <div class="icon-card">
    <div class="icon">☁️</div>
    <div class="label"><strong>Remote-first, cloud-based startup</strong><br/>Žádná vlastní serverovna – vše v cloudu (AWS, Azure). Důraz na zabezpečení domácích pracovišť a laptopů. Fyzická bezpečnost = bezpečnost koncových zařízení.</div>
  </div>
  <div class="icon-card">
    <div class="icon">🪖</div>
    <div class="label"><strong>Vojenská základna</strong><br/>Vícestupňové perimetry, ozbrojená stráž. Biometrická kontrola, skenování návštěvníků. Odstínění elektromagnetického záření, Faradayovy klece.</div>
  </div>
</div>

<div class="callout">
GRC specialistka musí vždy přizpůsobit opatření kontextu!
</div>

---
layout: default
---

# 7.1 Fyzické perimetry

- Určení bezpečnostního perimetru, který slouží k ochraně oblastí obsahujících informace a další přidružená aktiva
- Zabránění neoprávněného fyzického přístupu za účelem poškození nebo zásahu do informací organizace a souvisejících aktiv

Typická opatření:
- fyzicky celistvé obvody budovy (žádné mezery či nedostatky)
- pevné konstrukce střech, stěn, stropů, podlah
- ochrana vnějších dveří (mříže, alarmy, zámky)
- zamčené dveře a okna, především v přízemí
- požární dveře – monitoring a testování

---
layout: default
---

# 7.2 Fyzický vstup 1/3

- Zabezpečení oblastí vhodnými vstupními kontrolami a přístupovými body
- Přístup do prostor s omezeným přístupem by měly mít pouze oprávněné osoby
- Přístupová oprávnění by měla být pravidelně přezkoumávána a aktualizována
- Uchování logů o přístupech
- Zavedení procesů a technických mechanismů pro řízení přístupu tam, kde dochází ke zpracování a uchovávání informací
  - přístupové karty, biometrické údaje, MFA (karta + PIN), bezpečnostní dveře
- Recepce a kontrola osobních věcí
- Všechny osoby by měly mít viditelné označení odlišující např. zaměstnance od dodavatelů a návštěv

---
layout: default
---

# 7.2 Fyzický vstup 2/3

- Dodavatelé by měli vstupovat do „zakázaných" oblastí jen v případě nutnosti, jejich pohyb by měl být schválen a monitorován
  - zvláštní důraz na fyzickou bezpečnost v budovách, kde svá aktiva má více organizací
  - opatření k fyzickým přístupům by měla jít posílit v případě rostoucího výskytu incidentů
  - zabezpečení požárních dveří před neoprávněným vstupem
  - management fyzických klíčů, záznamová kniha, roční audit
- Návštěvníci
  - ověření totožnosti
  - záznam dne a času příchodu a odchodu
  - přidělování přístupu pouze pro konkrétní účely
  - dohled nad návštěvníky

---
layout: default
---

# 7.2 Fyzický vstup 3/3

Zásobovací a nakládací plochy a příjem materiálu:

- návrh zásobovacích a nákladních ploch tak, aby se např. řidiči kamionů nemohli dostat dále do ostatních částí budovy/areálu
- zabezpečení venkovních dveří v těchto prostorách, pokud jsou dveře do „zakázaných" oblastí otevřeny
- kontrola příchozích zásilek, zda neobsahují výbušniny, chemikálie či jiné nebezpečné materiály před dalším pohybem po areálu
- fyzické oddělení příchozích a odchozích zásilek
- prozkoumání příchozích zásilek, zda nedošlo během dopravy k poškození

---
layout: default
---

# 7.3 Security kanceláří, prostor a zařízení

Účelem je zabránit fyzickému přístupu, poškození nebo pozměnění informací a souvisejících aktiv.

Zajištění zabezpečených kanceláří, místností a vybavení:
- umístění kritických zařízení tak, aby nebyla přístupná veřejnosti
- v případě vhodnosti neoznačovat budovy zevnitř ani zvenčí, aby nebylo možné rozpoznat, kde a jaké informace se nacházejí
- příprava zařízení tak, aby nebylo možné informace vidět či slyšet (elektromagnetické stínění)
- telefonní seznamy či mapy by neměly odhalit umístění důvěrných informací neoprávněným osobám

---
layout: default
---

# 7.4 Monitoring fyzických prostor

Prostory by měly být nepřetržitě monitorovány, aby mohlo dojít k odhalení a odrazení neautorizovaného vstupu.

Monitoring prostor:
- bezpečnostní kamery
- hlídači
- alarmy
- bezpečnostní čidla (dveře, okna) – detektor pohybu, zvuku, kontaktu
- PSIM (Physical Security Information Management)

Všechny bezpečnostní systémy by měly být pravidelně testovány. Návrh monitorovacího systému by měl být utajený a nepřístupný neoprávněným osobám – vždy v souladu s místními právními předpisy.

---
layout: default
---

# 7.5 Ochrana proti přírodním a fyzickým hrozbám

Ochrana před přírodními pohromami a ostatními úmyslnými či neúmyslnými fyzikálními hrozbami. Identifikace rizik na základě risk analýzy.

Umístění či výstavba prostor by měla zohledňovat kritéria jako:
- **geografie**: nadmořská výška, vodní plochy, tektonické jevy
- **sociální (městské) hrozby**: politické nepokoje, trestná činnost, teroristické útoky

Hrozby a protiopatření:
- požár → detektory kouře, protipožární systém, hašení vhodnou látkou (speciální plyny v serverovnách)
- povodeň → detekční systém, čerpadla pro případ povodně
- elektrické přepětí → systém ochraňující servery i klienty
- výbušniny a zbraně → kontroly před vstupem

---
layout: default
---

# 7.6 Práce v zabezpečených zónách

Nastavení opatření pro práci v zabezpečených oblastech – platí pro všechny osoby, které do oblastí vstupují, a na všechny aktivity vykonávané uvnitř.

Pokyny ke zvážení:
- informování osob vstupujících do zabezpečených oblastí na principu need-to-know
- vyhýbání se práci bez dozoru v zabezpečených prostorách
- fyzické zamykání a pravidelná kontrola prázdných zabezpečených míst
- zákaz vnášení fotografického, audio a video zařízení (fotoaparáty, telefony, diktafony)
- kontrola vnášení a použití koncových zařízení
- viditelné vyvěšení nouzových postupů

---
layout: default
---

# 7.7 Clear desk and clear screen policy

Slouží ke snížení rizika neoprávněného přístupu, ztráty či zničení informací na stolech, obrazovkách či přenosných médiích, a to během i po pracovní době.

Pravidla:
- zamykání citlivých nebo kritických informací (papír i elektronická úložiště)
- ochrana koncových zařízení zámky
- opouštění koncových zařízení až po odhlášení nebo zamčení obrazovky (vhodné automatické odhlašování)
- okamžité odebrání výtisků z tiskárny a multifunkčního zařízení, autentizace u tiskáren
- bezpečné uchování informací a skartace
- omezení pop-up oken (např. e-mail), především ve veřejném prostoru
- smazání citlivých a kritických informací z white-boardů
