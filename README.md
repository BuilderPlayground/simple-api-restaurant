# LastCall — Use Everything Up

**Make more of what's already on hand.**

LastCall is a browser-based application that helps restaurant teams discover meal ideas using ingredients they already have available.

Powered by TheMealDB API, the application allows users to search by ingredient and explore matching dishes through a visual, easy-to-navigate interface.

Designed with restaurant operations and food-waste reduction in mind, LastCall explores how accessible recipe discovery can help kitchen teams find inspiration and make more intentional use of available ingredients.

## Application Preview

![LastCall — Use Everything Up application preview](img/lastcall-use-everything-up.png)

## Features

- **Ingredient-Based Search:** Enter an ingredient to discover matching meal ideas.
- **Meal API Integration:** Retrieve relevant dishes using TheMealDB API.
- **Visual Meal Discovery:** Display meal names and accompanying photographs.
- **Dynamic Results:** Generate meal cards directly from API responses.
- **Updated Search Results:** Clear previous results when performing a new search.
- **Empty-State Feedback:** Display a message when no matching meals are found.

## Tech Stack

| Technology | Purpose |
|------------|---------|
| HTML5 | Application structure and ingredient search interface |
| CSS3 | Styling, layout, and visual meal cards |
| JavaScript | User interactions, API requests, and DOM manipulation |
| Fetch API | Asynchronous requests to the meal database |
| TheMealDB API | Meal information and image data |

## Technical Highlights

### Ingredient-Based API Integration

LastCall uses TheMealDB's ingredient-filtering endpoint to retrieve meals associated with a user-provided ingredient.

When a user selects **Find Ideas**, JavaScript reads the search input, constructs an API request, and retrieves matching meal data.

### Dynamic Meal Cards

The application processes the returned API response and creates individual meal cards using JavaScript.

Each card includes:

- The meal's name
- An accompanying meal photograph

The cards are inserted into the results section without reloading the page.

### Search Result Management

Before displaying new results, the application clears the previous search results.

This ensures that each search presents a fresh set of matching dishes rather than combining results from multiple searches.

### Empty-State Handling

When TheMealDB returns no matching meals, LastCall displays a message informing the user that no meal ideas were found for the selected ingredient.

## Product Roadmap

LastCall establishes a foundation for exploring how recipe discovery can support more resource-conscious kitchen operations.

Potential enhancements include:

- **Detailed Recipes:** Allow users to open individual dishes to view ingredients, preparation instructions, and cooking methods.
- **Multi-Ingredient Search:** Find meal ideas using combinations of available ingredients.
- **Inventory Integration:** Connect searches to a kitchen's existing ingredient inventory.
- **Waste Reduction Insights:** Explore ways to identify ingredients approaching expiration and prioritize their use.
- **Menu Planning:** Help kitchen teams organize potential dishes into menus or specials.
- **Saved Ideas:** Allow users to bookmark recipes and revisit them later.
- **Enhanced Search Experience:** Introduce input validation, loading indicators, and clearer feedback when API requests fail.
- **Responsive Refinements:** Improve the search interface and meal card layout across smaller screens.

These enhancements represent potential future development rather than functionality currently available.

## Getting Started

### Run Locally

1. Clone the repository's `answer` branch:

   ```bash
   git clone --branch answer --single-branch https://github.com/BuilderPlayground/simple-api-restaurant.git
   ```

2. Navigate to the project directory:

   ```bash
   cd simple-api-restaurant
   ```

3. Open the project in VS Code.

4. Launch `index.html` using Live Server.

5. Enter an ingredient, such as `salmon`, and select **Find Ideas**.

6. Explore the matching meal ideas displayed in the results section.

## Project Structure

```text
simple-api-restaurant/
├── css/
│   ├── normalize.css
│   ├── reset.css
│   └── style.css
├── img/
│   └── lastcall-use-everything-up.png
├── js/
│   └── main.js
├── index.html
└── README.md
```

## Credits & Acknowledgments

Built using the [Resilient Labs starter repository](https://github.com/Resilient-Labs/simple-api-restaurant).

Meal information and imagery are provided through [TheMealDB API](https://www.themealdb.com/api.php).
