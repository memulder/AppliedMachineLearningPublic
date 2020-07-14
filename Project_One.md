[Mardi Gras Parade Social Distance Detection Video](https://i.imgur.com/ISfAyvF.gifv)

#### Was your social distance detector effective at detecting potential violations?

Quite honestly I was shocked by the results of my detector. The video I chose to analyze was from a parade of dancers during Mardi Gras in New Orleans, where there were certain to be innumerable social distancing violations (though this video was shot some years before COVID-19 was even a concern). However, the detector picked on a detail that I had originally missed when viewing this video, all of the dancers were evenly spaced out, and apparently, they were more than 6 ft. apart. So, while I was expecting a lot of violations, my detector concluded (which I concur with) that there were no violations between the dancers. That being said, while the dancers were front and center and I believe the detector was correct in saying there were no violations among then, the detector largely ignored the crowd in the background and thus missed potential violations (though it might have ignored the crowds because of how dark they are and because they are at the very edges of the frame). As such, I think that my detector was relatively effective at detecting potential violations. 

#### Do you think this approach would be effective for estimating new infections in real time? How would you implement such an approach in response to the COVID-19 pandemic we are currently experiencing?

Personally, my computer took a long time to just analyze a few seconds of video, but if there was a computer that could handle processing so much data very quickly then it might be a good approach for estimating new infections. Although, this detector does not take into account the setting of the video (outside or inside), how quickly people are moving (and thus how long people are actually in contact with each other), and whether or not people are wearing masks or presenting signs of being sick (like coughing), so this simplistic detector might way overestimate how many potential infections there realistically are. 

To implement this approach during our current pandemic, I think I would focus on footage from enclosed spaces where large groups tend to congregate and move less, such as in grocery stores, hospitals, shopping centers, etc. just to get a more accurate count of the potential infections. The research so far seems to show that there is less of a chance of infecting people in open, outdoor spaces where people are quickly moving past each other, such as in parks or on the streets. So, in order to not overwhelm the system and target the conditions where getting infected is most likely I would implement this detector by looking at security footage from stores.  

### What limitations or improvements might you include in order to improve your proposed design?

As mentioned above, this detector ignores the context, speed, and nature of interaction amongst the people in the video. As such, to improve my design I would focus on trying to account for:
1.) whether the interactions are taking place in an outdoors or enclosed space
2.) whether there is prolonged contact/interaction between people, and 
3.) whether people are wearing masks or coughing
