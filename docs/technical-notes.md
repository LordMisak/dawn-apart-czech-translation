# Technical Notes / Technické poznámky

## English

### Translation System Analysis

#### Current Game Language System
The game uses XML-based localization with the following structure:
- Language files: `*_en.xml`, `*_de.xml`, `*_fr.xml`, etc.
- Language definitions: `SettingsMenu/languages_cs.xml`
- Translation database: `FinishedTranslations.csv`

#### Czech Language Implementation Status
- ✅ **Complete translation data exists** - All 38 modules translated
- ✅ **Language definition ready** - Czech is defined as language #4
- ❌ **Missing UI integration** - Czech not accessible from settings menu

#### Root Cause Analysis
Investigation suggests the language selection is hardcoded in the game binary (`Assembly-CSharp.dll`), preventing Czech from appearing in the language menu despite having complete localization data.

### File Structure
```
Localization/
├── [Module]/[module]_en.xml     # English (default)
├── [Module]/[module]_de.xml     # German  
├── [Module]/[module]_fr.xml     # French
├── [Module]/[module]_cs.xml     # Czech (hidden)
└── FinishedTranslations.csv     # Translation database
```

### Current Workaround
Replace English XML files with Czech translations to bypass hardcoded language restrictions.

### Implementation Recommendations

#### Option 1: Extend Language Selection
- Add Czech to hardcoded language list
- Enable `*_cs.xml` file loading
- Update UI to show "Čeština" option

#### Option 2: Modding Support
- Create language mod loading system
- Allow community translations without core game modifications
- Support for additional languages beyond the base set

#### Option 3: Dynamic Language Loading
- Scan localization folder for available languages
- Auto-detect `*_cs.xml` patterns
- Generate language menu dynamically

---

## Česky

### Analýza překladového systému

#### Současný jazykový systém hry
Hra používá XML lokalizaci s následující strukturou:
- Jazykové soubory: `*_en.xml`, `*_de.xml`, `*_fr.xml`, atd.
- Definice jazyků: `SettingsMenu/languages_cs.xml`
- Překladová databáze: `FinishedTranslations.csv`

#### Stav implementace češtiny
- ✅ **Kompletní překladová data existují** - Všech 38 modulů přeloženo
- ✅ **Definice jazyka připravena** - čeština je definována jako jazyk #4
- ❌ **Chybí integrace do UI** - čeština není dostupná z menu nastavení

#### Analýza příčiny
Šetření naznačuje, že výběr jazyka je napevno zakódován v binárce hry (`Assembly-CSharp.dll`), což brání zobrazení češtiny v jazykovém menu navzdory kompletním lokalizačním datům.

### Struktura souborů
```
Localization/
├── [Modul]/[modul]_en.xml       # Angličtina (výchozí)
├── [Modul]/[modul]_de.xml       # Němčina
├── [Modul]/[modul]_fr.xml       # Francouzština
├── [Modul]/[modul]_cs.xml       # Čeština (skrytá)
└── FinishedTranslations.csv     # Překladová databáze
```

### Současné obejití
Nahrazení anglických XML souborů českými překlady pro obejití napevno zakódovaných jazykových omezení.

### Doporučení implementace

#### Možnost 1: Rozšířit výběr jazyka
- Přidat češtinu do napevno zakódovaného seznamu jazyků
- Povolit načítání `*_cs.xml` souborů
- Aktualizovat UI pro zobrazení možnosti "Čeština"

#### Možnost 2: Podpora moddingu
- Vytvořit systém načítání jazykových modů
- Umožnit komunitní překlady bez úprav základní hry
- Podpora dalších jazyků nad rámec základní sady

#### Možnost 3: Dynamické načítání jazyků
- Skenovat lokalizační složku pro dostupné jazyky
- Automaticky detekovat vzory `*_cs.xml`
- Generovat jazykové menu dynamicky

## Translation Quality Metrics

### Statistics
- **Total files:** 38 XML files + 1 CSV database
- **Translation coverage:** 100%
- **File size:** ~2.5 MB total
- **Encoding:** UTF-8 with Czech diacritics

### Quality Assurance
- All texts tested in-game context
- Consistent terminology across modules
- Proper Czech grammar and localization conventions
- Gaming terminology adapted for Czech players

### File Dependencies
```
FinishedTranslations.csv → All *_cs.xml files
languages_cs.xml → Language selection system
settings_menu_cs.xml → Settings interface
```

## Community Impact

### Benefits
- First complete Czech translation for Dawn Apart
- Professional quality suitable for official integration  
- Ready-to-use translation data
- Template for future community translations

### Usage Recommendations
- Suitable for immediate player use via workaround
- Production-ready for official game integration
- Reference implementation for modding system development