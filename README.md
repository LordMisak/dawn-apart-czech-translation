# Dawn Apart - Czech Translation / Český překlad

![Dawn Apart](https://img.shields.io/badge/Game-Dawn%20Apart-blue)
![Translation Status](https://img.shields.io/badge/Translation-Complete-brightgreen)
![Language](https://img.shields.io/badge/Language-Czech-red)

## English

### About
This repository contains a complete Czech translation for the game **Dawn Apart**. The translation includes all game texts, UI elements, menus, and dialogues.

### Translation Status
- ✅ **Complete** - 38 XML files translated
- ✅ **All game modules covered** - UI, gameplay, items, buildings, quests, etc.
- ✅ **Fully playable** in Czech
- ⚠️ **Current limitation** - Czech language not visible in game menu (requires developer implementation)

### Current Implementation
Due to the game not having built-in modding support for languages yet, we're using a workaround:
- Replacing English `_en.xml` files with Czech translations
- Game runs fully in Czech but displays "English" in language menu

### Files Included
- **38 XML translation files** organized by game modules
- **FinishedTranslations.csv** - complete translation database
- **Installation guide** for testing

### For Developers
We're working with the development team to implement proper modding support for languages. This repository provides:
- Complete Czech localization data
- Current file structure analysis
- Implementation suggestions

### Contact
- Translator: Michal (LordMisak)
- For questions about implementation or translation details, please open an issue

---

## Česky

### O projektu
Tento repozitář obsahuje kompletní český překlad hry **Dawn Apart**. Překlad zahrnuje všechny herní texty, uživatelské rozhraní, menu a dialogy.

### Stav překladu
- ✅ **Dokončeno** - 38 XML souborů přeloženo
- ✅ **Všechny herní moduly pokryty** - UI, gameplay, předměty, budovy, questy, atd.
- ✅ **Plně hratelné** v češtině
- ⚠️ **Současné omezení** - čeština se nezobrazuje v herním menu (vyžaduje implementaci vývojáři)

### Současná implementace
Vzhledem k tomu, že hra zatím nemá vestavěnou modding podporu pro jazyky, používáme obejití:
- Nahrazení anglických `_en.xml` souborů českými překlady
- Hra běží plně v češtině, ale v menu jazyků zobrazuje "English"

### Obsah repozitáře
- **38 XML překladových souborů** organizovaných podle herních modulů
- **FinishedTranslations.csv** - kompletní překladová databáze
- **Návod k instalaci** pro testování

### Pro vývojáře
Spolupracujeme s vývojářským týmem na implementaci modding podpory pro jazyky. Tento repozitář poskytuje:
- Kompletní česká lokalizační data
- Analýzu současné struktury souborů
- Návrhy implementace

### Kontakt
- Překladatel: Michal (LordMisak)
- Pro otázky ohledně implementace nebo detailů překladu prosím vytvořte issue

---

## File Structure / Struktura souborů

```
translations/
├── Achievements/          # Achievements system
├── Agents/               # AI agents
├── Analytics/            # Game analytics
├── Blueprints/           # Building blueprints
├── BugReport/            # Bug reporting system
├── Buildings/            # Buildings and structures
├── Debug/                # Debug interface
├── Decorations/          # Decorative items
├── DetailViews/          # Detailed item views
├── GameHud/              # Game HUD elements
├── GameSeedMenu/         # World generation menu
├── GifRecorder/          # Recording system
├── Global/               # Global game texts
├── Hints/                # Game hints and tips
├── Items/                # Items and equipment
│   └── Combat/           # Combat items
├── LoadingScreen/        # Loading screen texts
├── MainMenu/             # Main menu and credits
├── ModelViewer/          # 3D model viewer
├── PauseMenu/            # Pause menu
├── Prototypes/           # Prototype definitions
├── Quests/               # Quests and events
├── Recipes/              # Crafting recipes
├── SaveLoadMenu/         # Save/Load interface
├── SettingsMenu/         # Settings and languages
├── Ships/                # Ships and vehicles
├── Toasts/               # Notification toasts
├── Trading/              # Trading system
├── Units/                # Game units and characters
├── WorldResources/       # World resources
│   └── Trees/            # Tree resources
├── WorldSettings/        # World generation settings
└── FinishedTranslations.csv  # Translation database
```

## License
This translation is provided for community use. Original game content belongs to the Dawn Apart developers.