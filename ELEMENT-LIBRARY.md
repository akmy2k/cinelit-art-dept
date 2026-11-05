# Graphic element library

Open **Elements** beside Layers, or use **Layers → Elements**. Search or choose a collection, select an ink, then tap a graphic. It becomes a separate layer in the current project. Drag on the canvas, use the corner handles to resize, or use Layers to set width, height, rotation, opacity, ink and line weight. Duplicate, reorder, hide and undo use the existing editor tools.

## Included collection

40 original vector pieces are bundled with the app: six frames, six flourishes, six badges, four ribbons, four botanical ornaments, four symbols, four arrows and six patterns. They require no remote art service. Stars mark favourites on this browser/device; favourites are a browsing preference rather than part of project backups.

Every inserted piece is one independent graphic layer. Internal strokes/leaves within a piece are not individual sublayers. Native vector paths are retained by ordinary SVG export; the existing soft/pixelated screen-export mode deliberately rasterizes the complete screen. PNG/JPEG/PDF follow the existing export pipeline.

**Add your own artwork** creates an image layer with a replacement/upload control. Uploaded scans move as a single image; they do not automatically become editable paths or separate objects. High-resolution transparent PNGs are useful for isolated vintage art. Keep source-page links and rights statements with any future source pack; no third-party public-domain download pack was added by this release.

## What can currently move?

- Native packaging and the ten Vintage Forge source covers expose their designed text, shapes and art as layers.
- Many other templates expose text and uploaded images through the existing direct-selection system.
- Some older template decorations are baked into their renderer, and composite raster art stays a single image. This release does not claim to separate every detail of every existing design.
- All newly added library graphics use independent movable layers across the editor, including older templates.

Hollow library frames ignore clicks through their central opening, so text/art inside remains selectable. Overlapping click/drag now targets the newly clicked region consistently. Startup controls wait for the initial project to load, avoiding a fast edit being overwritten by late initialization.

## Implementation and proof

Original paths: `src/lib/graphic-elements.ts`; browser: `src/components/ElementLibrary.tsx`; scene/validation: `src/lib/layers.ts`; hit testing: `src/lib/selection.ts`. Graphic IDs are validated against the bundled catalogue on project import. Added layers, transformations, ink and line weight use existing durable projects, undo, backup/import and export.

`tests/element-library.spec.ts` checks all 40 distinct renders and valid vectors, real insert/drag/recolour/stroke/duplicate/undo, saved reopening and backup roundtrip, SVG, hollow-frame selection, favourites and mobile width. Contact sheet: `qa/graphic-elements-contact-sheet.png`.

Physical phone gestures, final print/camera usefulness and any future external-art rights review remain separate from browser verification.
