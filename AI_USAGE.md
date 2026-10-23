# Záznam použití AI

- **Nástroj:** OpenAI Codex.
- **Model:** prostředí označuje hlavního asistenta jako Codex založený na GPT-6. Přesný identifikátor varianty modelu není spolehlivě zpřístupněn; neuvádíme odhad.
- **Datum práce:** 23. října 2026 (Europe/Prague, datum poskytnuté prostředím uživatele).

## Zadání

Uživatel poskytl podrobný anglický brief začínající „PROJECT: APEX MOTORS — Premium Automotive One-Page Website“ a vlastní pravidla AGENTS.md. Následuje věrný záznam požadavků, nikoli údajná doslovná kopie celého promptu:

Vytvořit a skutečně implementovat mimořádně propracovaný český jednostránkový web fiktivního luxusního autosalonu APEX MOTORS. Použít pouze HTML5 a CSS3, absolutně žádný JavaScript, knihovny, build nebo backend. Veškerý obsah vložit do `index.html`, veškeré vlastní styly do `style.css`. Zvolit tmavou paletu s decentní zlatou, velkou editorialovou typografii, kvalitní legálně použitelné fotografie a responzivní rozvržení.

Zahrnout viditelné upozornění na školní projekt, navigaci Úvod / O nás / Vozidla / Proč Apex / Kontakt, výrazný hero, příběh fiktivní značky, šest vozů (Porsche 911 GT3 RS, Lamborghini Huracán STO, Ferrari 296 GTB, Mercedes-AMG GT, McLaren 720S, Audi R8 V10), samostatný editorial Porsche, hodnoty značky, závěrečný odkaz na portfolio a zápatí. Nepředstírat skutečný autosalon, skladové zásoby, prodej, ceny, kontakty nebo neověřené parametry. Nepoužívat nefunkční formuláře či tlačítka.

Dodržet sémantiku, český jazyk, metadata, klávesnicovou přístupnost, fokus, redukovaný pohyb a rozvržení při šířkách 375, 768, 1024, 1440 a 1920 px. Odkazovat na oba validátory W3C, přiznat AI, dokumentovat skutečné zdroje a licence fotografií. Připravit README s nasazením na GitHub Pages. Nic nevydávat za úspěšně validované či nasazené bez ověření. Neprovádět nesouvisející změny.

Uživatel následně zadal cílové portfolio **https://vojtechbedan.github.io/**.

## Použití a výstupy

AI navrhla původní vizuální identitu a rozvržení, vytvořila české texty, `index.html`, `style.css` a dokumentaci. Pomocný agent provedl vyhledání fotografií na Wikimedia Commons, ověření autorů a licencí, vizuální kontrolu modelů a lokální optimalizaci do WebP. Fotografie nejsou generované AI; jejich autoři jsou uvedeni v `ASSETS.md` i přímo v zápatí stránky.

Byly použity pokyny dovednosti Sites pro návrh a ověření lokálního webu. Výsledkem je statický projekt v uživatelem určeném workspace, bez publikace do Sites. Python a nástroje prohlížeče byly použity pouze při přípravě a kontrole; nejsou součástí webu ani jeho závislostmi.

## Ověření a lidské zásahy

Uživatel poskytl zadání, pracovní pravidla a URL portfolia. V tomto pracovním běhu nejsou zaznamenány ruční úpravy kódu ani lidské schválení finálního vizuálu. Automatické a vizuální kontroly provedené AI nejsou prezentovány jako lidská kontrola.

Skutečné vykreslení v Microsoft Edge bylo zkontrolováno při všech pěti požadovaných šířkách i s vypnutým vykonáváním skriptů. Byly pořízeny dočasné snímky mimo odevzdávaný projekt a vizuálně posouzeny desktopový a mobilní úvod, kolekce, editorial Porsche a závěrečná sekce. Rozměry dokumentu ani kontrolované textové prvky nevykázaly horizontální přetečení. Všech devět umístění šesti fotografií se úspěšně načetlo; grid měl očekávaný jeden, dva a tři sloupce. Byla ověřena funkce nativního rozbalení atribucí, první klávesnicový fokus na odkazu pro přeskočení navigace a hodnota `scroll-behavior: auto` při redukovaném pohybu. Statická kontrola potvrdila existenci lokálních odkazů a kotev, jedinečná ID, alt texty, jediné h1, absenci skriptů, obsluh událostí, JavaScript URL a vložených stylů.

Odeslání zdrojových souborů do online validátorů W3C zablokovala automatická kontrola oprávnění kvůli předání lokálního kódu externí službě. Bez obcházení tohoto omezení byl následně stažen oficiální Nu Html Checker a spuštěn pouze lokálně. Po odstranění nepřípustného `aria-label` na obecném `div` prošly `index.html` i `style.css` kontrolou `--also-check-css --format json` ve verzi 26.10.12 (0a70d65): prázdný seznam zpráv, návratový kód 0. Výsledky neznamenají provedení online kontroly službou W3C Jigsaw.

Nasazení na GitHub Pages ani úprava externího portfolia nebyly provedeny.

## Následná změna názvu

Dne 23. října 2026 uživatel zadal: „přejmenuj to na Vojta motors“. Značka byla přejmenována na VOJTA MOTORS v titulku, metadatech, logu, navigaci, textech a dokumentaci. Upraveny byly také kotvy, dekorativní iniciála na V a symbol značky. Původní zadání výše je zachováno jako historický záznam.
