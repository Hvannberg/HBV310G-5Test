2 Byrja upp á nýtt 
> 💡 **ATHUGIÐ:**  
> Þetta sniðmát (template) inniheldur sjálfvirkar gæðaskoðanir (GitHub Actions) sem keyra þegar þú opnar **Pull Request (PR)**.  
> Þær:
> - sýna form þar sem þú metur eigin innsendingu (t.d. „Uppfyllir atriðið matskvarða?“ og „Hvað má betur fara?“),
> - athuga að svör séu til staðar og nægilega ítarleg áður en PR má samþykkja,
> - senda áminningu ef eitthvað vantar.
>
> 🔧 **Eftir að þú býrð til repo úr þessu sniðmáti**, vertu viss um að:
> 1. Virkja **GitHub Actions** undir *Settings → Actions → General → Allow all actions*, og
> 2. Setja „PR Quality Check“ sem *required check* undir *Settings → Branches*.
>
> Sjá nánar leiðbeiningar neðst í þessari skrá.

# Verkefni 5 — Gæðaeiginleikar (HBV301G)

Setjið ykkar eigin texta um **verkefnið ykkar** og takið út eða aðlagið textann hér að neðan að ykkar verkefni. 

## Nafn kerfis

## Stutt lýsing á kerfi 

## Hópmeðlimir 


## Yfirlit
Í þessu verkefni veljið þið **5 ytri** (external) og **3 innri** (internal) gæðaeiginleika fyrir kerfið ykkar (úr Verkefni 1 eða nýtt kerfi).  
Fyrir **hvern** eiginleika:
- Skrifið **1 gæðakröfu** 
  Viðbótarskilyrði: Fyrir einn af eiginleikunum skrifaðu gæðakröfu í formlegri setningu (PLanguage). Fyrir aðra eiginleika, skrifaðu  gæðakröfuna í óformlegri setningu (informal sentence form)
- Bætið við **2–3 röksetningum** um af hverju krafan á við og hvaða **forsendur** gilda.

Veljið síðan **3 pör** úr þessum eiginleikum:
- Lýsið í **2–3 setningum** mögulegum **árekstri** milli þeirra.
- Rökstyðjið **forgangsröðun**: hvor fær að ganga fyrir og af hverju.

## Mappa & skráauppsetning
- `answers/quality-attributes.md` — allar 8 kröfurnar (5 ytri, 3 innri).
- `answers/conflicts.md` — 3 árekstrapör + rök.
- `templates/QUALITY_ATTRIBUTE.md` — endurnýtið fyrir hvern gæðaeiginleika.
- `templates/CONFLICT_PAIR.md` — endurnýtið fyrir hvert par.
- `templates/PLANGUAGE.md` — Sniðmát fyrir eina gæðakröfu skrifaða með **PLanguage** samkvæmt kafla 14 í *Wiegers & Beatty*. |
- `docs/glossary.md` — *(valfrjálst)* orðasafn hugtaka.

## Hvernig á að vinna verkefnið með þessu repo-i 
1. Opnið sniðmát í `templates/`.
2. Afritið (copy) og límið í `answers/quality-attributes.md` eða búið til sérskrár ef óskað er.
3. Fyllið út. Notið **kerfissértækar** forsendur (notendafjölda, tengingar, rekstrarumhverfi o.s.frv.).
4. Gerið commit /push með skýrum skilaboðum.
5. Samstarfsnemandinn á að rýna pull request og skrifa athugasemdir 

## Dæmi — ein stutt færsla
**Gæðaeiginleiki (ytri):** Afköst (Performance)  
**Krafa (óformleg):** Kerfið skal svara vefbeiðnum á innan við 500 ms að meðaltali undir venjulegu álagi.  
**Rök/forsendur (2–3 setn.):** Notendur hætta við aðgerðir ef bið > 1s. Við reiknum með allt að 300 samhliða notendum í hámarki; CDN og gagnagrunnsbætur styðja markið.

> Ath.: Þetta er *leiðbeinandi* dæmi. Notið eigin tölur/forsendur.
> 
> ---

## 🔧 Uppsetning eftir að þú býrð til repo úr sniðmáti

Þetta sniðmát inniheldur sjálfvirkar athuganir og spurningar sem hjálpa þér að skila verkefni í góðu formi.
Til að þær virki í þínu eigin repo þarftu að virkja þær í stillingum.

---

### 🧩 1. Virkja GitHub Actions

1. Farið í **Settings → Actions → General**
2. Skrunaðu niður að “Actions permissions”
3. Veldu ✅ **Allow all actions and reusable workflows**
4. Smelltu á **Save**

Þetta gerir PR Quality Check og Nudge Comment workflow virkt.

---

### 🧠 2. Sjálfvirkar athuganir (PR Quality Check)

- Í hvert skipti sem þú opnar eða breytir Pull Request, keyrir athugun sem tryggir að þú hafir svarað
  spurningum um gæði, læsileika og umbætur.
- Ef eitthvað vantar eða er of stutt svar, birtist rauður ⚠️ *“PR Quality Check failed”* undir **Checks** flipanum.

✅ **Ábending:** Bættu síðan við þessi skref í „Branch Protection Rules“ (ef þú mátt breyta stillingum repoins):

1. Farið í **Settings → Branches → Add rule**
2. Skrifaðu `main` undir “Branch name pattern”
3. Merktu við:
  - ✅ Require a pull request before merging
  - ✅ Require status checks to pass before merging
4. Undir “Status checks” veldu **PR Quality Check**
5. Vistaðu.

Þá má ekki sameina PR fyrr en checkið er grænt ✅.

---

### 🧾 3. PR form (sjálfmat og athugasemdir)

Þegar þú býrð til nýtt **Pull Request**, opnast sjálfkrafa form sem spyr:
- Uppfyllir atriðið matskvarða verkefnisins?
- Er textinn læsilegur og réttur?
- Hvað má betur fara?

👉 Fylltu út þessi svör áður en þú sendir PR til yfirferðar.
Ef þú gleymir því, þá skrifar GitHub-botinn sjálfkrafa áminningu í athugasemd.

---

### 📊 4. Hvernig þetta lítur út í framkvæmd

1. Búðu til nýja grein og breyttu einhverju (t.d. README).
2. Opnaðu Pull Request.
3. Svaraðu spurningunum í forminu.
4. Skoðaðu flipann **Checks** — hann sýnir hvort PR Quality Check er í lagi.
5. Ef rauður ⚠️ kemur upp → bættu við svör eða lengd texta og vistaðu PR aftur.

---

### 💡 5. Ef eitthvað virkar ekki

- Athugaðu að þú sért á **main** (eða aðal) grein áður en þú býrð til PR.
- Farðu í **Actions** flipann — þar sérðu hvort workflow keyrir eða hvort það hefur verið stöðvað.
- Ef það segir *“Workflow runs are disabled for this repository”* → þá þarftu að virkja Actions eins og í skrefi 1.

---

### ✅ Samantekt

| Skref | Tilgangur | Hvar | 
|-------|------------|------|
| 1️⃣ Virkja Actions | Leyfa workflow keyrslur | Settings → Actions → General |
| 2️⃣ Stilla Branch Protection | Tryggja að PR sé grænt áður en merge | Settings → Branches |
| 3️⃣ Fylla út PR form | Sjálfsmat á gæðum og umbótum | Pull Request skref |
| 4️⃣ Fylgjast með Checks | Sjá hvort athuganir standist | Pull Request → Checks |

---

---
