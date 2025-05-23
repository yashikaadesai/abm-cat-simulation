# Cat Behaviour Agent-Based Model


- Yashika Desai Role: Programmer
- Shanze Owais Role: Programmer
- Carla Carreon-Elisea Role: Programmer, PowerPoint
- Ebise Tarekegn Role: Abstract, PowerPoint

Have you ever wanted to test and see what different personality types of cats would interact with one another? 

In this project, we are creating an agent-based model that shows cats' interactions with other cats and objects. Each cat's interactions will be different based on its personality type.

Some cats might be more social than others, causing compatibilities between the cats or disputes. 

The visualizations will be 2d in a table format that will show our cats interacting

# Project Abstract:

Agent-based modeling (ABM) is a computational modeling approach that uses object-oriented programming (OOP) to simulate and mimic complex environments. In this project, the goal is to model the behavior of a select number of cats to gain a deeper understanding of feline behavior within a contained space and the complex interactions between differing personalities. Our approach was to create cat agents with a range of personality traits from the following list: Calm, Shy, Playful, and Aggressive. The index is from 1-2, 1 being low and 2 being maximum. Along with these needs, there are sub-areas for feeding, sleeping, and a litter box overlayed on our visualization. Any remaining area in the environment is designated as the roaming zone. To quantify our results, we added a play and fight count attribute to each cat to evaluate the effect of varying personality levels on these count variables.

We used Boolean variables to track the needs of cats. We sought to determine if cats of similar personalities interact with each other when their personality levels are the same, if cats of different personality traits interact negatively or avoid one another due to differences in personalities, and are the cats able to maintain their needs alone without being instructed to (i.e. setting initial hunger levels). To test these hypotheses, we varied the initial personality traits of each cat agent. In the simulation, each cat was inactive/sleeping for the first two hours. To define the interactions between agents, playing was only allowed if the cat's personalities were not aggressive, one or both of the cats’ personalities were playful, or if one cat was playful while the other was calm. Similarly, to allow fighting, the cats’ personalities must both be aggressive, or one cat is aggressive while the other is playful. Two shy cats were defined to avoid each other. To outline the parameters for the needs of cats, the agents were set to use the litter after eating, eat after three interactions or three inactive hours, and roam approximately 70% of the time for 20-40 frames. The roaming ability was generated via a random integer generator to ensure that the cats would be actively moving around the board, increasing the possibility of interacting with other cats. The movement of the agents occurred in a direct, random, or goal-oriented manner. For direct movement, the cats will move directly towards their goal target in the x and y directions.

Similarly, for random motion, the surrounding cells are randomly selected if the position does not violate the parameters of the board. If cats are unable to move towards their goal target, a neighboring cell is randomly selected. However, for goal-oriented motion, the cats will take the shortest path possible. Visualization of the environment was implemented with Matplotlib, and markers were encoded to appear when cats would fight or play with each other. For the animation, each hour had ten steps for a total of twelve hours. To track the motivation and purpose behind each cat’s movements, a side column was used to display the cat’s new goal and motivation for every 20 frames. 

We found that with four cats displaying one maximum personality trait, the parameters of the environment were upheld, with all but aggressive cats having playful interactions. When we paired cat personalities together, we observed that for playful and shy cats, the shy cats would have several playful interactions, compared to having zero playful interactions. Parking aggressive and calm cats resulted in an increased number of fights, and yielded zero playful interactions. Finally, with maximum personality traits, there were zero playful interactions, leaving only aggressive interactions. In all these simulations, we found that the cats were able to maintain their needs without count variables,  demonstrated by the constant movements within the food, bed, and litter zones. 

To conclude, we observed that cats with similar personalities will engage and interact with one another in either playful or aggressive manners. Cats can fulfill their own needs without the use and initialization of count variables. For further studies, an expansion on cat personalities and increased attributes can be implemented to better represent and simulate feline behavior. 
