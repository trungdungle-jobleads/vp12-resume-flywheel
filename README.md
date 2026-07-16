# Resume Flywheel — Storyboard (website)

Interaktive Storyboard-Sketch-Ansicht für den JobLeads Brand-/Produktfilm **„Resume Flywheel"**
(Scene 1–6, 32 Shots). Diese Seite wird über GitHub Pages ausgeliefert.

**➡️ Ansehen:** die Root-URL der Pages-Seite dieses Repos.

Dieses Repo enthält **nur die Website-Dateien**. Die Arbeitsunterlagen (Storyboard-Doku,
Sketch-Prompts, Master-Resume, Original-Screenshots) liegen bewusst nicht hier, sondern lokal
im Projektordner.

## Inhalt

| Pfad | Inhalt |
|---|---|
| `index.html` | Die Seite selbst: Card-Grid Scene·Shot + Timecode → VO/Kamera/Spec → 16:9-Sketch, mit Bild-Umschalter pro Shot, neutrale Graustufen, Light/Dark. |
| `storyboard-sketches/` | Die 32 Sketch-PNGs (`s<scene>_sh<shot>.png`) plus Alternativ-Versionen (`_v2`, `_v3` …). |
| `storyboard-sketches.html` | Weiterleitung auf `index.html` (alte URL bleibt gültig). |
| `.nojekyll` | Statische Seite, kein Jekyll-Build. |

## Bild-Varianten pro Shot

Ein Shot kann mehrere Versionen haben. Sobald neben `s3_sh1.png` auch `s3_sh1_v2.png` liegt,
zeigt die Seite unten rechts im Bild einen Umschalter `‹ 1/2 ›`. Neue Variante = Datei nach dem
Schema `_v2`, `_v3` … in `storyboard-sketches/` ablegen, committen. Kein Code-Eingriff nötig,
`index.html` findet sie beim Laden selbst. Die Auswahl merkt sich der Browser lokal pro Shot.

Gewinnt eine Variante endgültig: über die `.png` ohne Suffix kopieren (`cp s3_sh1_v2.png s3_sh1.png`),
die `_vN` löschen, committen. Dann verschwindet der Umschalter wieder.
