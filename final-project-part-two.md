| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Wireframes / storyboards

This storyboard outlines the structure of the final Shorthand story. The goal is to guide a user, whether they are a hardcore skier or just planning a winter weekend, through the landscape of Colorado resorts using data.

### 1. Part A: The Hook (Introduction)
- **Headline:** "The Colorado Skier’s Dilemma"
- **Sub-headline:** "Finding the perfect balance between deep snow, challenging terrain, and your bank account."
- Visual: High-quality photo of a snowy mountain landscape (wide shot).
- Narrative: "Colorado is world-famous for its winter sports, but visiting can be intimidating and expensive. With tickets ranging from $50 to over $250, how do you know what you are paying for? This guide helps you navigate the trade-offs between cost, snow reliability, and terrain."
- Goal: Set the stage for a "Value Analysis." 
### 2. Part B: The Landscape (Interactive Map)
- Goal: Understand geography. Where are these places?
- Design Notes:
    - Encoding: Bubble size = Mountain Size (Vertical Drop), Color = Price.
    - Key Feature: Tooltips that translate "Distance" into "Drive Time" (e.g., "2 hours from Denver"), as this is more useful for students and travelers.
### 3. Part C: The Value Equation (Scatterplot)
- Goal: Compare resorts directly to find the "Sweet Spot."
- Design Notes:
    - Layout: A scatterplot comparing Price (X-axis) vs. Snowfall (Y-axis).
    - Annotation: A clear shaded box in the top-left labeled "Best Value (High Snow, Low Price)" so users don't have to guess what the chart means.
### 4. Part D: The Rankings (Bar Charts)
- Goal: Quick answers for specific needs (Cheapest vs. Snowiest).
- Design Notes:
    - Visual: Two simple bar charts.
    - Context: Since a "cheap" resort might be very small, I will color-code the "Cheapest" bars by size (Grey = Small, Green = Big) to keep the data honest.
### 5. Part E: Conclusion
- Narrative: "There is no 'best' resort, only the right one for your budget and skill level. Use the tools above to decide if you want to pay for luxury or just pay for snow."

