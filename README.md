# Downloader4etesty2 CLI

Neoficiální nástroj příkazové řádky pro stahování testových otázek z portálu etesty2.mdcr.cz

## Popis

Tento nástroj umožňuje stahovat testové otázky z oficiálního portálu etesty2.mdcr.cz a ukládat je do lokálních souborů ve formátu JSON. Podporuje také stahování přiložených médií (obrázků a videí).

## Funkce

- 📋 Interaktivní výběr témat pro stažení
- 💾 Export dat do formátu JSON
- 🖼️ Volitelné stahování médií (obrázky, videa)
- 📁 Konfigurovatelný výstupní adresář

## Instalace

### Sestavení ze zdrojového kódu

```bash
git clone https://github.com/ahi6/autoskola_testy_workspace
cd autoskola_testy_workspace/downloader4etesty2_cli
cargo build --release
```

## Použití

Spusťte nástroj pomocí:

```bash
cargo run
```

nebo po instalaci:

```bash
downloader4etesty2_cli
```

### Průběh použití

1. **Výběr témat**: Zobrazí se seznam dostupných témat, ze kterých můžete vybrat více položek pomocí mezerníku
2. **Výstupní adresář**: Zadejte cestu, kam se mají uložit stažené soubory (výchozí: `./output`)
3. **Stahování médií**: Rozhodněte, zda chcete stáhnout také přiložená média (obrázky a videa)
4. **Stahování**: Nástroj automaticky stáhne vybraná témata a uloží je jako JSON soubory

### Výstupní formát

Každé téma se uloží jako samostatný JSON soubor obsahující:
- Kód otázky
- Text otázky
- Možné odpovědi (text nebo odkazy na obrázky)
- Označení správné odpovědi
- Odkazy na média (obrázky, videa)

## ⚠️ Upozornění

**DŮLEŽITÉ**: Tento projekt je určen pouze pro osobní a vzdělávací účely. Respektujte prosím podmínky používání oficiálního webu etesty2.mdcr.cz.

**Tento projekt je neoficiální a není spojen s Ministerstvem dopravy ČR.**

## Licence

Tento projekt je licencován pod EUPL v1.2 licencí - viz soubory `LICENSE` (v češtině) a `LICENSE_en` (v angličtině) pro podrobnosti.

## Struktura projektu

```
downloader4etesty2_cli/
├── src/
│   └── main.rs          # Hlavní aplikace
├── Cargo.toml           # Konfigurace projektu
├── LICENSE              # Licence v češtině
├── LICENSE_en           # Licence v angličtině
└── README.md            # Tento soubor
```