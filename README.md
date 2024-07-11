# OSUBaseballDashboard
A dashboard created as part of the analysis completed for the Ohio State University varsity baseball team, hosted here: [https://tbutz.shinyapps.io/OSUBaseballDashboard/](url)

In 2022, I worked with several other individuals to perform an in-depth analysis for the OSU baseball team. I worked closely with the pitching coaches on the team, who were interested in learning about how pitch sequencing could affect game outcomes. Initially, the coaches relied on conventional wisdom, their own expertise, and the expertise of the players to determine which pitch might be the right one to throw in a given scenario. By consuming the reslts of this analysis, the coaches were able to begin making data-driven decisions throughout each game about what pitch should be thrown.

The data for this project is pitch-by-pitch data recorded manually during the 2021 and 2022 seasons and stored in Excel. Extensive EDA was performed in RStudio, and RStudio was eventually chosen to build an interactive dashboard. For this, the RShiny and ShinyDashboard packages were utilized. The main deliverable consists of five visualizations:

**Pitch Tendencies**: This is a series of bar graphs that demonstrate the type of pitch that a pitcher tends to throw, given the count and their pitch arsenal. For example, we can see how often a pitcher throws a fastball on counts where they are ahead (0-1, 0-2, 1-2) vs when they are behind. Then, it's possible to "click into" the pitch tendencies to see what the outcomes are for a given pitch in a given count. 

**Pitch Sequences**: For a given pitcher, this visualization shows the distribution of pitches thrown within the same at-bat immediately AFTER a certain pitch. For example, it might be the case that after a curveball, a pitcher is more likely to throw another curveball than a fastball. 

**Sequences With Outcomes**: For a given pitcher OR all pitchers and a given first pitch, these pie charts show the distribution of outcomes after each possible combination of first and second pitch. This visualization can be utilized to show the best course of action given the most recent pitch. If a pitcher has just thrown a fastball, it would be useful to know whether throwing another fastball or going to the slider would result in more strikes swinging.

**Base Running/Score Differential**: This visualization shows pitch tendencies within the context of a real game scenario. Based on the score differential of the game and the location of any runners on the base paths, the pitcher's strategy must change. Adding this context enables the user to increase the depth of their data-driven strategy decisions in relation to which pitch should be thrown. 

**Pitching fatigue**: This visualization shows how the the average velocity for each pitch in one outing changes as the outing progresses. Predictably, the average velocity does trend downward as the pitcher fatigures, but this does not happen uniformly across all pitches, or across all pitchers. 
