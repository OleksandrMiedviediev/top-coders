# Reviews Section Design

## Goal

Build the Reviews section from the English Excellence Figma design. The section must remain usable and visually stable from 320px through desktop widths.

## Structure

- Add a semantic `<section>` with an accessible heading.
- Use “What our students say” as the section heading.
- Add the supporting paragraph from the design.
- Render the three reviews as an unordered list.
- Place each student avatar in a content `<img>` with descriptive alternative text.

## Responsive Layout

- From 320px: show one review card.
- From 768px: show two review cards in a two-column grid.
- From 1280px: show all three cards in a three-column grid.
- Keep the cards equal in height at each breakpoint.
- Match the project container widths and breakpoint conventions.
- Use CSS only; the section does not need a carousel or JavaScript.

## Images

- Store all review avatars in `src/images`.
- Provide 1x and 2x raster files through `<picture>` or `srcset`.
- Set explicit image dimensions to reduce layout shift.
- Use lazy loading and asynchronous decoding.
- Optimize the source files before committing them.

## Project Integration

- Implement markup in `src/partials/reviews.html`.
- Implement styles in `src/css/reviews.css`.
- Keep the existing Reviews `<load>` entry in `src/index.html`.
- Keep the existing Reviews import in `src/css/styles.css`, which is the project’s current CSS entry file.
- Do not modify unrelated sections.

## Verification

- Build the Vite project.
- Validate the section at 320px, 375px, 768px, and 1280px.
- Check intermediate widths for overflow and broken card layouts.
- Check the browser console for errors.
- Confirm semantic list and image requirements in the generated page.
