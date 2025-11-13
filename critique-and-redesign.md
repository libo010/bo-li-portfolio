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


# The Progress
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
#### Q1: What worked?
A: Using the map to visualize the data was effective, and the color scheme particularly stood out.	
B: The comparison line chart clearly shows how prices changed during the given period.		
D: The store locations are helpful, which are shown on the map.

#### Q2: What didn’t work?
B: The small, zoomed-in maps for the various NYC regions are somewhat confusing, as their intended purpose is unclear.	
C: While the author's intention is to create a heat map for prices, this element is missing from the sketch. It would be easier to implement digitally.	
D: The intention behind comparing pepperoni and plain pizza is unclear.

#### Q3: What needs further investigation?
A: It would be interesting to know if the author has historical pizza price data for individual locations, to see how a single shop's prices have changed over time.			
D: The data visualization is missing a narrative element. The data itself is great, but it didn’t present with a story. For example, it would be useful to explore interesting correlations, such as the relationship between the year and the pizza price.

#### Q4: What might you try next?
A: The size of the dots on the map could relate to the popularity of each pizza store, providing an visual cue for demand.	
B: Using different colors to represent the various types of pizza purchased would make it easy to compare preferences across locations.		
C: A comparison of pizza prices across different boroughs would be very insightful, provided the data is presented clearly.


Based on this critique, my redesign plan is much clearer. I will focus the project for an audience looking for affordable pizza in NYC. The title will be straightforward, like **"NYC's Cheapest Slices: A Price Map by Borough."**
The biggest change will be to the map. I will create a **borough-based heat map using a blue-to-orange gradient**, where blue shows cheaper areas and orange shows expensive ones. This will immediately answer the location and price question. I'll also add a clear legend to show that dots represent pizza types, fixing the color confusion.
For the line charts, I will **separate the data by borough**, creating individual charts for Manhattan, Brooklyn, and Queens to show their unique price trends over time. I'll also update the time scale to quarters for more detail. 


# The End
I chose a dot map as the foundation for my redesign because its primary intent is to answer a straightforward, location-based question: "Where can I find an affordable slice of pizza in New York City?" Unlike a simple chart, a map provides immediate geographical context, allowing users to connect pricing data directly to neighborhoods and boroughs they know. By plotting each pizzeria as a single point on the map, the visualization grounds the abstract concept of "average price" in tangible, specific places, transforming the data from a statistical summary into a practical guide for exploration.

The color coding is central to achieving this clarity. I used a gradient from cool to warm colors—specifically, blue for the most affordable slices transitioning to orange and red for the most expensive. This intuitive color scheme creates an instant visual hierarchy; the "cool" blue dots signal budget-friendly options, while the "warm" red dots act as a visual caution for higher prices. This immediate categorization allows a user to quickly scan the map and identify clusters of affordability or expense. In a fully interactive version, hovering over a dot would reveal the shop's name and exact price, adding a crucial layer of detail to this initial geographic overview.

<div class='tableauPlaceholder' id='viz1763010291180' style='position: relative'><noscript><a href='#'><img alt='Sheet 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress01&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Progress01&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress01&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                
<script type='text/javascript'>                    
	var divElement = document.getElementById('viz1763010291180');                    
	var vizElement = divElement.getElementsByTagName('object')[0];                    
	vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
	var scriptElement = document.createElement('script');                    
	scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
	vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

This monthly data table was created to investigate consistency of the data collection over the eight-year period. While the original visualization effectively showed the overarching annual trend, this table's intent is to reveal the finer, seasonal patterns that might be lost in a yearly average, such as potential price fluctuations during tourist-heavy summer months or slower winter periods. More importantly, its structure immediately exposes a key finding about the data's composition: the complete absence of entries for 2018. This wasn't just a slow year; it was a definitive pause in the project, a "gap year" for pizza logging that the annual line chart would otherwise completely obscure.

To make this table functional and visually communicative, a strategic color scheme would be essential. Each year's column could be shaded with a varying intensity of a single color (like a gradient from light to dark blue) to help the eye track across the wide timeframe. The most critical color choice, however, would be applied to the empty 2018 cells. By filling them with a neutral, contrasting color like light grey, the table would instantly and non-judgmentally highlight the data hiatus, transforming the empty space from a simple absence of information into an informative data point itself. This visual cue ensures the audience understands the break in collection is a documented part of the project's story. **It’s interesting but this graph is not used for the final design. **

