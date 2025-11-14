| [home page](https://zenbeam.github.io/shubham-dataviz/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Critique by Design: Drug Harm Visualization

## Step one: the visualization

I selected a data visualization published by The Economist titled **"Paying Through the Nose"**, which shows the relative harm of different drugs in Britain. The graphic comes from a 2019 article exploring which substances cause the most harm when accounting for impacts on both users and others. I picked this visualization because I noticed that the topic itself is meaningful and I wanted to see whether the design helped or hindered the message. This writeup started from the course template for the Critique by Design assignment. 

**Original visualization**  
![Original Economist Graphic](https://www.economist.com/cdn-cgi/image/width=960,quality=80,format=auto/sites/default/files/images/2019/06/articles/main/20190629_woc294.png)

[Article](https://www.economist.com/graphic-detail/2019/06/25/what-is-the-most-dangerous-drug)

[Data source](https://data.world/makeovermonday/2025w36-drug-harms-in-the-uk)


I selected this chart because I feel the subject is socially important, and I wondered whether a redesign could help general readers see the key insight more clearly: that alcohol causes more total harm than substances often assumed to be more dangerous.

---

## Step two: the critique

I completed the critique form and reflected on what worked and what did not. Below is a concise summary of my thoughts.

- I noticed that the chart makes it easy to see the overall ranking, especially alcohol at the top.  
- I also noticed that the six tiny stacked segments made the bars hard to read and I found myself checking the legend repeatedly.  
- I think the title did not tell me what to take away and the subtitle created some ambiguity about the scale.  
- I wondered why the axis went to 80 when the chart said "out of 100".  
- I felt the main storyline got buried under the amount of detail.

These early impressions shaped the direction of my redesign.

---

## Step three: sketch a solution

For my first sketch, I stayed close to the original chart structure and treated it as a clean up pass rather than a complete redesign.

![First sketch](/drug-harm-first-sketch.png)

In this version, I:

- Moved and simplified the legend so it is easier to connect categories to the bars.  
- Adjusted the color palette so shades within "harm to users" and "harm to others" are easier to distinguish.  
- Added numeric labels on each segment so readers can compare the individual harm components without guessing.  
- Cleaned up spacing and typography to make the chart feel more intentional and legible.

At this point I still kept all six harm categories, but I started to feel that even a prettier stacked bar might not fully solve the cognitive overload problem.

---

## Step four: test the solution

### User interviews

I prepared a short script to focus on broad comprehension and first impressions. The table below is adapted from the HTML feedback file and summarizes responses from three different participants. 

### Interview feedback

| User persona | What do you think this is? | What is this telling you? | Anything surprising or confusing? | Intended audience? | What would you change? |
|-------------|---------------------------|---------------------------|----------------------------------|---------------------|-------------------------|
| Student, mid 20s, Marketing Analytics | Comparison chart of drugs and harm factors | Ranking drugs by harm, alcohol highest | Six color shades hard to tell apart; unclear what the title means | Policy makers or researchers | Group harms into "Harm to Users" and "Harm to Others" |
| MSPPM student, Data Scientist | Horizontal bar chart ranking harm | Alcohol leads, psychedelics lowest | Empty space on the right; redundant drugs | Policy analysts, researchers, journalists | Reduce number of drugs shown |
| Early 20s student, tech twitter user | Data viz about drug harm with stacked bars | Alcohol more harmful than many illegal drugs | Title and subtitle unclear; too many tiny segments | Harm reduction advocates or academic readers | Simplify to two categories only |

### Synthesis

A few patterns stood out to me:

- Everyone struggled with the six segment stacked bars and wanted simplification.  
- Everyone noticed alcohol being highest but felt the narrative was unclear.  
- Two people felt the number of drugs shown was overwhelming.  
- All three suggested collapsing categories to "harm to users vs harm to others".

From this feedback, I realized the redesign should focus on clarity, simplicity, and narrative framing. It also convinced me that I should move beyond a refined stacked bar and try a different chart type.

---

## Step five: build the solution

### Final redesign

For the final visualization, I pivoted from the incremental sketch and built a new view using a diverging bar chart. I aggregated the six detailed harm categories into two totals: **Harm to users** and **Harm to others**.

![Final diverging chart](/drug-harm-final-diverging.png)

### What I changed and why

- I collapsed the six subcategories into two totals: harm to users and harm to others. I feel this helps readers immediately see the larger story.  
- I used a diverging bar chart so users and others split cleanly left and right and share a common baseline.  
- I grouped drugs wherever possible into categories such as "Stimulants" or "Psychedelics", which several interviewees found helpful.  
- I revised the title so the main point is explicit and aligned it with the ranking on the chart.  

### Reflection

I liked seeing how my early instincts aligned with user comments. I noticed that simplifying the chart did not weaken the story but actually made it stronger. I feel the diverging design communicates both who is harmed and by how much, without overwhelming readers. The process reminded me that polishing the original form can be a useful first step, but sometimes the most helpful move is to change the form entirely. I also realized how often design problems come from structural clutter rather than aesthetic choices, and how a small shift in layout can reshape the entire narrative. 

I think this exercise made me more aware of how readers scan visuals, not how designers intend them to be read. I noticed that every redesign choice forces a tradeoff, and the best version is usually the one that respects attention rather than detail.

Overall, I feel I learned how to balance nuance with clarity in a way that serves the reader rather than the data alone.

---

## References

- Original graphic from *The Economist*: [https://www.economist.com/graphic-detail/2019/06/25/what-is-the-most-dangerous-drug](https://www.economist.com/graphic-detail/2019/06/25/what-is-the-most-dangerous-drug)

- Dataset: [https://data.world/makeovermonday/2025w36-drug-harms-in-the-uk](https://data.world/makeovermonday/2025w36-drug-harms-in-the-uk)

- Inspiration for diverging bar format: [https://www.datylon.com/resources/chart-library/diverging-bar-chart](https://www.datylon.com/resources/chart-library/diverging-bar-chart)

---

## AI acknowledgements

I used GitHub Copilot to help me explore alternative visualization methods, verify data calculations, and debug code while generating early prototypes of the chart. I used Google Gemini to help fix markdown formatting issues in the notebook and to troubleshoot spacing problems in the final file export. All design decisions and written content reflect my own judgment and interpretation.
