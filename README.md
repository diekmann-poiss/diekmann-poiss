# Website2.1 - Diekmann & Poiss

**Version:** 2.1 (Updated with language switch and comprehensive translations)
**Last Updated:** 2026-10-07
**Project:** Building Greenery Software - Diekmann & Poiss

---

## 📁 File Structure

```
website/
├── README.md                    # This file
├── index.html                   # Original (Cocoa HTML Writer format)
├── Website2.1.html              # Clean, working version
├── images/                      # All images (referenced with images/ prefix)
│   ├── Schwarzau1.JPG
│   ├── Schwarzau4.jpg
│   ├── LoniceraHeck.JPG
│   ├── IrrigationTech.PNG
│   ├── ProfileFridi.jpg
│   ├── ProfileMax.jpg
│   ├── Plants.JPG
│   ├── Soil.jpeg
│   ├── Maintenence.JPG
│   ├── Wisteria4.JPG
│   └── ... (25 images total)
```

---

## ✅ What Has Been Done

### 1. **Clean HTML Extraction**
- Extracted clean HTML from Cocoa HTML Writer wrapper
- Removed `<p class="p1">` wrapper tags
- Unescaped HTML entities
- Valid HTML5 structure

### 2. **Image Paths Fixed**
- All image references updated to use `images/` prefix
- Fixed case sensitivity (Schwarzau4.JPG → Schwarzau4.jpg)
- Replaced missing images with available alternatives:
  - TeamPhoto.jpg → Schwarzau5.JPG
  - AquaCalc1-3.PNG → Plants.JPG, Soil.jpeg, IrrigationTech.PNG
  - Greensight.PNG → IrrigationTech.PNG

### 3. **Service Areas (5 Areas of Expertise)**
- **Structure** - Climbing Aid & Building integration
- **Soil & Substrate** - Growing Medium & Nutrient Systems
- **Plants** - Botanical Expertise & Species Selection
- **Irrigation Technology** - Water Management & Automation
- **Maintenance** → Changed to **Pflege** (German)
- All have placeholder text in detail sections
- Narrowed layout (padding: 3rem 2rem, gap: 2rem)
- Images max-width: 550px

### 4. **Language Switch Feature** 🌐
- Added EN/DE button to navigation
- Comprehensive translation object with:
  - English (en) translations
  - German (de) translations
- `switchLanguage()` function toggles between languages
- Covers ALL sections:
  - Navigation
  - Hero & Intro
  - Services (Areas of Expertise)
  - Chain Diagram (all 5 items)
  - Service Details (titles & taglines)
  - Contact Section
  - Team (names, skills, LinkedIn)
  - Footer
  - **Why Us** section (all text except paper titles)
  - **Software** section (tools, descriptions)
- **Paper titles NOT translated** (as requested)

### 5. **Specific Text Updates**
- "Maintenance" → "Pflege" in German
- AquaCalc link: https://diekmann-poiss.github.io/Aquacalc/
- CoverScope link (formerly GreenSight): https://diekmann-poiss.github.io/coverscope/
- GreenSight renamed to CoverScope

---

## 📝 Current Status

### Website2.1.html Features:
- ✅ Responsive design (mobile-friendly)
- ✅ Modern CSS with variables
- ✅ Google Fonts (Playfair Display, DM Sans)
- ✅ Smooth scrolling
- ✅ Parallax hero background
- ✅ Interactive chain diagram
- ✅ Reveal animations
- ✅ Multi-page structure (Home, Why Us, Software)
- ✅ **Working language switch (EN/DE)**
- ✅ All images load from images/ folder
- ✅ Valid HTML5

### Placeholder Text Still Present:
The 5 service detail sections still contain placeholder text:
```
[Placeholder text: Comprehensive structural planning...]
```
**These need to be replaced with actual descriptions.**

---

## 🎯 What Still Needs to Be Done

### High Priority:
1. **Replace placeholder text** in service detail sections (5 sections)
   - Structure / Struktur
   - Soil & Substrate / Boden & Substrat
   - Plants / Pflanzen
   - Irrigation Technology / Bewässerungstechnik
   - Maintenance / Pflege

### Medium Priority:
2. Add translations for placeholder text in German
3. Add favicon
4. Optimize images for web (compress, proper formats)

### Low Priority:
5. Add SEO meta tags
6. Add alt text for all images
7. Test on various browsers
8. Add loading animations

---

## 🚀 How to Test

```bash
# Navigate to folder
cd /Users/admin/Desktop/DIV/D-P/website

# Start local web server (required for Google Fonts & JS)
python3 -m http.server 8000

# Open in browser
# http://localhost:8000/Website2.1.html
```

**Important:** Opening the file directly (file://) will NOT work properly:
- ❌ Google Fonts won't load (CORS restriction)
- ❌ Some JavaScript may not execute
- ✅ Use local web server for full functionality

---

## 🔧 Technical Notes

### JavaScript Functions:
- `showPage(pageId)` - Switches between pages (Home, Why Us, Software)
- `switchLanguage()` - Toggles between English and German
- `observeReveals()` - Handles scroll reveal animations
- `scrollToSection(sectionId)` - Smooth scroll to service sections

### CSS Features:
- CSS Variables: --off-white, --dark, --mid, --muted, --accent, --border
- Responsive: @media (max-width: 768px)
- Animations: reveal, scrollpulse
- Blend modes: mix-blend-mode: difference (on nav)

### Known Issues:
- None currently identified
- Language switch preserves HTML structure (br, em tags)

---

## 📞 Contact Information in Website

**Email:** diekmann-poiss@proton.me
**Location:** Vienna, Austria / Wien, Österreich
**Team:**
- Fridtjof Diekmann (Technical implementation, project coordination, soil & substrate)
- Max Poiss (Thermal comfort, vegetation technology, automatisation)

---

## 💡 For Next Session

**To pick up where we left off:**
1. Read this README.md file
2. Open Website2.1.html in a text editor
3. Check the placeholder text in service detail sections
4. The language switch is fully functional
5. All German translations are complete (except placeholder text)

**Quick Commands:**
```bash
# Start server
python3 -m http.server 8000

# Check file structure
ls -la

# Check images
ls images/
```

---

**Last Modified:** 2026-10-07
**Status:** Ready for content population (placeholder text replacement)
