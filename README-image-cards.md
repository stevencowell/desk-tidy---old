# Image Cards CSS System

This CSS system provides consistent 40mm image cards with proper semantics and responsive layout for the Desk Tidy Project.

## Features

- **40mm sizing**: Uses CSS absolute length units for consistent sizing
- **No distortion**: `object-fit: contain` keeps images proportional
- **Proper semantics**: Uses `<figure>` and `<figcaption>` for accessibility
- **Side-by-side layout**: Flex container for multiple images
- **Responsive**: Adapts to different screen sizes
- **Print-friendly**: Optimized for PDF generation

## Implementation Status

✅ **Fully Implemented and Integrated**

The image cards system has been successfully integrated into the Desk Tidy Project with:

- **Week 1 (Safety)**: Safety equipment, PPE, and emergency equipment images
- **Week 2 (Design & Tools)**: Essential tools, power tools, and materials
- **Week 7 (Hardware)**: Hardware tools and safety equipment for attachments
- **Enhanced Example**: Updated demonstration with real project images

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
- `image-cards-example.html` - Enhanced example with real project images
- `index.html` - Main project file (already includes the CSS link)
- `sections/main-theory/week1.html` - Week 1 with safety equipment images
- `sections/main-theory/week2.html` - Week 2 with tools and materials
- `sections/main-theory/week7.html` - Week 7 with hardware tools

## Integration

The CSS is already linked in your main `index.html` file. The image cards have been integrated into:

1. **Week 1**: Safety equipment, PPE, and emergency equipment
2. **Week 2**: Essential tools, power tools, and materials
3. **Week 7**: Hardware tools and safety equipment

## Example Use Cases

1. **Safety Equipment**: PPE, safety signs, emergency equipment
2. **Tools and Equipment**: Hand tools, power tools, measuring equipment
3. **Materials**: Timber, paint, hardware
4. **Construction Progress**: Before/after comparisons
5. **Multiple Views**: Front, side, top views of the desk tidy
6. **Process Steps**: Step-by-step construction photos

## Technical Notes

- Images maintain aspect ratio with `object-fit: contain`
- Cards are exactly 40mm × 40mm (perfect for print/PDF)
- Responsive breakpoints: 768px and 480px
- Print media queries prevent page breaks within cards
- Uses semantic HTML with `<figure>` and `<figcaption>`
- Flexbox layout for consistent spacing and alignment

## Image Sources

The system uses real construction and workshop images from the `Construction Pictures/` directory, including:
- Safety equipment (hard hats, gloves, boots, etc.)
- Tools (hammers, drills, saws, etc.)
- Materials (timber, paint, etc.)
- Safety signs and emergency equipment