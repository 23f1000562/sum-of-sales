# Sales Summary Dashboard

This project provides a simple, single-page web application to display a summary of sales data fetched from a local `data.csv` file. It's built with modern web standards, using HTML, JavaScript, and Tailwind CSS for a responsive and clean user interface.

## Features

- **Dynamic Data Fetching**: Reads sales data from `data.csv`.
- **Sales Summation**: Automatically calculates the total sales from the 'sales' column.
- **Responsive Design**: Utilizes Tailwind CSS for a mobile-first, responsive layout.
- **Clear Presentation**: Displays the total sales prominently on the page.
- **Dynamic Title**: Sets the page title to 'Sales Summary [Current Period]'.

## Setup and Usage

To run this application, you only need a web browser and the provided files. No backend server or complex build tools are required for development, as it's a static HTML file that fetches a local CSV.

1.  **Save the files**: Ensure `index.html` and `data.csv` are in the same directory.
2.  **Open `index.html`**: Simply open `index.html` in your preferred web browser.

### `data.csv` Format

The `data.csv` file should be a comma-separated values file with at least one header row. It must contain a column named `sales` (case-insensitive) for the application to correctly calculate the total.

**Example `data.csv`:**

```csv
product,sales,quantity
Laptop,1200.50,5
Mouse,25.75,10
Keyboard,75.00,8
Monitor,300.25,3
```

## Technology Stack

-   **HTML5**: Structure of the web page.
-   **Tailwind CSS**: Utility-first CSS framework for styling.
-   **JavaScript (ES6+)**: For fetching, parsing data, and updating the DOM.

## Error Handling

The application includes basic error handling for scenarios such as:

-   `data.csv` file not found or inaccessible.
-   `data.csv` being empty.
-   The 'sales' column not being present in `data.csv`.

In case of an error, an informative message will be displayed on the page instead of the sales total.

## Customization

-   **`index.html`**: Modify the HTML structure and Tailwind classes to change the layout and styling.
-   **JavaScript**: Adjust the `fetchDataAndDisplay` function in the `<script>` tag to alter data processing or display logic.
-   **Title Seed**: The `titleSeed` variable in the JavaScript can be changed to update the dynamic part of the page title.

## License

This project is open-source and available under the MIT License. See the `LICENSE` file for more details.