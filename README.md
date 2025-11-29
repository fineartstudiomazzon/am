# Antonio Mancini Website

A static HTML website dedicated to Antonio Mancini (1852-1930), Italian Verismo painter and technical innovator.

## Website Structure

```
website/
├── index.html           # Home page with introduction and overview
├── biography.html       # Detailed chronological biography
├── works.html          # Gallery of major works in museums
├── technique.html      # Technical innovations (graticola, materials)
├── bibliography.html   # Scholarly resources and research
├── README.md           # This file
├── css/
│   └── style.css       # Main stylesheet
├── images/            # Artwork images and photos
│   └── front_portrait.png
└── js/                # JavaScript (for future enhancements)
```

## Pages Overview

### 1. Home (index.html)
- Introduction to Mancini's life and significance
- Key achievements timeline
- Artistic significance overview
- Entry point for visitors

### 2. Biography (biography.html)
- Comprehensive chronological life story
- Birth through death (1852-1930)
- Organized by life periods with timeline styling
- Personal character and relationships

### 3. Works (works.html)
- Gallery of major works in museum collections
- Organized chronologically
- Museum locations and provenance
- Currently text-based (ready for image additions)

### 4. Technique (technique.html)
- The graticola (grid) method explained
- Impasto technique evolution
- Material experimentation (embedded objects)
- Relationship to artistic movements

### 5. Bibliography (bibliography.html)
- Comprehensive scholarly resources
- Organized by type (monographs, catalogs, articles)
- Digital resources and archives
- Research gaps and opportunities

## Content Sources

All content compiled from verified sources in:
- `../MASTER_CONTENT.md` - Consolidated verified facts
- `../VERIFICATION_NEEDED.md` - Conflicts requiring resolution
- `../antoniomancini-site.pdf` - Original research materials
- `../research_1.txt` and `../research_2.txt` - Background research

## Design Features

### Current Implementation
- Clean, academic design
- Responsive layout (mobile-friendly)
- Sticky navigation header
- Timeline styling for biography
- Grid layout for gallery (ready for images)
- Professional color scheme (dark blue, brown, gold accents)

### Typography
- Georgia serif font for readability
- Clear hierarchy with styled headings
- Justified text for scholarly appearance

### Color Palette
```css
Primary: #2c3e50 (dark blue-gray)
Secondary: #8b4513 (saddle brown)
Accent: #c9a063 (gold)
Background: #fff (white)
Light Gray: #f4f4f4 (for sections)
```

## How to View Locally

### Option 1: Direct File Opening
1. Navigate to `/home/q/Documents/ART/web_material/mancini/website/`
2. Double-click `index.html`
3. Opens in your default web browser

### Option 2: Local Server (Recommended)
```bash
cd /home/q/Documents/ART/web_material/mancini/website
python3 -m http.server 8000
```
Then visit: http://localhost:8000

### Option 3: VS Code Live Server
1. Open website folder in VS Code
2. Install "Live Server" extension
3. Right-click `index.html` → "Open with Live Server"

## Next Steps

### Phase 1: Add Images ✓ Ready
The Works page is structured to receive artwork images from the PDF:
1. Extract images from `../antoniomancini-site.pdf`
2. Save as JPG/PNG in `images/` directory
3. Update `<img>` tags in works.html
4. Recommended naming: `work-title-year.jpg`

Example:
```html
<div class="artwork-card">
    <img src="images/saltimbanco-1879.jpg" alt="Il Saltimbanco, 1879">
    <div class="artwork-info">
        ...
    </div>
</div>
```

### Phase 2: Resolve Content Conflicts
Before final publication, address conflicts in `../VERIFICATION_NEEDED.md`:
- Asylum dates (1879 vs 1881)
- Brother Giovanni existence
- "After the Duel" location
- Il Saltimbanco date variations
- Obtain Virno 2019 Catalogue Raisonné

### Phase 3: Domain Deployment
When ready to publish:
1. Choose hosting (GitHub Pages, Netlify, traditional web hosting)
2. Update absolute URLs if needed
3. Add domain name to hosting service
4. Consider adding:
   - Contact form
   - Search functionality
   - Image galleries with lightbox
   - Social media integration

### Phase 4: Dynamic Enhancements (Future)
Potential additions:
- JavaScript image gallery/lightbox
- Search functionality
- Interactive timeline
- Commenting system for scholars
- Newsletter signup
- Multi-language support (Italian translation)

## Content Quality Notes

### ✓ Verified Content (Safe to Publish)
- Birth/death dates and locations
- Parents' names and professions
- Naples Academy admission (age 12)
- Major teachers (Morelli, Palizzi, Lista)
- Friendship with Gemito and Sargent
- Mesdag contract and collection
- Technical innovations (graticola, materials)
- Major museum holdings

### ⚠️ Needs Verification Before Final Publication
- Exact asylum dates (chronological conflict)
- Sibling information (contradictory sources)
- Some artwork locations
- Paris trip timeline details
- Late period political involvement

See `../VERIFICATION_NEEDED.md` for complete list.

## File Maintenance

### To Update Content
1. Edit HTML files directly
2. Use `MASTER_CONTENT.md` as authoritative source
3. Maintain consistent formatting and style
4. Update footer copyright year if needed

### To Modify Design
1. Edit `css/style.css`
2. Test on multiple screen sizes
3. Check mobile responsiveness
4. Verify browser compatibility

## Browser Compatibility

Tested and compatible with:
- Chrome/Chromium (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

Uses standard HTML5/CSS3, no special requirements.

## License

Content compiled from scholarly sources and public domain materials.
Check individual image copyrights before commercial use.

## Contact / Attribution

Website developed: 2025
Based on research materials compiled in `/home/q/Documents/ART/web_material/mancini/`

---

**Status:** Static site ready for local viewing and testing. Image integration and conflict resolution recommended before public deployment.
