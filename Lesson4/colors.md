# Colors

## Standard Colors

Standard colors, e.g., blue, red, yellow.

```CSS
  p {
    color: blue;
  }
```

Full list can be found here: [W3Schools Color Names](https://www.w3schools.com/tags/ref_colornames.asp)

---

## HEX & HEXA

### HEX:

* HEX colors are defined with a hashtag (`#`) followed by six characters, representing the red, green, and blue (RGB) components of the color.
* Format: `#RRGGBB`
* Example: `#FF5733` is a shade of orange.

```CSS
  p {
    color: #FF5733;
  }
```

### HEXA (Hex with Alpha):

* HEXA is a HEX color with an additional component for alpha (opacity/transparency).
* Format: `#RRGGBBAA` (last two characters represent opacity).
* Example: `#FF573380` is the same color as `#FF5733` with 50% transparency.

```CSS
  p {
    color: #FF573380; /* Semi-transparent orange */
  }
```

---

## RGB & RGBA

### RGB:

* RGB stands for Red, Green, and Blue, and the values range from `0` to `255`.
* Format: `rgb(red, green, blue)`
* Example: `rgb(255, 87, 51)` is a shade of orange.

```CSS
  p {
    color: rgb(255, 87, 51);
  }
```

### RGBA:

* RGBA is RGB with an additional value for Alpha (opacity/transparency).
* Format: `rgba(red, green, blue, alpha)`
* The `alpha` value ranges from `0` (fully transparent) to `1` (fully opaque).
* Example: `rgba(255, 87, 51, 0.4)` is an orange with 40% opacity.

```CSS
  p {
    color: rgba(255, 87, 51, 0.4); /* Semi-transparent orange */
  }
```

---

## HSL & HSLA

### HSL:

* HSL stands for Hue, Saturation, and Lightness.

  * **Hue (H)**: A value from 0 to 360, representing the color (e.g., 0 is red, 120 is green, 240 is blue).
  * **Saturation (S)**: A percentage from 0% to 100% that defines how intense the color is. 100% is fully saturated.
  * **Lightness (L)**: A percentage from 0% to 100% that defines how light or dark the color is. 0% is black, 100% is white.
* Format: `hsl(hue, saturation%, lightness%)`
* Example: `hsl(9, 100%, 60%)` is a bright orange.

```CSS
  p {
    color: hsl(9, 100%, 60%); /* Bright orange */
  }
```

### HSLA:

* HSLA is HSL with an additional Alpha (opacity/transparency) component.
* Format: `hsla(hue, saturation%, lightness%, alpha)`
* The `alpha` value ranges from `0` (fully transparent) to `1` (fully opaque).
* Example: `hsla(9, 100%, 60%, 0.4)` is an orange with 40% opacity.

```CSS
  p {
    color: hsla(9, 100%, 60%, 0.4); /* Semi-transparent orange */
  }
```

---

## Best Practices

* **Consistency**: It's a good practice not to mix different color types (HEX, RGB, HSL) in the same project unless needed. Choose one and stick to it for uniformity.
* **Opacity**: If transparency is required, use RGBA or HSLA instead of HEXA for better readability and control over the transparency.