<div class='tableauPlaceholder' id='viz1763010466094' style='position: relative'><noscript><a href='#'><img alt='MONTHLY DATA ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress02&#47;Sheet6&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Progress02&#47;Sheet6' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress02&#47;Sheet6&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>               
<script type='text/javascript'>               
	var divElement = document.getElementById('viz1763010466094');   
	var vizElement = divElement.getElementsByTagName('object')[0];      
	vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';     
	var scriptElement = document.createElement('script');               
	scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';   
	vizElement.parentNode.insertBefore(scriptElement, vizElement);       
</script>

I created this bar chart to directly answer the geographic question that the original visualization lacked: how does the average price of a slice compare across New York City's boroughs? The intent was to move beyond a city-wide average and provide a clear, ranked comparison. This format is excellent for this purpose, as the human eye can instantly judge the relative length of the bars, making it immediately obvious that, for instance, Brooklyn and Queens are close in price while Bronx stands out as the most expensive. It efficiently validates the hypothesis that location within the city is a major price determinant. For the color scheme, I chose distinct, contrasting colors for each borough to reinforce their separation as unique data categories. However, I agree that the final result isn't visually appealing; the colors feel extra and don't relate to the data (like price) in a meaningful way. This is a key reason I didn't use it in the final design. A better approach might have been to use a single-color gradient (e.g., light yellow to dark red) where the intensity of the color corresponds to the price, instantly creating a visual hierarchy. 

<div class='tableauPlaceholder' id='viz1763010564644' style='position: relative'><noscript><a href='#'><img alt='Sheet 8 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress03&#47;Sheet8&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Progress03&#47;Sheet8' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress03&#47;Sheet8&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>        
<script type='text/javascript'>                 
	var divElement = document.getElementById('viz1763010564644');      
	var vizElement = divElement.getElementsByTagName('object')[0];            
	vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';      
	var scriptElement = document.createElement('script');                
	scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';         
	vizElement.parentNode.insertBefore(scriptElement, vizElement);           
</script>

The shift from a bar chart to this straightforward text entry box was driven by a clear intent: to prioritize absolute clarity and speed of reading over visual embellishment. This minimalist approach strips away all graphical elements, presenting the core data, borough names and their corresponding average prices, in the most direct way possible. The goal is functional efficiency; a viewer can instantly locate a specific borough and its precise price without interpreting bar lengths, colors, or axis scales. This format excels as a quick-reference legend or a summary statistic, serving an audience that needs the raw numbers without any decorative overhead.

<div class='tableauPlaceholder' id='viz1763010639928' style='position: relative'><noscript><a href='#'><img alt='Sheet 9 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress04&#47;Sheet9&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Progress04&#47;Sheet9' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress04&#47;Sheet9&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>            
<script type='text/javascript'>                   
	var divElement = document.getElementById('viz1763010639928'); 
	var vizElement = divElement.getElementsByTagName('object')[0];  
	vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';  
	var scriptElement = document.createElement('script');        
	scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';  
	vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

These two visualizations represent a significant step toward a dynamic and user-driven final design. The first, an interactive line chart, was created to address the original critique's lack of a clear narrative. By breaking the annual data into quarterly points, it reveals more granular trends and seasonal fluctuations that the yearly average completely hid. The inclusion of a filter for "Pepperoni" and "Plain" styles, combined with a year selector, allows a user to actively investigate specific questions, such as whether the price gap between the two types widened after 2020. This interactivity transforms the chart from a static statement into a tool for personal exploration, directly answering the feedback that the data needed a stronger storytelling element.
The second visualization, a price range chart filtered by borough, serves a dual purpose. Firstly, it fulfills the core redesign goal of geographic separation, finally allowing for a direct comparison of pricing landscapes across the Bronx, Brooklyn, Manhattan, Queens, and Staten Island. The interactive borough filter is crucial here. Secondly, the price slider is the key feature; it empowers the user to set their own budget and immediately see which neighborhoods fall within it. This directly caters to the identified audience of cost-conscious consumers. The color choice for the range—likely a gradient from a cool color for $1.00 to a warm color for $6.53—would provide an intuitive, instant read on the spectrum of affordability within each selected borough, making the data both accessible and actionable.

