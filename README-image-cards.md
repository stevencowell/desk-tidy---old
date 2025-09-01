# Image Cards CSS System

This CSS system provides consistent 40mm image cards with proper semantics and responsive layout for the Desk Tidy Project.

## Features

- **40mm sizing**: Uses CSS absolute length units for consistent sizing
- **No distortion**: `object-fit: contain` keeps images proportional
- **Proper semantics**: Uses `<figure>` and `<figcaption>` for accessibility
- **Side-by-side layout**: Flex container for multiple images
- **Responsive**: Adapts to different screen sizes
- **Print-friendly**: Optimized for PDF generation

## Usage

### Single Image Card

```html
<div class="image-card">
  <figure>
    <img src="your-image.png" alt="Description">
    <figcaption>Caption text</figcaption>
  </figure>
</div>
```

### Multiple Images Side-by-Side

```html
<div class="image-cards">
  <div class="image-card">
    <figure>
      <img src="image1.png" alt="Description 1">
      <figcaption>Caption 1</figcaption>
    </figure>
  </div>
  
  <div class="image-card">
    <figure>
      <img src="image2.png" alt="Description 2">
      <figcaption>Caption 2</figcaption>
    </figure>
  </div>
</div>
```

## File Structure

- `image-cards.css` - Main CSS file with all image card styles
- `image-cards-example.html` - Example implementation
- `index.html` - Main project file (already includes the CSS link)

## Integration

The CSS is already linked in your main `index.html` file. You can start using the image cards immediately by adding the HTML structure above to any content section.

## Example Use Cases

1. **Construction Progress**: Before/after comparisons
2. **Multiple Views**: Front, side, top views of the desk tidy
3. **Process Steps**: Step-by-step construction photos
4. **Design Variations**: Different design options

## Technical Notes

- Images maintain aspect ratio with `object-fit: contain`
- Cards are exactly 40mm × 40mm (perfect for print/PDF)
- Responsive breakpoints: 768px and 480px
- Print media queries prevent page breaks within cards