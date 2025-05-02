# CSS Units

## 1. Absolute Units

Absolute units are fixed and do not change based on other elements or the screen size.

### Common Absolute Units:

* **px (pixels)**: Represents a single dot on the screen. It's a fixed size and does not scale with other elements. It's the most commonly used unit in web design.

  ```CSS
  p {
    font-size: 16px;
  }
  ```

* **pt (points)**: Used mainly in print media, 1pt = 1/72 of an inch. It’s rarely used in web development but might be useful when converting print designs.

* **cm (centimeters)**: Physical length, 1cm = 37.795px. Not commonly used for web design as it depends on physical screen dimensions.

* **mm (millimeters)**: Like cm, but much smaller, 1mm = 3.779px. Used mostly in print design.

* **in (inches)**: Physical measurement, 1 inch = 96px. It’s useful for print media but not recommended for responsive web design.

---

## 2. Relative Units

Relative units change based on other properties, like the parent element’s size or the viewport dimensions. They are more flexible and are widely used for responsive web design.

### Common Relative Units:

* **% (percentage)**: The most common relative unit, it is based on the size of the parent element. For example, `width: 50%` would make the element half the width of its parent.

  ```CSS
  div {
    width: 50%; /* 50% of the parent element’s width */
  }
  ```

* **em**: Relative to the font-size of the element. If no font-size is set, it will inherit the font size of the parent element.

  * **1em = current element’s font-size** (usually 16px by default in browsers).
  * **1.5em = 1.5 times the font size of the element**.

  Example:

  ```CSS
  p {
    font-size: 1.5em; /* 1.5 times the font size of the parent element */
  }
  ```

* **rem (root em)**: Similar to `em`, but always relative to the font-size of the root element (`html` or `body` element). By default, most browsers set this to 16px, so `1rem = 16px`. It’s helpful for keeping a consistent design across the website.

  Example:

  ```CSS
  html {
    font-size: 16px;
  }
  p {
    font-size: 2rem; /* 2 times the root font size, i.e., 32px */
  }
  ```

* **vw (viewport width)**: Relative to the width of the viewport (the visible area of the browser window).

  * **1vw = 1% of the viewport’s width**.
  * For example, `width: 50vw` would make the element 50% of the viewport’s width.

  Example:

  ```CSS
  div {
    width: 50vw; /* 50% of the viewport’s width */
  }
  ```

* **vh (viewport height)**: Similar to `vw`, but relative to the height of the viewport.

  * **1vh = 1% of the viewport’s height**.
  * For example, `height: 100vh` would make the element as tall as the viewport.

  Example:

  ```CSS
  div {
    height: 100vh; /* Full height of the viewport */
  }
  ```

---

## Key Differences and Best Practices for Beginners

* **Use absolute units (px, pt, in) when you want fixed sizes that won't change regardless of the screen or parent size**.

  Example: Fixed button size.

* **Use relative units (em, rem, %, vw, vh) to create flexible, responsive designs** that adjust based on the user’s screen size, the parent container, or the root font size. This is essential for making websites work well across different devices and screen resolutions.

* **`rem` vs. `em`**:

  * **`rem`** is typically preferred for global font sizes because it’s based on the root font size, making it easier to scale the whole layout.
  * **`em`** is more specific and based on the font size of the parent element, so it's useful when you want elements to scale based on their parent.

* **Use `vw` and `vh` for full-screen layouts** or responsive designs, especially for elements that need to adjust based on the screen size.