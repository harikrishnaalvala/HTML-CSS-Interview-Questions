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

## 1. What is the difference between Block and Inline Elements?

### Comparison

| Block Elements | Inline Elements |
|---------------|----------------|
| Occupy full available width | Occupy only required width |
| Start on a new line | Stay within the same line |
| Width and height can be applied | Width and height generally don't apply |
| Used for page structure | Used for styling/content within text |

### Block Elements

```html
<div>Block Element</div>
<p>Paragraph</p>
<section>Section</section>
```

### Inline Elements

```html
<span>Inline Element</span>
<a href="#">Link</a>
<strong>Bold Text</strong>
```

### Real-World Use Cases

#### Block Elements
- Page layouts
- Sections
- Cards
- Containers

#### Inline Elements
- Links
- Text styling
- Icons
- Labels

---

## 2. What is the purpose of the `alt` attribute in an `<img>` tag?

The `alt` attribute provides alternative text when an image cannot be displayed.

### Example

```html
<img src="profile.jpg" alt="User profile picture">
```

### Why It Is Important

#### Accessibility
Screen readers use the alt text to describe images to visually impaired users.

#### SEO
Search engines use alt text to understand image content.

#### Fallback Content
If an image fails to load, the alt text is displayed.

### Good Example

```html
<img src="dog.jpg" alt="Golden Retriever playing in a park">
```

### Poor Example

```html
<img src="dog.jpg" alt="image">
```

---

## 3. What is the difference between `<div>` and `<section>`?

### Comparison

| `<div>` | `<section>` |
|----------|------------|
| Generic container | Semantic container |
| No specific meaning | Represents a logical section |
| Used for styling/layout | Used for grouping related content |
| Less SEO-friendly | Better for SEO and accessibility |

### Using `<div>`

```html
<div class="about">
  <h2>About Us</h2>
  <p>Company information</p>
</div>
```

### Using `<section>`

```html
<section>
  <h2>About Us</h2>
  <p>Company information</p>
</section>
```

### When to Use

#### Use `<div>`
- Styling purposes
- Layout containers
- Wrappers

#### Use `<section>`
- Blog sections
- About page sections
- Feature sections
- Related content groups

---

# 🎨 CSS

## 4. What is the CSS Box Model?

Every HTML element is represented as a rectangular box.

### Structure

```text
Margin
 └── Border
      └── Padding
           └── Content
```

### Components

#### Content

The actual content such as text, images, or videos.

```css
width: 200px;
height: 100px;
```

---

#### Padding

Space between content and border.

```css
padding: 20px;
```

---

#### Border

Wraps around content and padding.

```css
border: 2px solid black;
```

---

#### Margin

Space outside the border.

```css
margin: 10px;
```

---

### Example

```css
.box {
  width: 200px;
  padding: 20px;
  border: 2px solid black;
  margin: 10px;
}
```

---

## 5. What is Flexbox?

Flexbox is a one-dimensional layout model used to align and distribute elements efficiently.

### Center an Element Horizontally and Vertically

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
```

```html
<div class="container">
  <div>Centered Content</div>
</div>
```

### Explanation

#### justify-content

Aligns items along the main axis.

```css
justify-content: center;
```

#### align-items

Aligns items along the cross axis.

```css
align-items: center;
```

### Common Use Cases

- Navigation bars
- Dashboard layouts
- Card grids
- Centered modals
- Login forms

---

## 6. What are Pseudo-Classes and Pseudo-Elements?

### Pseudo-Classes

Pseudo-classes target elements based on their state.

### Examples

```css
button:hover {
  background-color: blue;
}

input:focus {
  border: 2px solid green;
}

li:first-child {
  color: red;
}
```

### Common Pseudo-Classes

```css
:hover
:focus
:active
:first-child
:last-child
:nth-child()
```

---

### Pseudo-Elements

Pseudo-elements target specific parts of an element.

### Examples

```css
p::first-letter {
  font-size: 2rem;
}

p::before {
  content: "★ ";
}

p::after {
  content: " ✓";
}
```

### Common Pseudo-Elements

```css
::before
::after
::first-letter
::first-line
::selection
```

---

### Difference

| Pseudo-Class | Pseudo-Element |
|-------------|---------------|
| Targets state | Targets part of an element |
| Uses `:` | Uses `::` |
| Example: `:hover` | Example: `::before` |

---

## 7. Difference Between `position: relative` and `position: absolute`

### Comparison

| Relative | Absolute |
|-----------|----------|
| Positioned relative to itself | Positioned relative to nearest positioned ancestor |
| Remains in normal document flow | Removed from normal flow |
| Keeps original space | Does not keep original space |
| Used for small adjustments | Used for precise placement |

---

### Relative Example

```css
.box {
  position: relative;
  top: 20px;
  left: 30px;
}
```

The element moves while preserving its original space.

---

### Absolute Example

```css
.parent {
  position: relative;
}

.child {
  position: absolute;
  top: 0;
  right: 0;
}
```

The child is positioned relative to the parent.

---

### Real-World Use Cases

#### Relative
- Fine-tuning positions
- Base container for absolute children

#### Absolute
- Tooltips
- Dropdown menus
- Notification badges
- Modals
- Floating buttons

---

