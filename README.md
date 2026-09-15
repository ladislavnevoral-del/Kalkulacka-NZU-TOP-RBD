# Kalkulačka NZÚ 2026 – bytové domy

Interní nástroj IP Polná s.r.o. pro výpočet financování revitalizace bytového domu
z programu **Nová zelená úsporám 2026** a pro rozpočítání fondu oprav na jednotlivé byty.

Celá aplikace je **jeden soubor `index.html`** – nevyžaduje instalaci, spustí se
v prohlížeči a funguje i bez připojení k internetu.

## Spuštění

Otevřete `index.html` dvojklikem, nebo – je-li zapnutý GitHub Pages – přes adresu
publikovaného webu.

Při spuštění vyberte roli:

| Role | Co vidí | Heslo |
|---|---|---|
| **Obchodník** | Parametry financování, výsledky, FO na byty, decil | ne |
| **Přípravář** | Navíc zadávání ploch konstrukcí, FVE, TČ a TUV | ano |

## Co nástroj umí

- **Výpočet výše bezúročného úvěru NZÚ** podle sazeb a limitů SFŽP (250 000 / 750 000 Kč na byt)
- **Srovnání scénářů financování** – NZÚ úvěr 2026 + banka vs. původní NZÚ (přímá dotace)
- **Rozpočet fondu oprav na jednotlivé byty** podle spoluvlastnických podílů
  (načtení vlastníků z Nahlížení do katastru, vícenáklady, nízkopříjmové bonusy, osobní vklady)
- **Úspora na vytápění** rozdělená podle podílu → sloupec *Z vlastní peněženky*
  (kolik vlastníka revitalizace reálně stojí po započtení úspory na energiích)
- **Kalkulačka decilu** – posouzení nároku na nízkopříjmový bonus (§3.4.1)
- **Exporty**: Word, PDF, Excel s živými vzorci, dopisy vlastníkům (1 strana na byt)
- **Varianty zakázky** – uložení a porovnání více variant vedle sebe

## Ukládání dat

Data žijí **pouze v prohlížeči** (localStorage). Po každé zakázce použijte
tlačítko **↓ Export** a soubor JSON si uložte – je to jediná záloha.
Odznak v hlavičce hlídá, kdy jste zálohovali naposledy.

## Nápověda

Kompletní návod je přímo v aplikaci v záložce **❓ Nápověda**
(13 kapitol včetně metodiky výpočtů, modelového příkladu a přehledu sazeb).

---

Výpočty vycházejí ze závazných pokynů SFŽP ČR pro program Nová zelená úsporám –
bytové domy (SVJ a BD), platných od 28. 5. 2026. Výstupy jsou orientačním podkladem
pro rozhodování, nejsou závaznou nabídkou financování.
