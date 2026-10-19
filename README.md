# Responsive Web Design

## 1. Project Objective
Develop a responsive webpage that adapts to desktop, tablet, and mobile screen sizes using semantic HTML5 and modern CSS3.

## 2. Technologies Used
- HTML5
- CSS3
- CSS Grid and Flexbox
- Media queries
- CSS custom properties
- Fluid typography with `clamp()`
- Responsive images
- Git and GitHub (if used for version control)

## 3. Project Structure
- `index.html`: Semantic page structure and content.
- `style.css`: Layout, visual styling, and responsive rules.
- `README.md`: Project documentation.

## 4. Responsive Design Techniques

### Fluid layouts
The CSS `min()`, `clamp()`, and percentage-based widths help content adapt to available screen space.

### CSS Grid
CSS Grid creates a two-column hero layout and a three-column feature section on larger screens.

### Flexbox
Flexbox aligns navigation items and allows the header to wrap on smaller devices.

### Media queries
- Above 900px: Desktop-oriented layout.
- At 900px and below: Tablet adjustments and two-column cards.
- At 600px and below: Single-column hero and feature cards.
- At 360px and below: Additional adjustments for small phones.

### Responsive images
Images use `max-width: 100%`, `height: auto`, and `object-fit: cover` to prevent them from overflowing their containers.

### Accessibility
Semantic elements, descriptive image alternative text, visible keyboard focus, and reduced-motion support improve usability.

## 5. Layout Adjustments

| Viewport | Expected layout |
| --- | --- |
| 1440px desktop | Two-column hero; three feature cards |
| 768px tablet | Two-column hero; two-column feature cards |
| 390px mobile | Stacked hero; one feature card per row |
| 320px small phone | Single-column content with tighter spacing |

These are intended layouts. Confirm them using browser developer tools.

## 6. Testing Procedure
1. Open `index.html` in a browser.
2. Open developer tools using F12 or Ctrl+Shift+I.
3. Enable device emulation.
4. Test widths of 1440px, 768px, 390px, and 320px.
5. Check navigation links, image scaling, text wrapping, and card alignment.
6. Verify that no horizontal scrollbar appears.
7. Check keyboard focus and reduced-motion behavior.
8. Record actual results and fix any issues found.

## 7. Challenges and Solutions

### Challenge: Content overflowing on small screens
**Solution:** Use flexible widths, `minmax(0, 1fr)`, and responsive media queries.

### Challenge: Images appearing too large
**Solution:** Set `max-width: 100%`, `height: auto`, and an appropriate aspect ratio.

### Challenge: Text becoming too large or too small
**Solution:** Use `clamp()` for fluid headings and adjust spacing at smaller breakpoints.

### Challenge: Feature cards not fitting narrow screens
**Solution:** Change the grid from three columns to two and then one column at the relevant breakpoints.

## 8. Conclusion
This project demonstrates how HTML5 and CSS3 can be used to build a responsive webpage. CSS Grid, Flexbox, fluid sizing, and media queries help maintain a usable layout across different screen sizes.

## 9. Before Submission
- Test all target viewport sizes in a browser.
- Update this README with actual test results.
- Capture desktop, tablet, and mobile screenshots if required.
- Add the files to your GitHub repository.
