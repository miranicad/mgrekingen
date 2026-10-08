# Designsystem Musikgesellschaft Rekingen

Quelle: das Design-System-Artifact auf claude.ai. Änderungen dort machen und hierher übernehmen.

## Einbinden

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Cabin:wght@400;500;600&display=swap">
<link rel="stylesheet" href="design-system/tokens.css">
```

Dann Werte nur über Variablen verwenden, z. B. `color: var(--ink); background: var(--surface);`. Die Textstile gibt es als Klassen (`.display`, `.h1`, `.body`, `.label` …). Dunkles Theme: automatisch per Systemeinstellung oder mit `<html data-theme="dark">` erzwingen.

- `tokens.json`: alle Werte als Daten
- `tokens.css`: dieselben Werte als CSS-Variablen
- `assets/mg-rekingen-logo.png`: Logo, farbig, 1329 × 507 px

## Richtlinien

Das visuelle Erscheinungsbild der Musikgesellschaft Rekingen für Website, Plakate, Flyer und Konzertprogramme. Grundlage ist das Vereinslogo: ein blaues Oval mit gelbem Horn und Notenbogen, daneben die blaue Wortmarke.

## Logo

- Verwende immer die Originaldatei `assets/mg-rekingen-logo.png`. Logo nie nachzeichnen, umfärben, verzerren oder die Wortmarke neu setzen.
- Das Logo steht auf Weiss (`surface` im hellen Theme). Auf dunklem Grund oder auf `mg-blue` das Logo in eine weisse Fläche mit `radius-lg` und mindestens `space-4` Innenabstand setzen, bis eine Negativversion vorliegt.
- Rundherum Freiraum lassen; das Logo nie in Text oder Bilder laufen lassen.

## Farbe

- Zwei Markenfarben, beide exakt aus dem Logo: `mg-blue` (#298FCE) und `mg-yellow` (#F7DA00). Blau führt, Gelb akzentuiert. Faustregel: viel Weiss, deutlich Blau, wenig Gelb.
- Fliesstext in `ink` auf `surface` oder `surface-tint`. Nebentext in `ink-muted`.
- `mg-blue` als Textfarbe nur ab 24px (Titel). Für Links und kleineren blauen Text `blue-text`.
- `mg-yellow` nie als Textfarbe auf Weiss. Gelbe Flächen tragen Text in `on-yellow`.
- Buttons: Füllung `blue-text`, Schrift `on-blue`. Sekundär: Rahmen `ink-muted`, Schrift `ink`.
- Keine Verläufe, keine weiteren Akzentfarben.

## Schrift

- Eine Familie für alles: `sans` (Gill Sans, wie die Wortmarke; Fallback Cabin von Google Fonts, dann Trebuchet MS). Cabin auf Websites per Google Fonts laden.
- Titel in `display`, `h1`, `h2`, `h3`; Text in `body`, `small`; Daten und Kategorien in `label` (Grossbuchstaben).
- Titel eher leicht (Regular) wie die Wortmarke, nicht fett. Hierarchie über Grösse und Farbe.

## Abstände und Formen

- Abstände nur aus `space-1` bis `space-6`. Karten innen `space-4`, Abschnitte `space-5`.
- Ecken: `radius-md` für Buttons und Karten, `radius-lg` für grosse Flächen und Bilder. Die weiche, runde Form des Logo-Ovals darf sich in Flächen wiederholen.
- Trennlinien 1px in `border`. Keine Schatten.
- Fokus: 2px Ring in `focus-ring` mit 2px Abstand.