### Shorthand
[Shorthand Draft Presentation](https://preview.shorthand.com/jmYWTXrMZ7sy5ori)

# User research 

## Target audience
#### 1. Readers: 
Young adults, students, Colorado residents and visitors interested in travel or outdoor activities. This audience is broader than just "skiers & snowboarders", it includes anyone looking to plan a trip or understand the local landscape. 

#### 2. Interview Participant Profiles
Since the target audience is broad, my plan is to select classmates with different levels of experience and skill levels in order to get the idea of the spectrum of real-world users.

|    Person     | Profile |  Role |
|-------------------------|--------------------------------|-------------|
| Person 1 (The Novice) | New to Colorado. Has never skied and is unfamiliar with resort geography.       |   Tests for barriers and basic accessibility.      |
|     Person 2 (The Casual User)    |   Casual skier, skis 1-2 times a year on a budget.     |   Tests the "Value Analysis" tools and price sensitivity.          |  
|    Person 3 (The Critic)      |    Data Science student with design experience.       |   Tests for visual clarity, color logic, and layout flow.     |  

## Interview script
**Research Goal**

To evaluate the clarity and accessibility of the data visualizations. Since the audience includes potential visitors who may not be ski experts, the research focuses on whether the charts are understandable without prior domain knowledge.


| Goal | Questions to Ask |
|------|------------------|
| To evaluate if the visualizations are intuitive without heavy explanation.    |    "Looking at this map, can you point to the resorts that are the most expensive? How did you know?"         |
|  To assess "Data Literacy." Can the user interpret the X and Y axes simultaneously to find a specific data point (High Snow + Low Price)?    |   "Look at this chart comparing 'Price' (bottom) and 'Snow' (left). If you wanted to save money but still see a lot of snow, which area of the chart would you look at?"               |
|  To identify domain-specific language (e.g., "Vertical Drop," "Skiable Acres") that creates barriers for a general audience.    |     "Are there any words, labels, or titles on these charts that you find confusing or unfamiliar?"     |
| To determine if the sequence of visualizations tells a coherent story or feels disjointed.     |    "Is there any information missing that you feel you would need to see before making a decision?"     |


## Interview findings

Interview 1: First year grad student with no experience in neither data visualization nor snow sprots 

Interview 2: Master student with some experience snowboarding, have been to a couple of trips near Pittsburgh

Interview 3: Female student with some course works experience in data visualization


| Questions               | Interview 1 | Interview 2 | Interview 3 |
|-------------------------|--------------------------------|-------------|-------------|
|**"Looking at this map, can you point to the resorts that are the most expensive? How did you know?"** | "I can tell the dark blue ones are expensive. But the size... I'm confused if a big bubble means a scary mountain."    |   "I see the big bubbles are the major resorts. But you list 'Distance' in miles. That's annoying because 60 miles in the mountains takes way longer than 60 miles on the plains. I need to know drive time."          |    "The color scale is intuitive. The bubbling size is good, but maybe add a note that size = height, not width."     |
| **"Look at this chart comparing 'Price' (bottom) and 'Snow' (left). If you wanted to save money but still see a lot of snow, which area of the chart would you look at?"** |       "I see the 'Best Value' box you drew. That helps a lot. Without that, I'd probably have to stare at the axes for a while to figure out that 'up and left' is good." |  "I'd click the top left, Wolf Creek. Lots of snow, cheap ticket. But wait, why is it so cheap? Is it far away?" |     "This is the strongest chart. The annotation is key. It guides the eye immediately to the insight."  |
|   **"Are there any words, labels, or titles on these charts that you find confusing or unfamiliar?"**  |   “The legend says 'Vertical Drop.' Does that mean how steep the slope is? Or how tall the mountain is?” |   "I know what acres are, but maybe explain if 500 acres is big or small? I don't have a frame of reference."  |             |
|  **"Is there any information missing that you feel you would need to see before making a decision?"**  | "I like starting with the map. It helps me orient myself before seeing the numbers." |   "The bar charts at the end are my favorite. I just want the list of 'Cheapest' so I can book it. Maybe put a 'Top 5' summary at the top?"   |   "The flow works. It goes from 'Where?' (Map) to 'Which?' (Scatter) to 'What?' (Rankings)."    |

# Identified changes for Part III

| Research synthesis                       | Anticipated changes for Part III                                                |
|------------------------------------------|---------------------------------------------------------------------------------|
| **Misunderstanding of "Vertical Drop":** P1 interpreted "Vertical Drop" as "Steepness" rather than mountain height. This caused confusion about the map's bubble size encoding, making them fear "big" bubbles meant "too difficult." | Rename Legend & Add Subtitle: I will change the map legend title from "Vertical Drop" to "Mountain Height". Or Keep both. I will also add a small subtitle explaining: "Measured from base to peak indicates the vertical size of the resort." |
|   **"Miles" is a poor proxy for Travel Effort:** P2 noted that measuring distance in miles is misleading for mountain travel (e.g., 60 miles on I-70 can take 3+ hours). This metric failed to help them plan a realistic trip.            |       Switch to Traveling Time: I will replace the Dist_Denver_Miles metric in the tooltips with Travel_Time_Min (Average Drive Time). The tooltip will now read: "Approx. Drive from Denver: [X] Hours."   |
|   **Distrust of Low Price Points:** When viewing the "Cheapest Resorts" bar chart, P2 questioned the quality of the lowest-priced options (e.g., "Is this $59 resort just a tiny hill?"). The simple bar chart lacked context on value/size.  |   Add Contextual Color Coding: I will modify the "Cheapest Resorts" bar chart to include a color code for Resort Size. Green Bars: Large Resorts (>1,000 acres). Grey Bars: Small Hills (<500 acres). This helps users distinguish between a "great deal" and a "small hill." |
|   **Effectiveness of Annotations:** All participants praised the "Best Value" text box on the scatterplot. P1 noted they would have struggled to interpret the chart without it.  |  Standardize Annotations: I will ensure that all final charts in Tableau include explicit text annotations (e.g., "Best Value Zone," "Most Expensive," "Hidden Gem") rather than relying on the user to read the axes alone. |



## References
> Colorado Snow Report, OnTheSnow. (n.d.). Retrieved November 15, 2025, from https://www.onthesnow.com/colorado/skireport

> Epic Ski & Snowboard Passes, Epic Season Pass. (n.d.). Retrieved November 15, 2025, from https://www.epicpass.com/

> Member Resorts - Official Site of Colorado Ski Country USA. (n.d.). Colorado Ski Country USA. Retrieved November 15, 2025, from https://www.coloradoski.com/resorts/

> Multi-Resort Unlimited Ski/Snowboard Season Pass, Ikon Pass. (n.d.). Retrieved November 15, 2025, from https://www.ikonpass.com/

> Snow and Climate Monitoring Predefined Reports and Maps, Natural Resources Conservation Service. (n.d.). Retrieved November 15, 2025, from https://www.nrcs.usda.gov/resources/data-and-reports/snow-and-climate-monitoring-predefined-reports-and-maps


## AI acknowledgements
- Grammar Check
- Summerizing in-class brainstorming ideas
- Polishing write-up
- GitHub coding assistance
- Initial Sketch ideas
