# Notes on Magic Ink
This isn't a full summary of the paper, but just the parts that were interesting to me.

Bret Victor, a notable computer scientist devoted to improving human-computer interaction, wrote the paper *Magic Ink: Information Software and the Graphical Interface* in 2006. Despite its age, the paper is still considered by many as required reading for software designers. I agree that *Magic Ink* provides a valuable perspective on the way software should present information to users and has influenced or predicted how "good" software works today.

The core argument of the paper is that putting interactivity at the forefront of information software development is a bad idea: it leads to a more complicated user experience because the user has to learn how to interact with each new piece of software they use. Humans didn't evolve alongside complex interfaces, argues Victor, so we should make our software as similar to tried-and-true graphical representations, such as maps and newspapers, as possible.
Software developers and designers should instead begin by figuring out what information the user actually wants. What questions does a user want answered when they access this piece of information software?

Victor advocates strongly for several methods of contextualising software that make me uncomfortable given the current climate of regular privacy violations by tech companies. Even "helpful" things that Apple and Google do, such as grouping my photos by my friends' faces or pulling guesses for calendar events from my text messages, are more likely to evoke feelings of unease than gratitude to the designers. Victor proposes this kind of information gathering throughout, for example: "Consider a person reading the website of an upcoming stage play. When she opens her calendar, the available showings should be marked. When she opens a map, she should see directions to the playhouse. When she opens a restaurant guide, she should see listings nearby..." What isn't discussed is how this data can be used to serve ads or be exploited by companies for profit, which is a concern today. Whether we like it or not, Victor's vision is being fulfilled: YouTube tailors its suggestions to each user given their (and others' trending) preferences, Google by default tracks your location and "knows" where you work to provide commute estimates, our phones listen to our conversations then feed us relevant ads on Facebook and Instagram.

A smaller-scoped suggestion of Victor's that we could consider for our software is last-value predictors, which he frames as a minimum requirement. We could remember user search and form input to provide suggestions or pre-fill future forms.

In what seems to be the climax of the paper, Victor proposes a tool to “allow designers to create dynamic data-dependents graphics with no conventional programming”. In 2006, the only options for designers are static mockups and fully programmed UIs, but in 2019 we have JustInMind, Adobe XD, etc. His idea is for a designer to be able to input several pairs of UI + dataset examples into the tool, and for the tool to infer a pattern and be able to generate any UI given by any dataset, which could then be used to provide a fuller experience of what the end product will be. Even though Victor considers a lot of points, including implementation, I’m not convinced that a tool like this is achievable or that it would have a scope wide enough to cover any UI. Additionally, I think there are a lot of places where inference could go the wrong way and cause a loss in translation between the designer’s idea and prototype. Perhaps this is evidenced by the fact that there isn’t any design tool out there (as far as I know—please correct me if I’m wrong) that uses this method to the degree proposed. 

How can we apply some of these ideas to our team so our software has better UI? 

•	Our program isn’t nearly as simple or narrowly-scoped as the examples Victor gave, however, we could break things up by module or task to then try to apply Victor’s viewpoints. 

•	He points out that it’s much easier to just throw in a new menu item than to redesign a dynamic graphic, which I’m definitely guilty of. 

•	However, his extreme favour for graphical representation over textual dropdowns, etc., won’t always translate well to our product. The items we deal with are abstract and custom and it would be expensive to coordinate with customers on a graphical interpretation for them.

•	We currently only provide absolute navigation—maybe we could look into relative navigation (defined as predictions that the user refines) depending on the user’s role.

•	We *should* raise our standards for tight feedback loops: letting the user know that their actions have been registered and making it clearer when we’re doing additional work behind the scenes

•	I agree that hiring developers who have a track record of good UI habits and investing in educating employees on good UI design is key. 

In conclusion, Victor was clearly ahead of his time, and I’m glad to have looked through the world through his lens. Just exposing oneself to different viewpoints on software design is a valuable investment that pays off when considering approaches for a new design. I do agree with his assertions that "interaction is a bottleneck" and "good information software reflects how humans, not computers, deal with information" and will be chewing on these ideas for future applications.

Additional notes:

•	Victor predicts "pocket devices" that will eventually replace wallets and keys, with great onboard storage but also ubiquitous network access.

•	"Sometimes an excellent graphical element is simply a concise sentence"

•	I loved the settings approach of modifying a piece of text that said what the program was doing 

•	My favourite quote (that I wholeheartedly agree with): “Further, the user might prefer to learn information while user her hands for other purposes, such as writing or eating or stroking a cat.”
