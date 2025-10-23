# Gæðakrafa lýst í PLanguage 

> Þetta skjal sýnir hvernig á að skilgreina eina **gæðakröfu** með aðferðinni **P-Language** samkvæmt Wiegers & Beatty (kafli 14).  
> Fyllið út reiti með upplýsingum um gæðaeiginleika og mælanleg markmið.

---

## Merkimiði (TAG)
Einkvæmt auðkenni gæðakröfunnar.  
**Dæmi:** `Performance.Report.ResponseTime`

---

## Tilgangur / Ásetningur (AMBITION)
Lýsir **tilgangi** eða **ástæðu** fyrir kröfunni — hvað hún á að bæta, tryggja eða hámarka.  
**Dæmi:** Kerfið skal bregðast hratt við þegar notandi biður um að mynda skýrslu.

---

## Mælikvarði (SCALE)
Skilgreinir **hvað er mælt** og í **hvaða mælieiningum**.  
**Dæmi:** Sekúndur sem líða frá því að notandi sendir beiðni þar til skýrslan byrjar að birtast.

---

## Mælir / Mæliaðferð (METER)
Lýsir **hvernig** eða **hvar** gæðaeiginleikinn er mældur og hvaða aðferð er notuð.  
**Dæmi:** Stoppklukkupróf á 30 dæmigerðum skýrslum samkvæmt skilgreindu notkunarferli.

---

## Markmið (GOAL)
Lágmarksgildi sem **verður að nást** til að kröfunni sé fullnægt.  
**Dæmi:** 95% allra skýrslna skulu byrja að birtast innan **8 sekúndna**.  
*(Hagsmunaaðili: Skrifstofustjóri útibús)*

---

## Æskilegt (STRETCH)
Æskilegt frammistöðugildi sem teymið reynir að ná.  
**Dæmi:** Forskilgreindar skýrslur innan 2 sekúndna, allar skýrslur innan 5 sekúndna.

---

## Óska (WISH)
Gildi í besta heimi — markmið sem væri frábært að ná, en ekki krafa.  
**Dæmi:** Allar skýrslur innan 1,5 sekúndna.

---

## Grunnkerfi (BASE PLATFORM)
Upplýsingar um viðmiðunarumhverfi fyrir mælingar.  
**Dæmi:** Fjórkjarna örgjörvi, 8 GB RAM, Windows 10, 50 % frítt minni, 70 % CPU tiltækt, tengihraði 30 Mbps.

---


✅ **Leiðbeining:**  
Þegar þú skrifar þína eigin PLanguage kröfu skaltu velja einn gæðaeiginleika og fylla út alla reiti.  
Markmiðið er að gera kröfuna **mælanlega, prófanlega og rekjanlega**.
