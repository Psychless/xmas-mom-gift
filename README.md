# Ziemassvētku Dāvana - Lauku Atpūtas Vouchers

Vienkārša un eleganta vienas lapas tīmekļa vietne, kas izveidota kā digitāls Ziemassvētku dāvanas vouchers.

## Failu struktūra

- `index.html` - Galvenā HTML struktūra ar vouchers saturu (latviešu valodā)
- `styles.css` - Elegants dizains ar siltām krāsām un responsīvu izkārtojumu
- `README.md` - Šis fails

## GitHub Pages izvietošana

### 1. solis: Izveido GitHub repozitoriju

1. Ej uz [GitHub.com](https://github.com) un piesakies savā kontā
2. Noklikšķini uz "+" ikonas augšējā labajā stūrī un izvēlies "New repository"
3. Ieraksti repozitorija nosaukumu (piemēram, `mom-xmas-gift`)
4. Izvēlies "Public" (GitHub Pages darbojas arī ar privātiem repozitorijiem, bet publisks ir vienkāršāk)
5. Neklikšķini uz "Initialize this repository with a README" (jo mums jau ir faili)
6. Noklikšķini "Create repository"

### 2. solis: Augšupielādē failus

**Opcija A: Izmantojot GitHub tīmekļa saskarni**

1. Pēc repozitorija izveides, noklikšķini uz "uploading an existing file"
2. Velc un nomet `index.html`, `styles.css` un `README.md` failus
3. Noklikšķini "Commit changes"

**Opcija B: Izmantojot Git komandrindu**

```bash
# Inicializē Git repozitoriju (ja vēl nav izveidots)
git init

# Pievieno failus
git add index.html styles.css README.md

# Izveido commit
git commit -m "Initial commit - voucher website"

# Pievieno GitHub remote (aizstāj ar savu repozitorija URL)
git remote add origin https://github.com/TU-VARDS/mom-xmas-gift.git

# Augšupielādē failus
git branch -M main
git push -u origin main
```

### 3. solis: Iespējo GitHub Pages

1. Ej uz savu repozitoriju GitHub
2. Noklikšķini uz "Settings" (iestatījumi) repozitorija augšpusē
3. Skritlē uz leju līdz "Pages" sadaļai kreisajā sānjoslā
4. Zem "Source" izvēlies "Deploy from a branch"
5. Izvēlies "main" branch un "/ (root)" mapi
6. Noklikšķini "Save"

### 4. solis: Gaidi izvietošanu

- GitHub Pages parasti aktivizējas 1-2 minūšu laikā
- Tavs tīmekļa vietne būs pieejama: `https://TU-VARDS.github.io/mom-xmas-gift/`
- (Aizstāj `TU-VARDS` ar savu GitHub lietotājvārdu un `mom-xmas-gift` ar savu repozitorija nosaukumu)

## QR koda izveide

Kad tīmekļa vietne ir izvietota, var izveidot QR kodu, kas ved uz šo vietni:

1. Izmanto jebkuru bezmaksas QR koda ģeneratoru:
   - [QR Code Generator](https://www.qr-code-generator.com/)
   - [QRCode Monkey](https://www.qrcode-monkey.com/)
   - Vai jebkuru citu

2. Ievadi savu GitHub Pages URL (piemēram: `https://TU-VARDS.github.io/mom-xmas-gift/`)

3. Lejupielādē QR kodu un izdrukā vai saglabā kā attēlu

## Satura pielāgošana

### Teksta maiņa

Atver `index.html` un meklē šādas sadaļas, lai pielāgotu saturu:

- **Vouchers nosaukums**: Meklē `<h1 class="voucher-title">` un `<h2 class="voucher-subtitle">`
- **Apraksts**: Meklē `<div class="voucher-description">` sadaļu
- **Detalizēta informācija**: Meklē `<div class="voucher-details">` sadaļu
- **Izmantošanas instrukcijas**: Meklē `<div class="redemption-section">` sadaļu
- **Noteikumi**: Meklē `<div class="terms-section">` sadaļu
- **Paraksts**: Meklē `<div class="voucher-footer">` sadaļu

### Krāsu maiņa

Atver `styles.css` un meklē šādus krāsu kodus:

- **Zelta krāsa**: `#d4af37` (vouchers akcenti)
- **Brūna krāsa**: `#8b4513` (galvenie virsraksti)
- **Fona krāsa**: `#fffef8` (kartes fons)
- **Fona gradients**: `#f5e6d3`, `#e8d5c4`, `#d4c4b0` (lapas fons)

### Fontu maiņa

Meklē `font-family` īpašības `styles.css` failā. Pašlaik izmantoti:
- `'Georgia', 'Times New Roman', serif` - galvenajam tekstam
- `'Brush Script MT', cursive` - parakstam

## Tehniskās detaļas

- **Nav nepieciešamas atkarības** - tīra HTML/CSS
- **Responsīvs dizains** - darbojas uz mobilajām ierīcēm (ideāli QR koda skenēšanai)
- **Ātra ielāde** - minimāli faili, nav JavaScript frameworku
- **Drukāšanai piemērots** - var saglabāt kā PDF

## Atbalsts

Ja rodas problēmas ar izvietošanu vai pielāgošanu, pārbaudi:
- Vai visi faili ir augšupielādēti repozitorijā
- Vai GitHub Pages ir iespējots repozitorija iestatījumos
- Vai izmanto pareizo branch (parasti "main")

