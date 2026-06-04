# EURL EL-AMIN EXPORT - Safety Equipment Catalog Guide
## Image Numbering System (Starting from 350)

---

## 📁 IMAGE NUMBERING MAP

### SAFETY HELMETS (350-355) → 6 images for 10 products
| Number | File Name | Product Description |
|--------|-----------|---------------------|
| 350 | 350.jpg | Casque Industriel Blanc EN 397 |
| 351 | 351.jpg | Casque Ventilé Vert Delta Plus |
| 352 | 352.jpg | Casque Ventilé Orange |
| 353 | 353.jpg | Casque à Cliquet Bleu |
| 354 | 354.jpg | Casque ANSI Type I Rouge |
| 355 | 355.jpg | Casque CE Approuvé Jaune |

**Products using these images:**
- sh1 (350), sh2 (351), sh3 (352), sh4 (353), sh5 (354), sh6 (355)
- sh7 (350), sh8 (351), sh9 (352), sh10 (353)

---

### SAFETY VESTS (360-364) → 5 images for 10 products
| Number | File Name | Product Description |
|--------|-----------|---------------------|
| 360 | 360.jpg | Gilet HV Orange EN 20471 |
| 361 | 361.jpg | Gilet Exécutif Warsaw Noir/Jaune |
| 362 | 362.jpg | Gilet Signalisation Orange |
| 363 | 363.jpg | Gilet Hiver Matelassé Orange |
| 364 | 364.jpg | Gilet Travail Rembourré |

**Products using these images:**
- sv1 (360), sv2 (361), sv3 (362), sv4 (363), sv5 (364)
- sv6 (360), sv7 (361), sv8 (362), sv9 (363), sv10 (364)

---

### SAFETY GLOVES (370-376) → 7 images for 10 products
| Number | File Name | Product Description |
|--------|-----------|---------------------|
| 370 | 370.jpg | Gants Coton Tricoté Blanc 600g |
| 371 | 371.jpg | Gants Cuir NITRAS Premium |
| 372 | 372.jpg | Gants Soudure COVAL 42VB |
| 373 | 373.jpg | Gants Cuir NITRAS Renforcé |
| 374 | 374.jpg | Gants Anti-Coupure HPPE Niveau 5 |
| 375 | 375.jpg | Gants Chimie Nitrile PIP |
| 376 | 376.jpg | Gants Soudure Portwest A530 |

**Products using these images:**
- sg1 (371), sg2 (372), sg3 (373), sg4 (374), sg5 (375), sg6 (376), sg7 (370)
- sg8 (371), sg9 (372), sg10 (370)

---

### WORKWEAR / COVERALLS (380-385) → 6 images for 10 products
| Number | File Name | Product Description |
|--------|-----------|---------------------|
| 380 | 380.jpg | Combinaison Ventilée Construction |
| 381 | 381.jpg | Combinaison Ignifugée Pompier Rouge |
| 382 | 382.jpg | Combinaison Wearpack Orange |
| 383 | 383.jpg | Combinaison Coton KNP 60g |
| 384 | 384.jpg | Combinaison Mécanicien Multi-Poches |
| 385 | 385.jpg | Combinaison Deluxe FR 7oz |

**Products using these images:**
- sc1 (380), sc2 (381), sc3 (382), sc4 (383), sc5 (384), sc6 (385)
- sc7 (380), sc8 (381), sc9 (382), sc10 (383)

---

### SAFETY BOOTS (390-395) → 6 images for 10 products
| Number | File Name | Product Description |
|--------|-----------|---------------------|
| 390 | 390.jpg | Chaussures S4 Blanches Agro |
| 391 | 391.jpg | Bottes Ferme Néoprène Vertes |
| 392 | 392.jpg | Chaussures S3 ESPRO Evolve |
| 393 | 393.jpg | Chaussures Agriculture Vertes |
| 394 | 394.jpg | Chaussures Agroalimentaire Blanches |
| 395 | 395.jpg | Chaussures S3 Cuir Marron |

**Products using these images:**
- sb1 (390), sb2 (391), sb3 (392), sb4 (393), sb5 (394), sb6 (395)
- sb7 (390), sb8 (391), sb9 (392), sb10 (393)

---

## 🔧 HOW TO EDIT WHEN ADDING YOUR OWN PHOTOS

### Option 1: Replace existing images (same numbers)
Simply overwrite the files in your `images/` folder:
```
images/
  350.jpg  → Your helmet photo
  351.jpg  → Your helmet photo
  ...
  395.jpg  → Your boots photo
```

### Option 2: Add new images (continue numbering from 396)
If you want to add MORE products, continue from 396:
```
396.jpg  → New helmet variant
397.jpg  → New vest variant
...
```

Then update the JavaScript code to reference the new numbers.

### Option 3: Change image assignments
In the JavaScript code, find the product and change the image path:

```javascript
// Before:
{ id: 'sh1', name: 'Casque...', image: './images/350.jpg', ... }

// After (using your own photo):
{ id: 'sh1', name: 'Casque...', image: './images/350.jpg', ... }
// Just overwrite 350.jpg with your photo!
```

---

## 📂 FOLDER STRUCTURE

```
/your-website/
├── index.html
└── images/
    ├── 350.jpg  to  355.jpg   (Helmets)
    ├── 360.jpg  to  364.jpg   (Vests)
    ├── 370.jpg  to  376.jpg   (Gloves)
    ├── 380.jpg  to  385.jpg   (Workwear)
    ├── 390.jpg  to  395.jpg   (Boots)
    └── ...other category images...
```

---

## ✅ QUICK REFERENCE TABLE

| Category | Numbers | Count | Products |
|----------|---------|-------|----------|
| Helmets | 350-355 | 6 | 10 |
| Vests | 360-364 | 5 | 10 |
| Gloves | 370-376 | 7 | 10 |
| Workwear | 380-385 | 6 | 10 |
| Boots | 390-395 | 6 | 10 |
| **TOTAL** | **350-395** | **30** | **50** |

---

## 📝 NOTE FOR PROGRAMMING

When you want to add your own photos:
1. **Rename** your photos to match the numbers (350.jpg, 351.jpg, etc.)
2. **Replace** the existing files in the images folder
3. **Or** edit the JavaScript to point to new numbers (396.jpg, 397.jpg, etc.)
4. **No need to change code** if you just overwrite existing numbered files!

The code uses: `image: './images/350.jpg'`
Just make sure your photo is named `350.jpg` in the images folder.
