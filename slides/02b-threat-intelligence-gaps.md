---
layout: default
---

# Threat Intelligence – co s tím dál?

<div class="callout warning">
TI, které nikam nevede, je jen sbírka zajímavých článků. Auditor chce vidět: <strong>alert → analýza → akce</strong>.
</div>

**Propojení s Risk Managementem**
- Relevantní hrozby se promítají do **Risk Registru** (návaznost na Clause 6.1)
- Ke každé přijaté informaci existuje záznam — i "bez relevance", i to je výstup
- Příklad: nová TTP → aktualizace pravidla v SIEM / patch / záznam v riziku

**Kategorizace zdroje hrozby**
- Nejde jen o technické IoC, ale i o **motivaci a původ** útočníka
- Insider · Konkurence · Kyberzločinci · Státem sponzorované skupiny · Hacktivisté
- Rozlišení: masový automatizovaný útok vs. cílená kampaň na náš obor

---
layout: default
---

# Threat Intelligence – vlastnictví a proces

**Kdo to vlastní?**
- Jmenovaná osoba/role zodpovědná za pravidelný review (i "CTO každé pondělí" je v pořádku)
- "Sleduje to každý" = selhání této kontroly

**Jak často?**
- Definovaná frekvence review — týdně / kontinuálně (automatizace)
- Ad-hoc přístup bez cyklu je typický nález auditu

**Nové hrozby: AI a LLM infrastruktura**
- Standardní feedy toto většinou nepokrývají
- **Model poisoning** – manipulace trénovacích dat
- **Prompt injection** – obcházení bezpečnostních zábran LLM
- **AI-generated phishing** – sofistikovaný phishing tvořený pomocí AI

---
layout: default
---

# Nejčastější chyby – Threat Intelligence

<div class="callout warning">
„Sledujeme desítky feedů" neznamená nic, pokud z nich nevzniká jediná akce, kterou lze doložit.
</div>

- **„Shelfware" TI** – předplacené reporty a feedy, které nikdo nečte ani nevyhodnocuje
- Chybějící návaznost na **Risk Register** – relevantní hrozba se nikam nepromítne
- Nejasné vlastnictví – „sleduje to každý" ve skutečnosti znamená, že nesleduje nikdo
- Ad-hoc review bez definované frekvence namísto pravidelného cyklu
- Jen technická IoC bez kontextu – ignorování motivace a TTP útočníka (kdo a proč)
- Nepokrytí nových typů hrozeb – AI/LLM infrastruktura mimo standardní feedy
