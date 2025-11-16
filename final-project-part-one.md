| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |


# Outline
### High-level summary
This project will investigate how ski resorts in Colorado differ on three practical dimensions: snowfall, direct cost to visit (lift tickets or daily cost), and perceived/value metrics that combine snow and cost. I want to move beyond simple rankings and show the trade-offs a skier faces: a very snowy small hill may be cheap but have limited terrain; a premier resort may charge more but offer terrain variety and reliable snowmaking. The visualization package will let viewers answer concrete questions, such as “Where is the cheapest resort near Denver?” “Which resort has historically received the most snow?”, and explore the relationships (higher elevation means more snow, but also different price tier).

The analysis will use publicly available data where possible and link resort-level metadata (location, vertical drop, lift count) to objective snow measurements (OpenSnow / NOAA) and to price information scraped or recorded from resort or aggregator sites. Visual storytelling will start with a map and simple comparisons, then let users drill into chosen resorts and compare normalized metrics (price per vertical foot, snowfall per operating day). The narrative arc goes from orientation (map & simple facts) to insight (where good snow and low-cost overlap), to decision support (filters for travel distance, budget, and skill level).


### Project structure
1.	Intro & user stories
      1. “This interactive report helps skiers find Colorado resorts that maximize snow, minimize cost, or balance both.”
      2. User stories:
         - As a budget skier, I want to find resorts with the lowest daily lift cost within a 2-hour drive of Denver.
         - As a powder hunter, I want to find resorts that historically have the greatest average seasonal snowfall.
         - As a trip planner, I want to compare a few resorts on snowfall, price, and elevation so I can pick the best compromise.
2.	Exploratory layer - map + small multiples
      1. Interactive state map with resort points sized by vertical drop and colored by a chosen metric (e.g., average snowfall, daily price).
      2. Sidebar filters (distance from a selected city, price range, snow threshold).
3. Comparative layer - charts
      1. Scatterplot: average seasonal snowfall vs. average daily lift price (points sized by skiable acres).
      2. Bar charts: cheapest vs. most expensive resorts, snowiest vs. least snowy.
      3. Matching the Mountain to the Skier. Use data on terrain difficulty (e.g., % beginner, intermediate, expert) to guide different skier types. For instance, Aspen is a haven for experts, while Buttermilk is ideal for beginners.
4. Conclusion
      1. Conclude with clear, data-backed recommendations for different user personas (e.g., "The Budget-Conscious Expert," "The Powder-Hunting Family"). The final takeaway is that Colorado has a perfect mountain for everyone.


# Initial sketches
1. Colorado Ski Resorts - Snow Map View
- A state map with each resort represented as a bubble. The size of the bubble corresponds to size of the resort, and the sidebar includes filters such as drive time (e.g., within 6 hours), snwo fall amount, pass type, or price range.
- Purpose: This sketch introduces the viewer to the overall landscape, showing where resorts are located and how snow varies across the state.

2. Seasonal Snowfall vs. Daily Lift Price Scatterplot
- A scatterplot comparing snowfall (y-axis) and average lift ticket price (x-axis). Each point represents a resort.
- Purpose: Useful for finding the “best value”, resorts with high snow but lower cost stand out visually as upper-left points.

3. Cheapest vs. Snowiest Resorts (Side-by-side Bar Charts)
- Two simple ranked lists. One shows the lowest-priced resorts, the other shows the resorts with the highest average snowfall.
- Purpose: A clean and quick way to compare rankings and contrast how resort price does not always correlate with snowfall.

4. Resort Detail Card
- A profile layout for a single resort: elevation, vertical drop, skiable acres, and average snowfall, plus a small line chart showing 10-year snowfall history.
- Purpose: Acts as the detail view in the final project, giving viewers context for each resort’s characteristics and performance over time.

<img width="1000" alt="Initial Sketches Ideas_01" src="https://github.com/user-attachments/assets/48587b71-1e1a-4acb-bfa1-27d8c350bdd8" />

5. “Most Valuable Resort?” Concept Illustration
- A simple mountain sketch with symbolic markers representing resorts at different altitudes and values.
- Purpose: This could serve as the opening visual for the story, posing the essential question (“Which resort gives the best value?”) before diving into the data.

6. Snowiest Resort? Horizontal Bars
- A focused bar chart ranking snowfall totals.
- Purpose: A straightforward visual that immediately communicates which resorts get the most snow.

7. Map + Comparison Panel
- Left side: a resort map with dot markers.
- Right side: a comparison metric block (e.g., snowfall, price, or acres) represented by a shaded chart area.
- Purpose: Shows a two-panel layout combining geographic context with numeric comparison to help viewers interpret both spatial and metric-based information together.

8. Top 5 Ski Resorts (Rank List + Mini Chart)
- A ranking from 1 to 5 on a chosen metric (value, snowfall, price efficiency), paired with a small thumbnail chart summarizing the metric distribution.
- Purpose: Useful as part of the insights section, highlighting best-in-category resorts.

<img width="1000" alt="Initial Sketches Ideas_02" src="https://github.com/user-attachments/assets/acae5fde-4c6a-4c86-a1de-90252a38425f" />

# The data
> A couple of paragraphs that document your data source(s), and an explanation of how you plan on using your data. 

Text here...

> A link to the publicly-accessible datasets you plan on using, or a link to a copy of the data you've uploaded to your Github repository, Box account or other publicly-accessible location. Using a datasource that is already publicly accessible is highly encouraged.  If you anticipate using a data source other than something that would be publicly available please talk to me first. 

| Name | URL | Description |
|------|-----|-------------|
|      |     |             |
|      |     |             |
|      |     |             |

# Method and medium
> In a few sentences, you should document how you plan on completing your final project. 

Text here...

## References
_List any references you used here._

## AI acknowledgements
- Grammar Check
- Summerizing in-class brainstorming ideas
- Polishing write-up
- GitHub coding assistance
- Initial Sketches Ideas
