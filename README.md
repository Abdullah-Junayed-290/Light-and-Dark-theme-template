# Light and Dark Theme Template (Alpine.js & Tailwind CSS)

[![GitHub Forks](https://img.shields.io/github/forks/Abdullah-Junayed-290/Light-and-Dark-theme-template?style=social)](https://github.com/Abdullah-Junayed-290/Light-and-Dark-theme-template/network)
[![GitHub Stars](https://img.shields.io/github/stars/Abdullah-Junayed-290/Light-and-Dark-theme-template?style=social)](https://github.com/Abdullah-Junayed-290/Light-and-Dark-theme-template/stargazers)
[![GitHub Issues](https://img.shields.io/github/issues/Abdullah-Junayed-290/Light-and-Dark-theme-template)](https://github.com/Abdullah-Junayed-290/Light-and-Dark-theme-template/issues)
[![GitHub License](https://img.shields.io/github/license/Abdullah-Junayed-290/Light-and-Dark-theme-template)](https://github.com/Abdullah-Junayed-290/Light-and-Dark-theme-template/blob/main/LICENSE)

A simple and dynamic light and dark theme toggle template built using **Alpine.js** for interactivity and **Tailwind CSS** for styling. This template provides a concise example of how to implement theme switching with minimal JavaScript and the utility-first approach of Tailwind CSS.

## Features

* **Dynamic Theme Switching:** Uses Alpine.js to handle the toggling of light and dark themes without requiring manual DOM manipulation.
* **Tailwind CSS Powered:** Leverages Tailwind CSS classes for rapid styling and easy customization of the themes.
* **Minimal JavaScript:** Relies on Alpine.js directives for a declarative and efficient implementation.
* **State-Driven:** The theme state is managed within the Alpine.js component.
* **Live Text Update:** The button text dynamically updates to reflect the current theme.

## How to Use

1.  **Include CDN Links:** Ensure you have the CDN links for both Alpine.js and Tailwind CSS (browser version) in the `<head>` of your HTML file, as shown in the provided code.

    ```html
    <head>
      <script defer src="[https://cdn.jsdelivr.net/npm/alpinejs@3.14.8/dist/cdn.min.js](https://cdn.jsdelivr.net/npm/alpinejs@3.14.8/dist/cdn.min.js)"></script>
      <script src="[https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4](https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4)"></script>
    </head>
    ```

2.  **Copy the HTML Structure:** Use the provided HTML code as the base for your theme toggle.

    ```html
    <body x-data="{
        darkMod: false,
        text: 'dark mode',
        dark() {
          this.text = 'dark mode'
        },
        light() {
          this.text = 'light mode'
        }
      }" x-bind:class="darkMod ? 'bg-black text-white' : 'bg-white text-black'">
      <button class="border rounded-lg p-10 m-10" x-data x-bind:class="darkMod ? 'bg-white text-black' : 'bg-black text-white'" @click="darkMod = !darkMod" x-on:click="!darkMod ? dark() : light()">
        <strong x-text="text">
        </strong>
      </button>
    </body>
    ```

3.  **Understand the Code:**

    * **`x-data` (on `<body>`):** Initializes an Alpine.js component with the following reactive data:
        * `darkMod`: A boolean to track the current theme (initially `false` for light mode).
        * `text`: The text displayed on the toggle button (initially 'dark mode').
        * `dark()`: A function to set the `text` to 'dark mode'.
        * `light()`: A function to set the `text` to 'light mode'.
    * **`x-bind:class` (on `<body>`):** Dynamically applies CSS classes based on the `darkMod` state. If `darkMod` is true, it applies `bg-black text-white`; otherwise, it applies `bg-white text-black`. These are Tailwind CSS utility classes for background color and text color.
    * **`button` element:**
        * `class="border rounded-lg p-10 m-10"`: Basic Tailwind CSS classes for styling the button (border, rounded corners, padding, margin).
        * `x-data`: Creates a nested Alpine.js component (though in this simple case, it's not strictly necessary but demonstrates nesting).
        * `x-bind:class`: Similar to the `body`, it dynamically changes the button's background and text color based on `darkMod`, providing visual feedback.
        * `@click="darkMod = !darkMod"`: Toggles the `darkMod` state when the button is clicked.
        * `x-on:click="!darkMod ? dark() : light()"`: Calls the `dark()` function if `darkMod` is false (switching to dark mode) and the `light()` function if `darkMod` is true (switching to light mode).
        * **`strong` element:**
            * `x-text="text"`: Binds the text content of the `<strong>` element to the `text` data property, ensuring it updates dynamically.

4.  **Customize Themes:**

    * **Tailwind CSS Configuration (Optional):** For more advanced customization, you can configure Tailwind CSS to define your own color palettes and styles in a `tailwind.config.js` file. However, for basic color switching, directly using the utility classes within the HTML is often sufficient.
    * **Modify Tailwind Classes:** Change the Tailwind CSS classes applied in the `x-bind:class` directives to alter the colors and styles for both the light and dark themes.

## Integration into Your Project

To integrate this theme toggle into your existing project:

1.  Ensure you have Alpine.js and Tailwind CSS included in your HTML (either via CDN or by installing them through npm/yarn and configuring your build process).
2.  Copy the `<button>` element and the `x-data` attribute from the `<body>` tag into your desired location in your HTML structure.
3.  Adapt the Tailwind CSS classes in the `x-bind:class` directives on the elements you want to theme (e.g., `body`, `header`, `main`, etc.) to match your desired light and dark mode styles.

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
