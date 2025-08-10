# Changelog

Všechny významné změny tohoto projektu jsou zdokumentovány v tomto souboru.

Formát vychází z [Keep a Changelog](https://keepachangelog.com/cs/1.0.0/) a používá [Sémantické verzování](https://semver.org/lang/cs/).

## [Unreleased]
### Plánované změny
- Možné budoucí aktualizace herních souborů
- Sledování nových verzí hry Dawn Apart

## [1.2.0] - 2025-08-10
### Added
- Překlady zbraní: weapons_cs.xml (12 položek - pistole, pušky, zbraně na blízko)
- Nové herní objekty: Dub (Oak tree) v resources_cs.xml

### Changed
- Terminologie: "ingredience" → "suroviny" (11 výskytů napříč všemi soubory)
- Vesmírné lodě: "odjíždí" → "odletá" (3 výskyty pro konzistenci vesmírného kontextu)
- Automatické procesy: "krmení" → "zásobování" (nastavení a nápovědy)
- Demolice: "ODSTRANIT" → "ZBOURAT" (tlačítko bourání staveb)

### Fixed
- Japonský nábytek: přidány chybějící překlady "Tokonoma" a "Japonská postel"
- UI konzistence: "VYROBENO V" → "VYRÁBÍ SE V" pro lepší gramatiku
- Obchodní lodě: "přijíždí" → "přilétá" (vesmírný kontext)
- Oprava názvů nástěnných světel (odstranění duplicit)
- Stavební procesy: "nainstalovat" → "postavit"

## [1.1.0] - 2025-08-09
### Added
- Herní update: nové soubory weapons_cs.xml a Trees/resources_cs.xml
- Aktualizované FinishedTranslations.csv s drobnými změnami

### Fixed
- Rozšířena implementace přímého nahrazení o nové soubory
- Opraveny problémy s japonským nábytkem a duplicitními názvy

## [1.0.0] - 2025-08-08
### Added
- Kompletní český překlad hry Dawn Apart (39 souborů, 100% pokrytí)
- Implementace přímým nahrazením anglických _en.xml souborů
- GitHub repository s kompletní dokumentací
- Instalační příručka a technické poznámky

### Changed
- Nastavení hry: language = 4 pro češtinu

### Fixed
- Vyřešen problém s nezobrazováním češtiny v herním menu
- Všechny herní texty, menu a rozhraní přeloženy do češtiny

---

## Poznámky k verzování
- **Major version (X.0.0)**: Zásadní změny ve struktuře překladu
- **Minor version (0.X.0)**: Nové překlady, významné terminologické změny
- **Patch version (0.0.X)**: Drobné opravy, gramatické úpravy

## Struktura souborů
Všechny přeložené soubory se nacházejí ve složce `translations/` a jsou organizovány podle herních kategorií (Buildings, Items, Quests, atd.).