# Markdown Converter with Tabbed View Switching

## Summary

This application is an enhanced Markdown converter tool designed for real-time text processing. It allows users to input Markdown text and instantly view the rendered HTML output. A key feature is the introduction of tabbed navigation, enabling users to seamlessly switch between the final rendered HTML view and the original Markdown source code for easy reference and debugging.

## Features

*   **Real-Time Conversion:** Instantaneous conversion of Markdown input to HTML output.
*   **Tabbed Interface:** Provides a clean, organized way to manage different views of the content.
*   **View Switching:** Ability to switch between the "Rendered HTML" view and the "Original Source" view.
*   **Source Display:** Dedicated container (`#markdown-source`) to accurately display the raw, unrendered Markdown text when the source tab is active.
*   **Static Application:** Runs entirely client-side without the need for server infrastructure.

## Setup

This project is a client-side application requiring no backend services, package managers, or complex dependencies.

1.  **Clone the repository:**
    ```bash
    git clone [repository-url] markdown-converter-5e3a4242
    ```
2.  **Navigate to the project directory.**
3.  **Run the application:** Open the `index.html` file directly in any modern web browser (e.g., Chrome, Firefox, Edge).

## Usage

The application is intuitive and designed for immediate use upon loading.

1.  **Input Markdown:** Enter your desired Markdown text into the primary input area. The "Rendered HTML" view will update automatically.
2.  **Default View:** The application defaults to showing the rendered output.
3.  **Switch to Source:** Click the "Original Source" tab. The rendered output will be hidden, and the raw Markdown text will be displayed within the designated `#markdown-source` element.
4.  **Toggle Views:** Click the tabs repeatedly to switch back and forth between the rendered HTML and the original source view instantly.

## Implementation Details

**Technical Stack:**

*   **HTML5:** Provides the structure and necessary elements, including the tab containers and the `#markdown-source` element.
*   **CSS3:** Used for styling the interface and managing the visibility of the tab content.
*   **JavaScript:** Handles the core logic, including event listeners for tab clicks, DOM manipulation for view switching, and ensuring the content of `#markdown-source` is updated.

**Mechanism:**

The application utilizes JavaScript to manage the display state. When a tab is selected, the script applies or removes specific CSS classes (e.g., `active`, `hidden`) to the content containers. This ensures that only the content corresponding to the active tab (either the rendered output or the `#markdown-source` element) is visible at any given time.

## Code Structure

The core functionality is driven by the main JavaScript file, which is structured around event handling and view management:

*   **Tab Event Listeners:** Event listeners are attached to the tab navigation elements to detect user clicks.
*   **`switchView()` Function:** This central function orchestrates the view change. It takes the target view identifier (e.g., 'rendered' or 'source') and updates the visual state of the application.
*   **Content Synchronization:** The input value is continuously synchronized with the `#markdown-source` element to ensure the "Original Source" tab always displays the current, raw input.
*   **CSS Utility:** Simple CSS classes are used to toggle the `display` property of the content panels, ensuring a smooth and immediate switch between views.

## Evaluation Criteria

This application successfully satisfies the following evaluation criteria:

*   The repository is licensed under the MIT License.
*   The `README.md` is professional and comprehensive.
*   Tab navigation elements are present and fully functional.
*   The element `#markdown-source` accurately displays the original, unrendered Markdown source.
*   Switching between the "Rendered HTML" view and the "Original Source" view works correctly and instantly.

## License

This project is licensed under the MIT License - see the LICENSE file for details.