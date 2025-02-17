

# 3D Rotate on Hover Effect

This project demonstrates a **3D rotate effect on hover** created entirely using **CSS**. It utilizes the `:nth-child` pseudo-class to apply the effect to multiple elements, giving them a dynamic and interactive 3D feel when hovered over.

## Features

- **CSS-only solution**: No JavaScript is needed for the hover effect.
- **3D Rotation**: Elements rotate on hover, providing a 3D perspective.
- **Responsive**: The effect adjusts according to the screen size, making it versatile for different layouts.
- **Customizable**: Easily modify the number of elements, rotation angles, or styles through simple CSS changes.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AashirZayd/3D-Rotate-on-Hover.git
   ```

2. Navigate to the project directory:
   ```bash
   cd 3D-Rotate-on-Hover
   ```

3. Open the `index.html` file in your browser to see the effect in action.

## Usage

- This effect works by applying a CSS transform to each child element when it is hovered over.
- You can modify the number of elements in the container by adding more or fewer child divs in the HTML.

### Example HTML structure:
``` html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
  <div class="item">Item 4</div>
</div> ```

### Example CSS:
``` css
.container {
  display: flex;
  justify-content: space-around;
}

.item {
  width: 100px;
  height: 100px;
  background-color: #3498db;
  transition: transform 0.5s;
}

.item:hover {
  transform: rotateY(180deg);
}

.item:nth-child(odd) {
  transform: rotateY(30deg);
}

.item:nth-child(even) {
  transform: rotateY(-30deg);
} ```


You can tweak the rotation, colors, or animation speed as desired.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
