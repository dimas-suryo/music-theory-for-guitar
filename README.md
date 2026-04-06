# Music Theory for Guitar — Complete Reference

Interactive mind map dan referensi komprehensif teori musik untuk gitaris, dari fisika suara hingga advanced harmony.

## Overview

Site ini adalah **single-page reference** yang menyajikan seluruh teori musik yang relevan untuk gitaris dalam format **interactive mind map**. Klik node di panel kiri untuk membuka materi di panel kanan. Setiap topik ditulis mendalam dengan tabel, diagram, dan key takeaway di akhir section.

## Struktur File

```
├── index.html    # Layout, konten, mind map (D3.js), note picker logic
└── styles.css    # Styling — Inter + JetBrains Mono, Shadcn UI palette
```

Tidak ada build step. Buka `index.html` di browser.

## Topik yang Dicakup

**15 topik utama, 3 sub-topik:**

| # | Topik | Cakupan |
|---|-------|---------|
| 1 | Sound & Acoustics | Gelombang, frekuensi, amplitude, timbre, harmonic series, overtone, consonance/dissonance |
| 2 | Notes & Tuning | 12-TET, A440 (ISO 16:1975), Pythagorean vs Just Intonation vs Equal Temperament, enharmonic equivalence, alternate tunings |
| 3 | Intervals | 13 interval + rasio Just, melodic vs harmonic, inversion, compound intervals, ear training reference songs |
| 4 | Scales | Major, Natural/Harmonic/Melodic Minor, Pentatonic, Blues, Whole Tone, Diminished, Bebop, Phrygian Dominant |
| 5 | Scale Mathematics | Tetrachord construction, circle of fifths derivation, kenapa 7 nada dan 12 semitone |
| 6 | Chord Construction | 4 triad, 5 jenis 7th chord, extensions (9/11/13), altered chords, sus chords, voicings & inversions |
| 7 | Diatonic Harmony | Roman numeral analysis, 3 fungsi harmoni, progresi populer, chord substitution |
| 8 | The 7 Modes | Parallel approach, bright↔dark spectrum, characteristic/avoid notes, chord-scale theory |
| 9 | Advanced Harmony | 4 cadences, secondary dominants, 4 jenis modulasi, tritone substitution, modal interchange |
| 10 | Rhythm & Meter | Time signatures, subdivisions, syncopation, swing vs straight, polyrhythm |
| 11 | Guitar Essentials | Anatomi, standard tuning rationale, essential skills checklist, intonation & setup |
| 12 | CAGED System | 5 shapes, root navigation, scale shape overlay |
| 13 | Fretboard Mapping | Natural notes per string, octave shapes, shortcuts, metode latihan |
| 14 | Lead Techniques | 7 teknik esensial, bend & vibrato deep dive, dynamics & articulation |
| 15 | Ear Training | 4 area latihan, relative vs absolute pitch, latihan harian |
| 16 | Practice & Mindset | Deliberate practice, struktur sesi, core exercises, plateau & breakthrough |

## Note Picker

Tool interaktif untuk latihan fretboard mapping:

- **Random note generator** dengan tempo adjustable (20–240 BPM)
- **Fretboard display** menunjukkan semua posisi nada aktif di 6 string × 16 fret
- **Multi-note mode** — 1 sampai 4 nada sekaligus
- **Presets** — Natural notes, C Pentatonic, All 12, Clear
- Setiap nada menampilkan **frekuensi Hz**

## Tech Stack

- **HTML/CSS/JS** vanilla — no framework, no build
- **D3.js v7** untuk mind map (zoom, pan, radial layout)
- **Inter** (body) + **JetBrains Mono** (code/labels) via Google Fonts
- **Shadcn UI** color palette (zinc scale, blue accent, emerald untuk picker)

## Cara Pakai

1. Buka `index.html` di browser
2. Klik node di mind map (panel kiri) untuk membuka materi
3. Scroll panel kanan untuk membaca
4. Klik node **Note Picker** (hijau) untuk tool latihan fretboard
5. Drag untuk pan, scroll untuk zoom di mind map

## Design Decisions

- **Bahasa Indonesia** — Target audience gitaris Indonesia
- **Dark mode only** — Mengurangi eye strain saat belajar lama
- **No framework** — Load instan, zero dependencies selain D3 dan Google Fonts
- **Key Takeaway** di setiap section — Ringkasan 2-3 kalimat untuk review cepat
- **Fretboard display** di Note Picker — Visualisasi langsung posisi nada, bukan sekadar nama nada

## License

Free to use and modify.
