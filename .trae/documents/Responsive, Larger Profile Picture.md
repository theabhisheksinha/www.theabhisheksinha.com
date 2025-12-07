## Goal
- Make the profile picture slightly larger and dynamically fit the browser’s aspect ratio without distortion.

## Implementation
- Update `.profile-pic` styles in `index.html:349–361`:
  - Set `width: clamp(340px, 30vw, 580px)` and `height: auto`.
  - Add `aspect-ratio: 1` and `max-width: 100%` to preserve the circular crop.
  - Keep `border-radius: 50%` and `object-fit: cover` as-is.
- Remove fixed-size overrides for `.profile-pic` in media queries (`index.html:1207–1211`, `index.html:1300–1304`) so the clamp handles responsive sizing.
- Ensure the grid column allows the larger image without overlap; keep `hero-content` columns (`1fr 1.2fr`) unchanged unless layout clips, then adjust to `1fr 1fr`.

## Optional Enhancements
- Add `srcset` to `<img>` at `index.html:1451` with higher-resolution variants if available to keep crispness on high-DPI screens.
- Slightly increase border thickness proportionally if desired to maintain visual balance when image scales.

## Verification
- Preview at `http://localhost:8000/`.
- Resize the window across desktop/tablet/mobile; confirm the image scales smoothly, remains circular, does not overflow, and maintains spacing.
- Check performance and clarity; if any blur appears, lower the max clamp or provide a higher-res image.