<div class='tableauPlaceholder' id='viz1763010697742' style='position: relative'><noscript><a href='#'><img alt='PRICES OF PEPPERONI vs. PLAIN ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress05&#47;PriceOverTime&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Progress05&#47;PriceOverTime' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress05&#47;PriceOverTime&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>             
<script type='text/javascript'>    
	var divElement = document.getElementById('viz1763010697742');         
	var vizElement = divElement.getElementsByTagName('object')[0];   
	vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';   
	var scriptElement = document.createElement('script');              
	scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';    
	vizElement.parentNode.insertBefore(scriptElement, vizElement);             
</script>

<div class='tableauPlaceholder' id='viz1763010715637' style='position: relative'><noscript><a href='#'><img alt='PRICES BY ZIP CODE ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress06&#47;PricebyZipcode&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Progress06&#47;PricebyZipcode' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Pr&#47;Progress06&#47;PricebyZipcode&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>         
<script type='text/javascript'>                 
	var divElement = document.getElementById('viz1763010715637');       
	var vizElement = divElement.getElementsByTagName('object')[0];   
	vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';      
	var scriptElement = document.createElement('script');                 
	scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js'; 
	vizElement.parentNode.insertBefore(scriptElement, vizElement);             
</script>

My redesigned data visualization, "NYC's Cheapest Slices: A Price Map by Borough," aims to transform the original dataset from a personal log into a practical, interactive tool for a clearly defined audience: budget-conscious pizza enthusiasts exploring New York City. I selected a multi-component dashboard specifically to tell a more complete and accessible story than the original single chart. The design does three key things differently: First, it immediately grounds the user with a clear geographic breakdown by providing average prices per borough, something the original visualization completely omitted. Second, it introduces interactivity through filters for borough, year, and price range, empowering the user to ask and answer their own questions, such as how prices in Brooklyn evolved compared to Manhattan. Finally, it corrects the original's visual ambiguity by using distinct colors and clear legends to separate pepperoni and plain slice trends, ensuring the data is interpreted correctly at a glance.
The visualization now effectively shows three interconnected narratives. The central map provides a spatial overview of affordability. The interactive line chart reveals the temporal trend, showing not just that prices rose, but how the "pepperoni pizza" has fluctuated over time. The borough summary and zip code filter work in tandem to answer the most pressing user question: "Where can I find a slice in my budget?" By making these elements interactive and interconnected, the redesign moves beyond a static fun fact to become a dynamic exploration of cost, location, and time, ultimately providing a much richer and more useful insight into the economics of NYC's pizza culture.

<div class='tableauPlaceholder' id='viz1763010794728' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;NY&#47;NYCSCHEAPESTSLICESAPRICEMAPBYBOROUGH&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='NYCSCHEAPESTSLICESAPRICEMAPBYBOROUGH&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;NY&#47;NYCSCHEAPESTSLICESAPRICEMAPBYBOROUGH&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>           
<script type='text/javascript'>               
	var divElement = document.getElementById('viz1763010794728');  
	var vizElement = divElement.getElementsByTagName('object')[0];   
	vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';     
	var scriptElement = document.createElement('script');                    
	scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';     
	vizElement.parentNode.insertBefore(scriptElement, vizElement);             
</script>


# Reference:
Andy Kriebel. (2023, January 30). New York City Pizza Slices - #MakeoverMonday 2023 Week 5. YouTube. https://www.youtube.com/watch?v=bdFW6gnbBik&list=PLX-uPHRG0cLb697Ie-ZGSObRLLNhxzJGK&index=56
Quigley, L. (2023). NYC Slice – Liam Quigley. Elkue.com. https://elkue.com/nyc-slice/

# AI acknowledgements:
- Grammar Check
- Summerizing in-class brainstorming ideas
- Polishing write-up
- GitHub coding assistance 






