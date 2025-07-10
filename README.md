# Movie-TV-Show-Explorer

🎬 Movie & TV Show Explorer
💡 Concept
The Movie & TV Show Explorer is a dynamic web application that allows users to search for, discover, and manage trending movies and TV shows. It provides detailed information for each title, including posters, ratings, plot summaries, and embedded trailer links, alongside a personal watchlist feature.

✨ Features
Trending Content: Browse the latest trending movies and TV shows.

Search Functionality: Easily search for specific movies or TV shows by title.

Genre Filtering: Filter content by various genres to narrow down your interests.

Infinite Scrolling: Seamlessly load more movies or TV shows as you scroll down the page, providing a smooth browsing experience without the need for a "Load More" button.

Loading Indicators: Visual feedback (a spinner and message) is displayed while content is being fetched from the API.

Enhanced Error Handling: User-friendly error messages are displayed if there are issues fetching data from the TMDB API, guiding the user on how to resolve common problems (e.g., missing API key).

Detailed Views (Modal): Click on any movie or TV show card to open a comprehensive modal displaying:

High-resolution poster

Rating

Full plot summary

Associated genres

Release/First Air Date

Embedded Trailer: Watch the official YouTube trailer directly within the modal (if available).

"My Watchlist":

Add movies and TV shows to a personal watchlist.

Remove items from the watchlist.

Your watchlist data is persistently stored in your browser's localStorage.

The watchlist view now displays more detailed information for each item.

Responsive Design: Optimized for a seamless experience across various devices, from mobile phones to large desktop screens.

Responsive Images: Utilizes srcset to load appropriately sized images based on the user's viewport, improving page load performance.

Accessibility Improvements: Includes ARIA attributes for better screen reader support and focus management for modal interactions.

🔧 Technologies Used
HTML5: Structure of the web application.

CSS3 (Tailwind CSS): For modern, utility-first styling and responsive design.

JavaScript (ES6+): Core logic, API interactions, DOM manipulation, and interactive features.

TMDB (The Movie Database) API: For fetching movie and TV show data, including trending lists, search results, and detailed information.

localStorage: For client-side persistence of the "My Watchlist" data.

IntersectionObserver: For implementing efficient infinite scrolling.

🚀 Setup and Installation
To get this project up and running on your local machine, follow these steps:

Clone the Repository (or copy the code):
If this were a repository, you would clone it. For this single HTML file, simply copy the entire code provided into a new file named index.html (or any .html extension).

Obtain a TMDB API Key:

Go to The Movie Database (TMDB) website.

Sign up for a free account.

Once logged in, navigate to your profile settings.

Find the "API" section and request a new API Key (choose the "Developer" type).

Copy your API Key (v3 auth).

Insert Your API Key into the Code:

Open your index.html file in a text editor.

Locate the JavaScript section (within the <script> tags, usually near the end of the <body>).

Find the line:

const API_KEY = 'YOUR_TMDB_API_KEY';

Replace 'YOUR_TMDB_API_KEY' with the actual API key you obtained from TMDB. Make sure to keep the single quotes around your key.

// Example (replace with your actual key):
const API_KEY = 'your_actual_tmdb_api_key_here';

Open in Browser:

Simply open the index.html file in your preferred web browser. You can usually do this by double-clicking the file or dragging it into the browser window.

💡 Usage
Browse Trending: The application will automatically display trending movies upon loading. Use the "Trending Movies" and "Trending TV Shows" buttons to switch between categories.

Search: Type a movie or TV show title into the search bar and click "Search" (or press Enter) to find specific content. Use the dropdown next to the search bar to specify if you're searching for "Movies" or "TV Shows."

Filter by Genre: Use the "All Genres" dropdown to filter the displayed content by a specific genre.

Infinite Scroll: As you scroll down the page, more content will automatically load if available.

View Details: Click on any movie or TV show card to open a modal window with detailed information, including an embedded trailer.

Add to Watchlist: Inside the detail modal or on any card, click the "Add to Watchlist" button to save the item to your local watchlist. If an item is already in your watchlist, the button will change to "Remove from Watchlist."

My Watchlist: Click the "My Watchlist" button in the navigation bar to view all the movies and TV shows you've saved.

Back to Explorer: From the "My Watchlist" view, click "← Back to Explorer" to return to the main content browsing.

🔮 Future Enhancements
Sorting Options: Add options to sort content by popularity, release date, rating, etc.

User Authentication: Implement a backend to allow users to create accounts and save their watchlists across different devices.

Rating/Review System: Allow users to rate and leave reviews for movies/TV shows.

More Detailed Watchlist: Implement more advanced watchlist features like custom lists, watched/unwatched status, etc.

Offline Support: Utilize Service Workers to enable offline access to previously viewed content.

Animations: Add more subtle animations and transitions for a richer user experience.
