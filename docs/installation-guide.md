# Installation Guide / Návod k instalaci

## English

### For Players - How to Use Czech Translation

#### Current Workaround Method
Since the game doesn't have built-in Czech language support yet, we use a replacement method:

1. **Backup original files** (recommended)
   ```
   Navigate to: [Game Installation Folder]\Data\StreamingAssets\Localization\
   Create backup of all *_en.xml files
   ```

2. **Install Czech translation**
   - Download all files from `/translations` folder
   - Replace corresponding `*_en.xml` files with `*_cs.xml` files
   - Rename `*_cs.xml` to `*_en.xml` during replacement

3. **Game will now run in Czech**
   - All texts, menus, and UI will be in Czech
   - Language menu will still show "English" (cosmetic issue)

### For Developers - Testing the Translation

#### File Structure Analysis
```
Data/StreamingAssets/Localization/
├── Achievements/achievements_en.xml
├── Agents/agents_en.xml
├── Analytics/analytics_en.xml
... (and 35 more XML files)
```

#### Key Files for Language Implementation
- `SettingsMenu/languages_cs.xml` - Contains language definitions
- `FinishedTranslations.csv` - Complete translation database
- All `*_cs.xml` files - Individual module translations

#### Integration Suggestions
1. **Add Czech to language list** in game settings
2. **Enable language switching** without file replacement
3. **Use existing translation data** - everything is ready

---

## Česky

### Pro hráče - Jak použít český překlad

#### Současné řešení (obejití)
Protože hra zatím nemá vestavěnou podporu češtiny, používáme metodu náhrady:

1. **Zálohujte původní soubory** (doporučeno)
   ```
   Přejděte na: [Složka hry]\Data\StreamingAssets\Localization\
   Vytvořte zálohu všech *_en.xml souborů
   ```

2. **Instalace českého překladu**
   - Stáhněte všechny soubory ze složky `/translations`
   - Nahraďte odpovídající `*_en.xml` soubory soubory `*_cs.xml`
   - Při náhradě přejmenujte `*_cs.xml` na `*_en.xml`

3. **Hra poběží v češtině**
   - Všechny texty, menu a rozhraní budou v češtině
   - V menu jazyků se stále zobrazí "English" (kosmetická chyba)

### Pro vývojáře - Testování překladu

#### Analýza struktury souborů
```
Data/StreamingAssets/Localization/
├── Achievements/achievements_en.xml
├── Agents/agents_en.xml
├── Analytics/analytics_en.xml
... (a dalších 35 XML souborů)
```

#### Klíčové soubory pro implementaci jazyka
- `SettingsMenu/languages_cs.xml` - Obsahuje definice jazyků
- `FinishedTranslations.csv` - Kompletní překladová databáze
- Všechny `*_cs.xml` soubory - Překlady jednotlivých modulů

#### Návrhy integrace
1. **Přidat češtinu do seznamu jazyků** v nastavení hry
2. **Umožnit přepínání jazyka** bez náhrady souborů
3. **Použít existující překladová data** - vše je připraveno

## Technical Notes

### File Encoding
All XML files use UTF-8 encoding with proper Czech diacritics support.

### Translation Completeness
- ✅ UI Elements: 100%
- ✅ Game Content: 100%
- ✅ Menus: 100%
- ✅ Tooltips: 100%
- ✅ Dialogues: 100%

### Known Issues
- Language menu shows "English" instead of "Čeština" (requires code modification)
- No dynamic language switching (requires game restart with file replacement)

### Future Implementation Recommendations
1. Add Czech language option to game settings
2. Implement dynamic language loading from `*_cs.xml` files
3. Update language selection UI to properly display "Čeština"