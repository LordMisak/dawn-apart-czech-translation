# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](https://semver.org/).

***English version** | [Česká verze](CHANGELOG_CS.md)*

## [Unreleased]
### Planned changes
- Possible future game file updates
- Monitoring new Dawn Apart versions

## [1.2.0] - 2025-08-10
### Added
- Weapon translations: weapons_cs.xml (12 items - pistols, rifles, melee weapons)
- New game objects: Oak tree in resources_cs.xml

### Changed
- Terminology: "ingredience" → "suroviny" (11 occurrences across all files)
- Space ships: "odjíždí" → "odletá" (3 occurrences for space context consistency)
- Automatic processes: "krmení" → "zásobování" (settings and hints)
- Demolition: "ODSTRANIT" → "ZBOURAT" (building demolition button)

### Fixed
- Japanese furniture: added missing translations "Tokonoma" and "Japonská postel"
- UI consistency: "VYROBENO V" → "VYRÁBÍ SE V" for better grammar
- Trader ships: "přijíždí" → "přilétá" (space context)
- Wall light names fix (removed duplicates)
- Building processes: "nainstalovat" → "postavit"

## [1.1.0] - 2025-08-09
### Added
- Game update: new files weapons_cs.xml and Trees/resources_cs.xml
- Updated FinishedTranslations.csv with minor changes

### Fixed
- Extended direct replacement implementation for new files
- Fixed Japanese furniture and duplicate name issues

## [1.0.0] - 2025-08-08
### Added
- Complete Czech translation for Dawn Apart game (39 files, 100% coverage)
- Implementation by direct replacement of English _en.xml files
- GitHub repository with complete documentation
- Installation guide and technical notes

### Changed
- Game settings: language = 4 for Czech

### Fixed
- Resolved issue with Czech not showing in game menu
- All game texts, menus, and interface translated to Czech

---

## Versioning Notes
- **Major version (X.0.0)**: Breaking changes in translation structure
- **Minor version (0.X.0)**: New translations, significant terminology changes
- **Patch version (0.0.X)**: Minor fixes, grammatical corrections

## File Structure
All translated files are located in the `translations/` folder and organized by game categories (Buildings, Items, Quests, etc.).