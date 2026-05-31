# HTML-CSS-Interview-Questions

---

# 🌐 HTML

## ❓ What is Shadow DOM?

Shadow DOM is a browser technology that provides encapsulation for HTML, CSS, and JavaScript inside a component.

It creates a separate DOM tree that is isolated from the main document DOM.

### ✅ Benefits
- Style isolation
- Prevents CSS conflicts
- Improves component reusability
- Encapsulation of markup and behavior

### ✅ Real-World Examples
- Web Components
- Design Systems
- Native browser elements like `<video>` and `<input>`

---

# 🎨 CSS

## ❓ Difference Between Inline and Block Elements

| Inline Elements | Block Elements |
|---|---|
| Occupies only required width | Occupies full available width |
| Doesn't start on a new line | Starts on a new line |
| Width and height usually don't apply | Width and height can be controlled |

### ✅ Inline Examples

```html
<span>Hello</span>
<a href="#">Link</a>
<strong>Text</strong>
```

### ✅ Block Examples

```html
<div>Content</div>
<p>Paragraph</p>
<section>Section</section>
```

---

## ❓ What is CSS Isolation?

CSS Isolation means limiting styles to a specific component or scope so they don't affect other components.

### ✅ Methods
- CSS Modules
- Shadow DOM
- Styled Components
- Tailwind CSS
- CSS-in-JS Libraries

### ✅ Benefits
- Prevents style conflicts
- Easier maintenance
- Better component reusability

---

## ❓ Adaptive vs Responsive Web Design

| Adaptive Design | Responsive Design |
|---|---|
| Multiple fixed layouts | Flexible layout |
| Device-specific designs | Fluid design |
| More maintenance | Easier maintenance |
| Uses predefined breakpoints | Uses flexible grids |

### ✅ Adaptive Example
Different layouts for:
- Mobile
- Tablet
- Desktop

### ✅ Responsive Example
Uses:
- Flexbox
- CSS Grid
- Media Queries

to automatically adjust content.

---

## ❓ What is Tailwind CSS and Why is it Famous?

Tailwind CSS is a utility-first CSS framework that provides pre-built utility classes.

### ✅ Example

```html
<button class="bg-blue-500 text-white p-2 rounded">
  Submit
</button>
```

### ✅ Why It Is Popular
- Faster development
- No need to write large CSS files
- Consistent UI design
- Easy customization
- Smaller production builds

### ✅ Benefits
- Rapid prototyping
- Reusable utility classes
- Better maintainability

---
