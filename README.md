## Flask Application Design for Displaying Recent News Articles

### HTML Files

The application will consist of two main HTML files:

1. **index.html:**
   - This will serve as the main landing page, displaying the list of recent news articles.
   - It will contain a title, a header, and a section to display the news articles.
   - The news articles will be displayed in a list format, with each article featuring its title, a brief description, and a link to the full article.

2. **article.html:**
   - This file will be used for displaying the full content of a specific news article.
   - It will include the article's title, author, date, content, and any associated imagery or videos.

### Routes

The application will contain two main routes:

1. **/:**
   - This is the home route, which will render the **index.html** file.
   - It will retrieve a list of recent news articles from the database or a third-party API and pass them to the template.

2. **article/:id:**
   - This route will render the **article.html** file.
   - It will take an "id" parameter in the URL, which will be used to fetch the specific article from the database or the API.
   - The route will then pass the fetched article data to the template for display.