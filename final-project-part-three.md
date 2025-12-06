| [home page](zenbeam.github.io/shubham-dataviz) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Geography of Artificial Intelligence

## The final data story
You can view the final data story:
[View here](https://shubham-startup-story.vercel.app/)

(Note: This is a Next.js application. To run locally, clone the repo, run `npm install`, then `npm run dev`, and visit `http://localhost:3000`.)

## Changes made since Part II
Since Part II, the project has evolved from a collection of static charts into a cohesive, narrative-driven experience titled "The Geography of Intelligence."

Key changes include:
1.  **Narrative Restructuring**: We moved away from a generic "state of the market" report to a specific argument: *AI is concentrating in specific physical locations.* We added a new "Intro Section" to set this hook ("The Signal in the Noise").
2.  **New Sections**: We added "The Academic Pipeline" to highlight the critical role of universities (Stanford, MIT, Berkeley) as the supply chain for founders.
3.  **De-cluttering**: We removed the "Funding Maturity" and "Investor Concentration" sections to maintain focus on the core "Location & Origin" narrative.
4.  **Actionable Insights**: We added specific "Founder Takeaways" to every section, transforming the data from passive observations into active advice.
5.  **The Founder's Playbook**: The conclusion was completely rewritten from a summary into a tactical checklist for entrepreneurs.

## The audience
The primary audience for this story is **Aspiring AI Founders and Entrepreneurs**.

We narrowed this focus based on the insight that "data is only useful if it helps you make a decision." For a founder, the decision is "Where should I build?" and "What should I build?".

Adjustments made for this audience:
*   **Tone**: We shifted from academic/neutral to "entrepreneurial, curious, and warm."
*   **Format**: We used "Founder Takeaways" in distinct dialog bubbles to make the "So What?" immediately visible.
*   **Content**: We emphasized "Network Effects" and "Talent Density" over raw financial metrics.

## Final design decisions
*   **Visual Hierarchy**: We used a high-contrast design. The Hero section is dark and immersive (using a custom `DynamicBackground` particle effect) to signal "future/tech," while the narrative sections are clean and white for maximum readability.
*   **Motion**: We implemented subtle scroll animations using `Framer Motion` to give the site a "scrollytelling" feel without overwhelming the user.
*   **Typography**: We paired a Serif font (*Playfair Display*) for headings to give the narrative weight and authority, with a Sans-serif font (*Inter*) for body text to ensure clarity.
*   **Components**: We created a reusable `FounderTakeaway` component with a glassmorphism effect to visually distinguish actionable advice from the narrative text.

## References
*   **Data Source**: Analysis of 940 venture-backed AI companies founded since January 2024. Data provided by CB Insights (extracted November 2024).
*   **Images**: City landscapes and university logos were sourced for the visual storytelling elements.

## AI acknowledgements
Microsoft Copilot assisted with structuring the user research protocol and refining this markdown file. The interview findings, quotes, and identified changes reflect actual patterns from real user feedback sessions, with AI helping to organize and synthesize themes coherently. All visualization designs, data analysis, and narrative decisions remain my own original work. AI assistance focused on document structure and professional formatting rather than analytical direction or content creation.

## Final thoughts
This project demonstrated the power of "opinionated data." By taking a stance—that geography still matters—we were able to turn a spreadsheet of 940 companies into a story. The most exciting part was seeing how the "Founder Takeaways" instantly made the charts feel relevant. If I had more time, I would have loved to add an interactive map component where users could filter startups by specific university origins.
