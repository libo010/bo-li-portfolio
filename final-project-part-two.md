| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Wireframes / storyboards

This storyboard outlines the structure of the final Shorthand story. The goal is to guide a user, whether they are a hardcore skier or just planning a winter weekend, through the landscape of Colorado resorts using data.

#### 1. Part A: The Hook (Introduction)
- **Headline:** "The Colorado Skier’s Dilemma"
- **Sub-headline:** "Finding the perfect balance between deep snow, challenging terrain, and your bank account."
- Visual: High-quality photo of a snowy mountain landscape (wide shot).
- Narrative: "Colorado is world-famous for its winter sports, but visiting can be intimidating and expensive. With tickets ranging from $50 to over $250, how do you know what you are paying for? This guide helps you navigate the trade-offs between cost, snow reliability, and terrain."
- Goal: Set the stage for a "Value Analysis."
  
#### 2. Part B: The Landscape (Interactive Map)
- Goal: Understand geography. Where are these places?
- Design Notes:
    - Encoding: Bubble size = Mountain Size (Vertical Drop), Color = Price.
    - Key Feature: Tooltips that translate "Distance" into "Drive Time" (e.g., "2 hours from Denver"), as this is more useful for students and travelers.

#### 3. Part C: The Value Equation (Scatterplot)
- Goal: Compare resorts directly to find the "Sweet Spot."
- Design Notes:
    - Layout: A scatterplot comparing Price (X-axis) vs. Snowfall (Y-axis).
    - Annotation: A clear shaded box in the top-left labeled "Best Value (High Snow, Low Price)" so users don't have to guess what the chart means.

#### 4. Part D: The Rankings (Bar Charts)
- Goal: Quick answers for specific needs (Cheapest vs. Snowiest).
- Design Notes:
    - Visual: Two simple bar charts.
    - Context: Since a "cheap" resort might be very small, I will color-code the "Cheapest" bars by size (Grey = Small, Green = Big) to keep the data honest.

#### 5. Part E: Conclusion
- Narrative: "There is no 'best' resort, only the right one for your budget and skill level. Use the tools above to decide if you want to pay for luxury or just pay for snow."

#### Shorthand
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
| To test if the encoding (Bubble Size = Vertical Drop; Color = Price) is intuitive to users.      |  "Looking at this map, can you easily identify which resorts are the biggest and which are the most expensive?"    |
|   To determine if the geographic layout and tooltips (implied context) successfully convey "Drive Time" rather than just distance.    |   "If you had to drive from Denver, can you tell how far these places are?"   |
|   To verify if the "Sweet Spot" annotation and the X/Y axis layout allow users to find the 'Best Value' quadrant without guessing.    |  "If you wanted to find the best deal, high snow for a low price, where would you look on this chart?"    |
|  To see if the color-coding (Grey vs. Green) effectively provides context on resort size so the data remains "honest".     |   "Rank these resorts by price. Can you tell which of the cheap resorts are actually small mountains versus big ones?"   |
|  To evaluate if the layout allows for a quick comparison of season longevity.     | "Looking at this timeline, can you quickly tell me who stays open the longest?"    |
| To test if the stacked bar chart accurately conveys the difficulty levels      |  "If you are a beginner, which resort looks safest for you?"    |


## Interview findings

Interview 1: First year grad student with no experience in neither data visualization nor snow sprots 

Interview 2: Master student with some experience snowboarding, have been to a couple of trips near Pittsburgh, beginner level

Interview 3: Female student with some course works experience in data visualization


| Questions               | Interview 1 | Interview 2 | Interview 3 |
|-------------------------|--------------------------------|-------------|-------------|
|   **"Looking at this map, can you easily identify which resorts are the biggest and which are the most expensive?"**    | Found the "Vertical Drop" legend confusing. They asked, "Does a bigger circle mean the mountain is physically wider, or just taller?" They did not immediately equate "Vertical Drop" with "Mountain Size".     |    |  Noted that the color scale (Purple to Yellow) was effective, but felt the distinction between the yellow bubbles (expensive) was clear.  |
|  **"If you had to drive from Denver, can you tell how far these places are?"**     |      |    | Pointed out that the "I-70" and "I-25" road lines were too thin and the red star for "Denver" was somewhat small, making it hard to quickly gauge the route without looking closely.   |
|  **"If you wanted to find the best deal, high snow for a low price, where would you look on this chart?"**     |   Struggled with the term "Pass Affiliation" in the legend, as they did not know what "Ikon" or "Epic" meant.   | "I love the green box. It tells me exactly where to look so I don't have to do the math in my head." This confirmed the "Sweet Spot" design was working.   |    |
|   **"Rank these resorts by price. Can you tell which of the cheap resorts are actually small mountains versus big ones?"**    |   "I almost thought Wolf Creek was the best deal because it's the cheapest, but then I saw it was grey (Small). That stopped me from assuming it was a big resort."   |  Found this chart the easiest to read for a quick decision.  |    |
|  **"Looking at this timeline, can you quickly tell me who stays open the longest?"**    |   "Why is this sorted this way?" The bars appeared random (likely alphabetical) rather than sorted by length. "I have to scan up and down to find the longest bar."   |  Did notice that Arapahoe Basin extends into July, which was a surprise, but agreed the sorting made it harder to compare the middle-tier resorts.  |    |
| **"If you are a beginner, which resort looks safest for you?"**    | "I see the colors, but I don't know what they mean. Is Green easy or is Blue easy?" They lacked the domain knowledge that "Green = Beginner."   |   |  Suggested moving the legend closer to the bars or adding text labels directly onto the color segments.  |

