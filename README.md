# Light and Dark Theme Template

[![GitHub Forks](https://img.shields.io/github/forks/Abdullah-Junayed-290/Light-and-Dark-theme-template?style=social)](https://github.com/Abdullah-Junayed-290/Light-and-Dark-theme-template/network)
[![GitHub Stars](https://img.shields.io/github/stars/Abdullah-Junayed-290/Light-and-Dark-theme-template?style=social)](https://github.com/Abdullah-Junayed-290/Light-and-Dark-theme-template/stargazers)
[![GitHub Issues](https://img.shields.io/github/issues/Abdullah-Junayed-290/Light-and-Dark-theme-template)](https://github.com/Abdullah-Junayed-290/Light-and-Dark-theme-template/issues)
[![GitHub License](https://img.shields.io/github/license/Abdullah-Junayed-290/Light-and-Dark-theme-template)](https://github.com/Abdullah-Junayed-290/Light-and-Dark-theme-template/blob/main/LICENSE)

A simple and easily customizable template demonstrating a light and dark theme toggle using HTML, CSS, and JavaScript. This template provides a basic structure that you can adapt and integrate into your own web projects to offer users a choice between light and dark visual modes.

## Features

* **Clean and Minimalist Design:** Focuses on the core functionality of theme switching without unnecessary complexity.
* **Easy Integration:** Simple HTML structure, well-commented CSS, and straightforward JavaScript make it easy to incorporate into existing projects.
* **Customizable:** The CSS is organized to allow for quick and easy modification of colors and styles for both light and dark themes.
* **Persistent Theme:** The user's preferred theme is saved in local storage, so it persists across page loads.
* **JavaScript Toggle:** A simple JavaScript function handles the theme switching logic and updates the page's classes.

## How to Use

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/Abdullah-Junayed-290/Light-and-Dark-theme-template.git](https://github.com/Abdullah-Junayed-290/Light-and-Dark-theme-template.git)
    ```

2.  **Open `index.html`:** Navigate to the cloned directory and open the `index.html` file in your web browser.

3.  **Explore the Code:**
    * **`index.html`:** Contains the basic HTML structure and a button to toggle the theme.
    * **`style.css`:** Holds the CSS rules for both the light and dark themes. The dark theme styles are often defined after the light theme styles or using a specific class (e.g., `.dark-theme`).
    * **`script.js`:** Includes the JavaScript code that detects the user's preferred theme (if any), applies it on page load, and handles the toggling of the theme by adding or removing a CSS class on the `body` element.

4.  **Integrate into Your Project:**
    * Copy the `index.html`, `style.css`, and `script.js` files into your project.
    * Link the `style.css` file in the `<head>` of your HTML.
    * Include the `script.js` file just before the closing `</body>` tag.
    * Modify the HTML structure, CSS styles, and JavaScript logic as needed to fit your project's requirements.

## Customization

* **CSS (`style.css`):**
    * Modify the color variables or directly change the CSS rules under the `:root` (for light theme) and `.dark-theme` selectors to adjust the appearance of each theme.
    * Add your own styles for different elements and ensure they have corresponding styles for both light and dark modes.

* **JavaScript (`script.js`):**
    * Adjust the class name used for the dark theme (currently `'dark-theme'`) if needed.
    * Modify the logic for saving and retrieving the theme from local storage if you require different behavior.

* **HTML (`index.html`):**
    * Adapt the HTML structure to match your project. Ensure the toggle button has an appropriate ID or class that is referenced in the JavaScript.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to:

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and commit them.
4.  Push your changes to your fork.
5.  Submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE). See the `LICENSE` file for more information.

## Author

[Abdullah Junayed](https://github.com/Abdullah-Junayed-290)
