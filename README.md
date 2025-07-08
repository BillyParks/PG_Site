# ParadiseGrove.com - A Travel Affiliate Website

This repository contains all the files and articles for the unofficial travel guide to Burleigh Heads, Gold Coast, Australia. The website is built with simple HTML and Tailwind CSS and is hosted using GitHub Pages with a custom domain.

---

### Project Links

* **Live Site:** [https://www.paradisegrove.com](https://www.paradisegrove.com)
* **GitHub Pages Mirror:** [https://billyparks.github.io/PG_Site/](https://billyparks.github.io/PG_Site/)
  
  The custom domain points directly to the GitHub Pages build. The mirror URL remains available for reference.

### Project Goal

The primary goal of this website is to become a high-quality, trustworthy, and SEO-optimized resource for tourists planning a trip to Burleigh Heads. The secondary goal is to monetize this traffic through affiliate partnerships with accommodation, tour, and transportation providers.

### Technology Used

* **HTML5:** For the basic structure of all pages.
* **Tailwind CSS:** For all styling, included via a CDN link in each HTML file.
* **GitHub Pages:** For hosting the static website.
* **Google Analytics:** The GA tag lives in `analytics.html`, which each page fetches.

### File Structure

The site is organized into category folders to keep the content neat and create clean URLs.
/ (root)
|-- index.html           (The homepage)
|-- analytics.html       (Google Analytics loader)
|-- /accommodation/
|   |-- best-family-stays.html
|-- /food/
|   |-- (future articles go here)
|-- /activities/
|   |-- (future articles go here)
|-- README.md            (This file)

### Content Creation Workflow

To maintain consistency and quality, all new articles are created using the following process:

1.  **Choose a Topic:** Select the next article to be written from our content plan.
2.  **Use the SEO Prompt Template:** Fill out the agreed-upon template to define the Primary Keyword, Secondary Keywords, Title, and Goal.
3.  **Generate the Article:** Use our AI assistant to generate the complete, SEO-optimized HTML file for the article.
4.  **Create the File:** Create a new `.html` file in the appropriate category folder (e.g., `/food/top-cafes.html`).
5.  **Link the Article:** Edit the `index.html` homepage (or another relevant page) to add a link to the new article.
6.  **Load Analytics:** Add a script that fetches `analytics.html` and inserts it into the `<head>` of the page. This ensures the Google Analytics tag is loaded.
7.  **Use Root-Relative Paths with `{{ site.baseurl }}`:** Reference images and internal links using the Jekyll `baseurl` variable (e.g., `{{ site.baseurl }}/images/pic.jpg` or `{{ site.baseurl }}/about.html`) so links work on GitHub Pages and the custom domain.

### Project Roadmap & To-Do List

- [x] Set up GitHub repository and publish initial `index.html`
- [x] Create first article page for "Family-Friendly Accommodation"
- [x] Link homepage to the new article
- [ ] Write article for "Top Things To Do"
- [ ] Write article for "Food & Drink Guide"
- [ ] Apply to Awin affiliate network once 5-10 articles are live
- [ ] Set up the custom `paradisegrove.com` domain after affiliate approval
