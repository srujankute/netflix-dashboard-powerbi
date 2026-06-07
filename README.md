# 📊 Netflix Catalog Analysis & Audience Engagement Dashboard

## 1. About the Project
This project is an interactive, two-page Power BI dashboard designed to analyze Netflix's movie and TV show catalog from **1953 to 2022**. The main goal was to take raw data from IMDb, clean it up, and build a report that helps us understand how Netflix's content strategy has shifted over the years and what kind of content drives the most audience attention.

* **Tools Used:** Power BI Desktop, Power Query (for data cleaning), and DAX (for custom metrics).
* **The Dashboard Structure:** * **Page 1 (Executive Summary):** A high-level overview of total volume, historical trends, and average ratings.
  * **Page 2 (Deep-Dive Analysis):** A closer look at quality vs. popularity, the movie-to-show mix shift, and audience engagement metrics.

---

## 2. Questions This Dashboard Answers
I built this project to tackle specific, real-world questions about the entertainment streaming space:
* Is Netflix focusing more on TV shows or movies now compared to the past?
* Do age ratings (like PG-13, R, or TV-MA) have a visible impact on user scores?
* Which types of content pull in the highest volume of audience votes?
* Did the overall quality of content drop when production volume suddenly spiked?

---

## 3. Custom Metrics Created (DAX Formulas)
To uncover deeper insights, I moved beyond standard averages and created two custom metrics using DAX:

### Metric 1: User Engagement (Avg Votes Per Title)
A movie might have a high 9.0 rating but only 10 total votes, which can skew our analysis. To find out what audiences are *actually* watching and interacting with, I created this formula:

$$\text{Avg Votes Per Title} = \frac{\text{Total IMDb Votes}}{\text{Total Number of Titles}}$$

This metric helps us see which age certifications or categories command the largest active audience footprint.

### Metric 2: Popularity-Weighted Score
To find the definitive "all-time best" titles on the platform, I created a combined impact score using both votes and ratings ($Votes \times Rating$). This allows us to properly rank blockbuster titles that manage to keep an incredibly high user score despite being reviewed by millions of people, separating them from low-volume titles.

---

## 4. Dashboard Visuals & Layout
Below are screenshots of the completed dashboard pages showing the finalized layout and metrics:

### Page 1: Executive Summary
*(Tip: Upload your Page 1 screenshot to GitHub and paste the image link right below this line)*
* Add your image tag here: `![Executive Summary](your_image_link_1.png)`

### Page 2: Deep-Dive Analysis
*(Tip: Upload your Page 2 screenshot to GitHub and paste the image link right below this line)*
* Add your image tag here: `![Deep-Dive Analysis](your_image_link_2.png)`

---

## 5. Main Insights Discovered

* **The Pivot to TV Shows:** Early in the historical timeline, Netflix's catalog was dominated almost entirely by movies. However, over the last 15–20 years, TV series have steadily captured a massive percentage of the overall catalog share. Netflix clearly shifted its long-term strategy toward episodic content.
* **The Engagement Winner:** While family-friendly and TV-rated titles maintain highly competitive average rating scores, **R-rated and PG-13 content** dominates when it comes to audience interaction, pulling in exponentially higher user votes per title.
* **Quantity vs. Quality Trade-off:** The platform hit a massive production peak around 2020, adding a historic number of titles to the catalog. Interestingly, right at this peak, the average IMDb rating trajectory shows a slight cooling trend, highlighting the challenge of keeping quality control perfect during rapid volume expansion.

---

## 6. Dashboard Design Choices
The layout was designed with data-storytelling and usability in mind:
* **Top-Left KPI Cards:** High-level summaries (**Total Titles, Average Rating, Total Votes**) are placed in the top-left area because that is naturally where the human eye looks first when opening a report.
* **Timeline Alignment:** Stacking the line charts vertically on the right allows a viewer to scan across the exact same X-axis timeline seamlessly to compare volume, ratings, and runtime trends instantly.
* **Color Themes:** A cohesive wine-red/maroon color palette was used across both pages to give the report a clean, professional, and unified aesthetic.
