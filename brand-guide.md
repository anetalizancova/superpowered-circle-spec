# SUPERPOWERED Circle — Brand Guide

## Fonty

| Použití | Font | Fallback |
|---------|------|----------|
| Headlines / Display | Hedvig Letters Serif | Georgia, serif |
| Body / UI | Geist (Inter jako fallback) | system-ui, sans-serif |

## Barvy

### Primární paleta

| Název | HEX | Použití |
|-------|-----|---------|
| Violet | `#C0ADFF` | Primární accent, gradient základ |
| Violet Deep | `#8B5CF6` | Headline gradient, tagy |
| Blue | `#1C58FF` | Sekundární accent, CTA |
| Pink | `#FF5AFF` | Terciární, event akcenty |
| Orange | `#FF9414` | Doplňková, výjimečně |

### Neutrální

| Název | HEX | Použití |
|-------|-----|---------|
| Ink (text) | `#000000` | Hlavní text, headlines |
| Subtle | `#696969` | Sekundární text |
| Muted | `#94a3b8` | Popisky, meta |
| Soft BG | `#F2F5FF` | Pozadí, karty |
| Paper | `#FFFFFF` | Hlavní pozadí |

### Tmavá varianta

| Název | HEX | Použití |
|-------|-----|---------|
| Deep BG | `#060b18` | Tmavé pozadí |
| Deep Surface | `#0f172a` | Karty, sidebar |
| Deep Muted | `#1e293b` | Okraje, linie |
| Deep Text | `#f8fafc` | Text na tmavém |
| Deep Subtle | `#64748b` | Sekundární text tmavý |

## Vizuální směry

### 1. Aibility Core (Violet dominanta)

**Kdy:** Komunita, Hledám/Nabízím, obecné covery

- Světlý podklad `#F2F5FF`
- Gradient flow violet → blue, jemný přechod
- Žádné tvrdé tvary, žádné blob kolečka
- Hedvig Serif titulky, gradient clip text

**CSS příklad:**
```css
background: linear-gradient(135deg, #F2F5FF 0%, #e8e0ff 25%, #d4c8ff 40%, #b8c8ff 60%, #F2F5FF 80%);
```

**Světlá varianta:** Violet/blue flow na `#F2F5FF`
**Tmavá varianta:** Blue/violet ambientní glow na `#060b18`

### 2. Deep (Blue dominanta)

**Kdy:** Edu Stream dark, SP profily, noční covery

- Tmavý podklad `#060b18` → `#1a1050`
- Ambientní gradient blue → violet zespoda
- Jemný glow efekt, ne ostrý

**CSS příklad:**
```css
background: linear-gradient(170deg, #060b18 0%, #0d1540 30%, #18124a 50%, #0a1a3a 70%, #060b18 100%);
```

**Vždy tmavá.** Kombinovatelná se světlou Core variantou.

### 3. Bridge (Levandule + pink)

**Kdy:** Prostory kde grafika nemá křičet, jemné pozadí

- Levandule přechází do blankytné
- Minimum kontrastu
- Textové hlavičky, žádné fotky

**CSS příklad:**
```css
background: linear-gradient(155deg, #F2F5FF 0%, #ece7ff 30%, #e0d6ff 55%, #d5e3ff 75%, #F2F5FF 100%);
```

**Světlá varianta:** Levandule/blankytná
**Tmavá varianta:** Použít Deep směr místo toho

## Dominantní barvy podle sekce

| Prostor | Dominanta | Směr |
|---------|-----------|------|
| Komunita | Violet (`#C0ADFF` → `#8B5CF6`) | Aibility Core |
| AI Edu Stream | Blue (`#1C58FF` → `#4f46e5`) | Core / Deep |
| Events | Střídá se (blue / violet / pink dle akce) | Fotka + overlay |
| Hledám / Nabízím | Blue shift (`#1C58FF` → `#3b82f6`) | Aibility Core |
| SP / Inner Circle | Deep dark (`#060b18`) | Deep |

## Pravidla

1. **Gradient flow, ne blob kolečka** — přechody jsou vždy plynulé, organické
2. **Každá sekce jiná dominanta** — ale všechno z jedné palety
3. **Vždy kombinovatelné** — světlá + tmavá varianta musí fungovat vedle sebe
4. **Fotky u Events** — živé fotky z akcí + gradient overlay, barva rotuje
5. **Fonty konzistentní** — Hedvig Serif pro titulky, Geist/Inter pro body
6. **Covery se dělají interně** — žádný externí grafik

## Pro AI generování

Při generování vizuálů pro Circle používej:

- **Světlé pozadí:** `#F2F5FF` s jemným violet/blue gradient flow
- **Tmavé pozadí:** `#060b18` s ambientním blue/violet glow
- **Font titulků:** Hedvig Letters Serif, elegantní, tenký
- **Font textu:** Geist nebo Inter, čistý, moderní
- **Styl:** Clean, tech-lifestyle, moderní SaaS estetika
- **Vyhýbej se:** Blob kolečka, ostrým přechodům, přesyceným barvám, stock foto estetice
- **Preferuj:** Plynulé gradient flow, jemné přechody, vzdušnost, whitespace
