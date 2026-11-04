# Vintage Cover Forge source collection

Ten editable graphic-design adaptations from the user-supplied `vintage-cover-forge.zip` are under **Books → Vintage Forge source collection**. Search **Vintage Forge** to find them quickly.

## Source and scope

- ZIP SHA-256: `ee372bfbab615efeb7dcca1626431df501c6f5fdf522b1604e5793ef78eeab05` (802,325 bytes; 49 catalogue entries).
- Original ZIP and the older standalone Vintage Cover Forge remain untouched.
- Adapted source: `components/BookCover.tsx` and `lib/types.ts`; native Art Dev layer construction lives in `src/generators/vintage-source.ts`.
- Ten source IDs: `ancient-papyrus`, `medieval-gospel`, `illuminated-manuscript`, `1920s-art-deco`, `1920s-bauhaus`, `1950s-atomic`, `1960s-pop-art`, `1970s-brutalist`, `1990s-grunge-zine`, `1900s-art-nouveau`.
- These are native, editable interpretations, not pixel-identical screenshots or historical replicas. Remaining 39 ZIP entries were not promoted into the visible catalogue.
- Sample titles, authors and publishers are fictional replacements. Source Nancy Drew sample content, Gemini integration and Next.js infrastructure were not imported. No AI photorealistic images were added.

## Editing and output

Change title, author, tagline, publisher, inks, title face/scale and ornament visibility. Optional uploaded art sits below the typography and ornaments, with opacity control. Each ornament/text element uses existing Layers controls for movement, rotation, visibility, stacking and duplication. Existing Type, Effects, undo, project persistence and editable project backup remain available.

Four starting styles per cover: Source composition, Library copy, Attic find and Clean monochrome. Dot/rule/grid print overlays are editable native layers. Existing Art Dev paper, grain, aging, stains and tears supply surface wear. No external image service is needed.

Existing PNG/JPEG/PDF/SVG export uses the same high-resolution scene. Native cover size is 1500 × 2100; the checked 2× PNG is 3000 × 4200. SVG retains editable text and vector shapes where supported by the existing exporter; effects and uploaded artwork can remain raster elements.

## Typeface repair

The older bundled Anton, Special Elite and Barlow Semi Condensed files fell back for ordinary Latin cover text. Complete font files are bundled locally, with their OFL/Apache licences in `public/fonts/licenses/`; original files remain retained. Runtime does not depend on Google Fonts. Font URLs: Google Fonts/gstatic Anton v27, Special Elite v20 and Barlow Semi Condensed v16.

## Proof

See `tests/vintage-source.spec.ts` for all-ten render/layer/catalogue checks, real SVG and 2× PNG exports, layer undo, saved/reopened project, backup import and 390px mobile layout. Contact sheet: `qa/vintage-source-contact-sheet.png`.

Physical Safari/iPhone/Android, camera and paper acceptance remain separate from browser checks. Fonts and sample designs are not an assurance of third-party trademark or historical clearance.