# Identified changes for Part III

| Research synthesis                       | Anticipated changes for Part III                                                |
|------------------------------------------|---------------------------------------------------------------------------------|
| **During the review of the scatterplot chart, P3 pointed out severe over-plotting in the center of the chart. The labels for "Winter Park," "Steamboat," and "Aspen Highlands" overlap with the data points, making the specific names unreadable. This undermines the goal of helping users "navigate the trade-offs" if they cannot identify the specific resorts in the middle cluster.**     |   I will implement a collision-detection algorithm or manually adjust the x,y offsets of the text labels in the code. This ensures that every resort label is legible and distinct from its data point, prioritizing readability over precise geometric centering of the text.   |
|   **P1, who is new to Colorado and unfamiliar with ski geography, struggled with the terminology on the Map and Terrain charts. Specifically, the term "Vertical Drop" on the map legend was ambiguous to them, and the green/blue/black color scheme on the Terrain Analysis chart was not immediately understood as "difficulty levels" without a specific legend explaining ski trail ratings.**    |  For the Map: I will rename the size legend from "Vertical Drop" to "Mountain Size (Height)" or add a clearly visible subtitle explaining that vertical drop equals the skiable height of the mountain. For the Terrain Chart: I will add a direct legend that translates the colors: "Green (Beginner)," "Blue (Intermediate)," and "Black (Expert)."    |
|   **When viewing the timeline, participants noted that the random (or alphabetical) sorting of the bars made it difficult to quickly answer "Who stays open the longest?". P3 noted that this required the user to scan up and down repeatedly rather than seeing a clear pattern.**    |   I will update the sorting logic of the bar chart to order the resorts by Total Days Open (Descending). This will create a "staircase" visual effect, allowing the user to instantly see the top performers (Arapahoe Basin) at the top, facilitating the "quick answers" goal of this section.   |
|  **On the "Drive vs. Dive" analysis, the annotation text for the quadrant labels (e.g., "The Road Trip," "Local Gems") was rendered in a light grey that washed out against the white background. P3 identified this as a visibility issue, noting that it might be unreadable on lower-quality screens or for users with visual impairments.**     |  I will increase the opacity and darken the hex color code for these text annotations. I will also slightly bold the font to ensure these guiding labels are distinct from the grid lines, ensuring the "Sweet Spot" analysis remains the focal point.    |



## References
> Aranoff, J. (2025, April 1). My First Time: Aspen Snowmass. SKI. https://www.skimag.com/ski-resort-life/aspen-snowmass-first-time/

> Arapahoe Basin Ski Resort Review | Colorado. (2025, May 8). PeakRankings. https://www.peakrankings.com/content/arapahoe-basin

> Beginner Ski Terrain in Crested Butte: Your Ultimate Guide | Butte & Co. (2025, July 9). https://www.crestedbutteskirentals.com/blog/beginner-ski-terrain-in-crested-butte-your-ultimate-guide/

> Colorado Ski Resorts. (n.d.). Colorado.Com. Retrieved November 23, 2025, from https://www.colorado.com/colorado-ski-resorts

> Colorado Snow Report | OnTheSnow. (n.d.). Retrieved November 15, 2025, from https://www.onthesnow.com/colorado/skireport

> Epic Ski & Snowboard Passes | Epic Season Pass. (n.d.). Retrieved November 15, 2025, from https://www.epicpass.com/

> Member Resorts—Official Site of Colorado Ski Country USA. (n.d.). Colorado Ski Country USA. Retrieved November 15, 2025, from https://www.coloradoski.com/resorts/

> Multi-Resort Unlimited Ski/Snowboard Season Pass | Ikon Pass. (n.d.). Retrieved November 15, 2025, from https://www.ikonpass.com/

> Silverton Mountain. (n.d.). Silverton Mountain. Retrieved November 23, 2025, from https://silvertonmountain.com/mountain/stats/

> Skiing Purgatory Resort In the San Juan Mountains. (n.d.). OutdoorMaster. Retrieved November 23, 2025, from https://outdoormaster.com/blogs/om-blog/skiing-purgatory-resort-in-the-san-juan-mountains

> Snow and Climate Monitoring Predefined Reports and Maps | Natural Resources Conservation Service. (n.d.). Retrieved November 15, 2025, from https://www.nrcs.usda.gov/resources/data-and-reports/snow-and-climate-monitoring-predefined-reports-and-maps

> Winter Mountain Stats | Copper Mountain Resort. (n.d.). Retrieved November 23, 2025, from https://www.coppercolorado.com/the-mountain/mountain-safety-stats/winter-mountain-stats/

> Wolf Creek Review. (n.d.). PeakRankings. Retrieved November 23, 2025, from https://www.peakrankings.com/content/wolf-creek



## AI acknowledgements
- Grammar Check
- Summerizing in-class brainstorming ideas
- Polishing write-up
- GitHub coding assistance
- Initial Sketch ideas
