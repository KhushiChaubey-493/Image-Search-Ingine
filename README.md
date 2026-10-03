# 🔎 Image Search Engine

A responsive image search web application built with **HTML, CSS, and JavaScript** that allows users to search for images using the **Unsplash API**.

The application dynamically fetches image results from Unsplash and displays them in a responsive gallery. Users can search for new images and load additional results using the **Show More** feature.

## 🌐 Live Demo

**[View Live Demo](https://khushichaubey-493.github.io/Image-Search-Ingine/)**

> If GitHub Pages is not enabled for this repository yet, configure it from **Settings → Pages** before adding the live-demo link.

## 📸 Project Preview

*Add your project screenshot here.*

```markdown
![Image Search Engine Preview](screenshot.png)
```

## ✨ Features

* 🔍 Search images using keywords
* 🌐 Integration with the Unsplash REST API
* 🖼️ Dynamically display search results
* 📱 Responsive image gallery
* ➕ Load additional images with **Show More**
* 🔄 Pagination support using API page parameters
* 🔗 Click an image to open its Unsplash page
* ⚡ Asynchronous API requests using `fetch()`
* 🎨 Clean and simple user interface
* 🚫 Prevents the browser's default form submission behavior

## 🛠️ Technologies Used

| Technology            | Purpose                                 |
| --------------------- | --------------------------------------- |
| **HTML5**             | Page structure and search interface     |
| **CSS3**              | Styling, layout, and responsive gallery |
| **JavaScript (ES6+)** | Application logic and API integration   |
| **Unsplash API**      | Fetching image search results           |
| **Fetch API**         | Making asynchronous HTTP requests       |
| **DOM Manipulation**  | Dynamically rendering images            |

## 🔌 API Integration

This project uses the **Unsplash Search API** to retrieve images based on the user's search query.

The application sends requests using the following endpoint:

```text
https://api.unsplash.com/search/photos
```

The request includes:

* Search keyword
* Current page number
* Unsplash API access key
* Number of results per request

The application currently requests **12 images per page**.

## ⚙️ How It Works

### 1. Enter a Search Term

The user enters a keyword into the search box.

For example:

```text
nature
```

### 2. Submit the Search

When the form is submitted, JavaScript prevents the default page reload and starts the image search.

### 3. Fetch Images

The application sends a request to the Unsplash API using the entered keyword.

### 4. Process the Response

The API returns image information in JSON format.

The application extracts:

* Image URL
* Image page URL

### 5. Display Results

JavaScript creates image elements dynamically and adds them to the search-results container.

### 6. Load More Results

Clicking **Show More** increments the page number and requests the next set of results.

## 🔄 Application Flow

```text
        Enter Search Keyword
                ↓
          Submit Search
                ↓
       Send API Request
                ↓
        Unsplash API
                ↓
       Receive JSON Data
                ↓
       Extract Image URLs
                ↓
      Generate Image Elements
                ↓
        Display Gallery
                ↓
          Show More
                ↓
       Fetch Next Page
```

## 🧠 JavaScript Concepts Practiced

This project helped strengthen the following JavaScript concepts:

* DOM manipulation
* Event listeners
* Form submission handling
* `preventDefault()`
* `async/await`
* `fetch()`
* Promises
* API integration
* JSON response handling
* Template literals
* Dynamic element creation
* `appendChild()`
* Pagination logic
* Variables and state management

## 📂 Project Structure

```text
Image-Search-Ingine/
│
├── index.html
├── index.js
├── style.css
└── README.md
```

The current repository contains these three main source files: `index.html`, `index.js`, and `style.css`.

## 🚀 Getting Started

### Prerequisites

You need:

* A modern web browser
* A code editor such as VS Code
* Internet connection
* A valid Unsplash API access key

### 1. Clone the Repository

```bash
git clone https://github.com/KhushiChaubey-493/Image-Search-Ingine.git
```

### 2. Navigate to the Project

```bash
cd Image-Search-Ingine
```

### 3. Configure the API Key

The current JavaScript file contains an Unsplash access key directly in the frontend code.

For a learning project, you can keep the current setup, but for a production application, the API key should **not be exposed directly in client-side JavaScript**.

### 4. Run the Project

Open `index.html` in your browser.

For development, you can use the **Live Server** extension in VS Code.

## 🖼️ User Experience

The interface provides a straightforward workflow:

1. Open the application.
2. Enter an image-search keyword.
3. Click **Search**.
4. Browse the returned images.
5. Click an image to open its corresponding Unsplash page.
6. Click **Show More** to load additional results.

The implementation opens image links in a new browser tab.

## 📚 Learning Objectives

The main goals of this project were to practice:

* Working with third-party APIs
* Fetching remote data using JavaScript
* Understanding asynchronous programming
* Processing JSON responses
* Dynamically creating DOM elements
* Implementing pagination
* Building responsive frontend layouts
* Handling form events

## 🔮 Future Improvements

Possible improvements for future versions include:

* Add a loading indicator while images are being fetched
* Add an error message for failed API requests
* Handle empty search queries
* Display a "No results found" message
* Add image captions
* Add image download functionality where permitted
* Add category or filter options
* Add infinite scrolling
* Add dark/light theme support
* Improve accessibility with meaningful `alt` text
* Move API-key handling to a secure backend
* Add debouncing for repeated searches
* Add search history

## ⚠️ Security Note

The current implementation stores the Unsplash access key directly in `index.js`.

For a production application, sensitive API credentials should not be exposed in client-side JavaScript. A backend/server-side solution or an appropriate public-client configuration should be used depending on the API provider's authentication model.

## 📌 Project Status

**Completed — Frontend Practice Project**

This project was created to gain practical experience with **JavaScript API integration, asynchronous programming, DOM manipulation, and responsive frontend development**.

## 👩‍💻 Author

**Khushi Chaubey**

* GitHub: [KhushiChaubey-493](https://github.com/KhushiChaubey-493)

## 📄 License

This project was created for **learning and educational purposes**.
