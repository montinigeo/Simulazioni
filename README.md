# Simulazioni Interattive

Raccolta di simulazioni didattiche interattive realizzate in HTML/JavaScript, senza dipendenze esterne. Ogni file è autonomo e funziona direttamente nel browser.

---

## 🌀 Moto Armonico Periodico

**File:** `moto_armonico.html`

Simulazione interattiva del moto armonico periodico, con rappresentazione simultanea del piano fasoriale e dell'andamento temporale.

### Contenuto

Il moto armonico è descritto dall'equazione:

```
x(t) = A · cos(ωt + φ₀)
```

La simulazione mostra la connessione tra il **moto circolare uniforme** (piano fasoriale) e il **moto armonico** (proiezione sull'asse reale), permettendo di visualizzare le tre grandezze cinematiche normalizzate:

- **Spostamento** x(t) = cos(ωt + φ₀)
- **Velocità** v(t) = −sin(ωt + φ₀)
- **Accelerazione** a(t) = −cos(ωt + φ₀)

### Funzionalità

- Regolazione interattiva di **frequenza** (0.2–4 Hz), **ampiezza** e **fase iniziale** tramite slider
- Selezione del parametro da visualizzare nel grafico temporale (spostamento, velocità, accelerazione) con radio button
- Fasore rotante che cambia direzione in base al parametro selezionato:
  - Posizione → radiale
  - Velocità → tangenziale (+90°)
  - Accelerazione → centripeta (verso il centro)
- Visualizzazione opzionale dei vettori sull'asse x del piano fasoriale
- Marcatori verticali nel grafico temporale al cambio di parametri
- Forma trigonometrica e fasoriale aggiornate in tempo reale
- Continuità della simulazione anche con la finestra in background
- Layout responsive (PC e mobile)

---

## ⚛️ Diffrattometro XRD

**File:** `diffrattometro_xrd_v5.html`

Simulazione interattiva di un diffrattometro a raggi X per polveri, basata sulla **legge di Bragg**:

```
nλ = 2d · sin(θ)
```

### Contenuto

La diffrazione a raggi X è una tecnica fondamentale per la determinazione della struttura cristallina dei minerali e dei materiali. Quando un fascio di raggi X colpisce un campione policristallino, i piani reticolari con spaziatura *d* soddisfano la condizione di Bragg per un angolo θ specifico, generando un picco di diffrazione a 2θ nel diffrattogramma.

### Materiali inclusi

| Materiale | Sistema cristallino | Gruppo |
|-----------|-------------------|--------|
| NaCl (alite) | Cubico — Fm3̄m | — |
| Si (silicio) | Cubico — Fd3̄m | — |
| Al (alluminio) | Cubico — Fm3̄m | — |
| Quarzo (SiO₂) | Trigonale — P3₁21 | Tettosilicato |
| TiO₂ (rutilo) | Tetragonale — P4₂/mnm | — |
| FeO (wüstite) | Cubico — Fm3̄m | — |
| Olivina Fo | Ortorombico — Pbnm | Nesosilicato |
| Epidoto | Monoclino — P2₁/m | Sorosilicato |
| Berillo | Esagonale — P6/mcc | Ciclosilicato |
| Diopside | Monoclino — C2/c | Inosilicato (pirosseno) |
| Muscovite | Monoclino — C2/c | Fillosilicato |
| Anortite | Triclino — P1̄ | Tettosilicato (feldspato) |

### Funzionalità

- **Schema ottico** con sorgente, campione e rivelatore in geometria reale
- Due geometrie selezionabili:
  - **Bragg-Brentano** (θ/2θ): campione rotante, sorgente fissa
  - **θ-θ**: campione fisso, sorgente e rivelatore si muovono simmetricamente
- Quattro sorgenti disponibili: Cu Kα, Mo Kα, Co Kα, Cr Kα (lunghezze d'onda reali)
- **Diffrattogramma** costruito in tempo reale durante la scansione automatica o manuale
- Tabella dei picchi attesi con indici di Miller (hkl), spaziatura d e intensità relativa I/I₀
- Identificazione automatica dei picchi con etichette hkl
- Campione rappresentato come rettangolo rotante (BB) o fisso (θ-θ) con piani reticolari visibili
- Angoli θ e 2θ visualizzati come archi crescenti sul goniometro
- Layout responsive (PC: schema e diffrattogramma affiancati; mobile: verticale)

---

## Autore

Simulazioni sviluppate con l'assistenza di Claude (Anthropic).

## Licenza

Libero uso per scopi didattici e divulgativi.
