# The Beginning

I decided to work on NYC pizza slices data set. I was drawn to this visualization because it documents an interesting, daily purchase with the rigor of a long-term study. The author didn't just track prices; they compiled a dataset from 464 specific slices over eight years, explicitly excluding dollar slices to refine the average. This approach transforms a simple observation into a concrete record of urban life. As someone familiar with New York City and its food culture, seeing the steady climb from $2.52 to $3.00 for a plain slice validates a feeling I’ve had that the city's most basic needs are dramatically changing. The most compelling details are those observations, like the note on the declining amount of sauce, which suggests a downgrade of quality that a price line alone can't show. It’s a personal archive that uses data to tell a very human story about cost, value, and the slow evolution of a city's character through its food.

Here’s a link to the original data visualization: https://elkue.com/nyc-slice/
& 
Here're some screenshots of the original data viz.

<img width="1386" height="858" alt="Screenshot 2025-11-12 233700" src="https://github.com/user-attachments/assets/e0f3d9e5-633c-4a8d-98ec-564f73685591" />
Figure 01

<img width="1586" height="830" alt="Screenshot 2025-11-12 233706" src="https://github.com/user-attachments/assets/81bd8b41-7c77-4393-b5a3-b386b5bb7a85" />
Figure 02

<img width="1675" height="704" alt="Screenshot 2025-11-12 233712" src="https://github.com/user-attachments/assets/e34dde72-add7-4d66-9945-b316c68855aa" />
Figure 03


# The Critique 
Based on Few, Stephen. “Data Visualization Effectiveness Profile,” 2017, 11.
http://www.perceptualedge.com/articles/visual_business_intelligence/data_visualization_effectiveness_profile.pdf

Here's how I rated the original viz:
<img width="977" height="959" alt="Screenshot 2025-11-12 234310" src="https://github.com/user-attachments/assets/fec41176-9428-4b7c-a419-51e31436b344" />
<img width="987" height="1014" alt="Screenshot 2025-11-12 234339" src="https://github.com/user-attachments/assets/bcf66cb8-1620-4f85-9953-4cb3e68077ac" />


### Describe your overall observations about the data visualization here.  What stood out to you?  What did you find worked really well?  What didn't work well?
The author's chart does a great job of showing how pizza slice prices have changed over the years, which is really helpful for getting a quick overview of the data. However, the data combines different NYC regions like Manhattan, Queens, and Brooklyn into one graph. Since location could be a major factor in pricing, it might be better to have separate graphs for each borough to make comparisons easier.
Also, the color choices in the visualizations are a bit confusing. At first, I thought the colors on the map represented price levels, with red meaning a higher cost. But they actually represent different types of pizza, like Pepperoni and Plain. Adding a legend to the map would make this much clearer.

### Who is the primary audience for this tool?  Do you think this visualization is effective for reaching that audience?  Why or why not?
The tool's intended audience feels ambiguous. It could be for someone seeking a pizza place recommendation in NYC, but it lacks the necessary data, like recent reviews or specific rankings, to properly support that purpose. Alternatively, it might be a data visualization for analyzing NYC pizza prices over time. While it has enough pricing data, the presentation is somewhat unorganized. The audience might struggle to find what they need because data from different years is mixed together. For example, My PIE Pizzeria is ranked as the 3rd most expensive overall, but the price used is from 2016, which may not be relevant for someone looking for current information in 2025.
	
### Based on your critique, what do you think you'll try to focus on in your redesign?   Any ideas or inspiration for how you can make a better data visualization?  What are you excited to try next?
For my redesign, I plan to focus first on separating the data by region. I'll start with the three main regions, Manhattan, Queens, and Brooklyn, and then potentially break them down into smaller neighborhoods. For each area, I'll calculate the average slice price to establish a clear baseline.
Visually, I'll use distinct color schemes for the line chart and the map. I'll keep the line chart colors the same, using red for pepperoni and yellow for plain cheese. To show more granular trends, I'll adjust the time scale from years to quarters.
Finally, I'll create a layered map visualization. The base layer will be a heat map showing the general price range across different neighborhoods, with colors indicating high and low prices. I’m thinking using blue to orange gradient color. On top of this, I'll plot individual pizza shops for specific, detailed data.


# The Sktech & Interviews
Here's my sktech:
![2025-11-10 140509](https://github.com/user-attachments/assets/f729f7a2-e9ae-4fe8-9f7e-fed3717559b6)

### Test the solution
Because of limited time and discussion in class, I didn't get detailed feedback from every participant for each question I had prepared.

Person A:
Healthcare Analysis student with some course works experience in data visualization.
Person B:
Psychology student with a concentration on product research. No data visualization experience.
Person C:
Information System student. No data visualization experience.
Person D:
MSPPM student with data visualization experience and have worked on student council and dealt with data. 

For my script I used the in-class handout questions for my interview.



# The End
