# VOJTA MOTORS

Český jednostránkový web fiktivního prémiového autosalonu. Školní a portfoliový projekt zaměřený na automobilový design. Nejde o skutečnou obchodní nabídku ani provozovaný autosalon.

## Spuštění

Otevřete `index.html` v prohlížeči. Není potřeba instalace, sestavení, server ani internetové připojení pro zobrazení webu. Externí odkazy samozřejmě vyžadují internet.

## Technologie a funkce

- Sémantické HTML5 a jediný soubor CSS3; **žádný JavaScript**, frameworky nebo runtime závislosti.
- Responzivní rozvržení pomocí Grid a Flexbox, plynulá typografie a lokální WebP fotografie.
- Funkční kotvy, viditelný fokus, odkaz pro přeskočení navigace a respektování omezeného pohybu.
- Šest identifikovaných modelů, samostatná prezentace Porsche 911 GT3 RS a původní vizuální identita.
- Viditelné upozornění na školní projekt v záhlaví i zápatí, skutečný odkaz na portfolio a odkazy na validátory W3C.
- Zdroje fotografií a AI jsou přiznány v zápatí a v samostatné dokumentaci.

## Soubory

```text
index.html        Veškerý obsah webu
style.css         Veškeré vlastní styly
AI_USAGE.md       Záznam skutečného použití AI
ASSETS.md         Autoři, zdroje, licence a úpravy fotografií
README.md         Tento návod
assets/images/    Šest lokálních fotografií WebP
```

## Portfolio

Závěrečné tlačítko odkazuje na uživatelem poskytnuté portfolio: https://vojtechbedan.github.io/.

Pro změnu vyhledejte komentář `PORTFOLIO_URL` v `index.html` a upravte `href` následujícího odkazu. VOJTA MOTORS je skutečně implementovaný projekt připravený k prezentaci v portfoliu. Samotný externí web portfolia nebyl v tomto workspace upraven; po publikaci v něm přidejte položku VOJTA MOTORS s URL tohoto projektu.

## GitHub Pages

1. Nahrajte obsah této složky do kořene svého GitHub repozitáře. Zachovejte strukturu `assets/images/`.
2. Otevřete **Settings → Pages → Deploy from a branch → main → /(root)** a uložte nastavení.
3. Po dokončení nasazení otevřete adresu zobrazenou GitHubem. Ověřte načtení fotografií, navigaci a odkaz na portfolio.

Uživatelský repozitář se musí jmenovat `<uživatel>.github.io`; jeho web běží na `https://<uživatel>.github.io/`. Projektový repozitář může mít jiný název, například `OneSinglePage`, a běží na `https://<uživatel>.github.io/OneSinglePage/`. Relativní cesty v tomto projektu fungují v obou variantách. Pokud již máte na hlavní adrese portfolio, použijte projektový repozitář, aby zůstalo zachováno.

Tento workspace při zahájení neobsahoval Git repozitář. Nebyl proveden commit, push ani nasazení na GitHub Pages.

## Ověření

Web byl skutečně vykreslen v Microsoft Edge při šířkách 375, 768, 1024, 1440 a 1920 px, se zakázaným vykonáváním skriptů. Kontrola rozměrů nezjistila horizontální přetečení dokumentu ani kontrolovaných textových prvků. Všech devět umístění šesti fotografií se načetlo. Ověřeny byly sloupce kolekce 1/2/3, první klávesnicový fokus na odkazu pro přeskočení navigace, rozbalení atribucí a vypnutí plynulého posuvu při omezeném pohybu. Místní kontrola HTML potvrdila platné cíle kotev, existující lokální soubory, jedinečná ID, alternativní texty a nepřítomnost JavaScriptu i vložených stylů.

**HTML i CSS úspěšně prošly lokálním [Nu Html Checker](https://validator.github.io/validator/) verze 26.10.12 (0a70d65), bez chyb a varování.** Kontrola opravila nepřípustný popisek ARIA na obecném prvku. Reprodukovatelný příkaz po stažení oficiálního `vnu.jar` a s Java 17 nebo novější:

```text
java -jar /cesta/k/vnu.jar --also-check-css --format json index.html style.css
```

Výsledek: `{"version":"26.10.12 (0a70d65)","messages":[]}`, návratový kód 0. Validátor je pouze vývojový nástroj, není součástí webu.

Odkazy v zápatí otevírají [validátor HTML](https://validator.w3.org/) a [validátor CSS](https://jigsaw.w3.org/css-validator/). Online kontrola přes tyto služby neproběhla: automatická kontrola oprávnění zablokovala odeslání místního kódu. Místo toho byl použit výše uvedený lokální validátor bez odeslání zdrojů. Web nepoužívá oficiální validační odznaky. Po zveřejnění lze do online služeb zadat veřejnou URL.

## Zdroje a AI

Podrobné licence, odkazy a autoři všech šesti fotografií jsou v [ASSETS.md](ASSETS.md). Fotografie a jejich upravené verze jsou pod CC BY-SA 4.0; tato licence sama o sobě neurčuje licenci HTML/CSS. Při dalším použití zachovejte odpovídající atribuce.

Záznam použití OpenAI Codex a zadání najdete v [AI_USAGE.md](AI_USAGE.md). Projekt neuvádí neověřené technické specifikace, ceny, dostupnost ani smyšlené kontaktní údaje.
