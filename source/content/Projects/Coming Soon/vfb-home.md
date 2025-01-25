---
title: VFB-H
draft: true
---

Disclaimer: The following was initially written as part of my dissertation, which was submitted as partial fulfillment of the requirements for my degree at the University of Georgia.[^diss]

TODO: go through and make whatever adjustments to chapter writing - straight from dissertation atm
TODO: add links to other pages
TODO: TABLES

<div class="article-header">

# What is VFB?
</div>

# Virtual Fitness Buddy - At Home Systems
    
Given the onset of the COVID-19 pandemic at the beginning of 2020, we were no longer able to run the afterschool-based Virtual Fitness Buddy (VFB-A) system. We pivoted once more and turned the public space VFB-A system into an at-home intervention (VFB-H). Instead of using the large screen kiosk from our prior studies, we used an iPad as the primary interaction device (see Figure 1)<!--- TODO: (see Figure ~\ref{fig:vfbh-interface}) --->. Our primary goal with this new system was still to motivate children to engage in healthier physical activity (PA) habits over time. With this version, we wanted to integrate the child’s family more into the system, giving siblings and guardians of the primary child the ability to contribute to and interact with their VFB. This way each participant had a support system similar to their peers and site staff during the VFB-A studies. Two cohorts of 25 children used this new VFB-H system across a 4.5-month period, which consisted of 16 and 9 children (C1-H and C2-H) respectively. We also had control groups for both of these cohorts, resulting in a total of 29 and 15 children which started in Fall 2021 and Spring 2022, respectively. There was also a small pilot that was used as a way to beta test this new system and address any bugs that were discovered in the field. This allowed us to focus on designing even more minigames and update existing ones based on feedback and play metrics.

<!--- TODO: (see Figure ~\ref{fig:vfbh-interface}) --->
<figure>
  <img class=scale-w100 
    src="vfbH_interface_example.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 1. The VFB-H iPad interface, featuring the Bark It minigame. The personal leaderboard is shown on the left. The player’s hand avatar is shown in the middle of the screen near the bottom.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.99\textwidth,height=90mm,keepaspectratio]{figures/VFB-H/vfbH\_interface\_example.png}
    \caption{The VFB-H iPad interface, featuring the Bark It minigame. The personal leaderboard is shown on the left. The player’s hand avatar is shown in the middle of the screen near the bottom.}
    \label{fig:vfbh-interface}
\end{figure} --->

## Input System
Initially, we focused on incorporating augmented reality (AR) elements as part of the system, where the VFB and minigames would appear as if they were part of the real world. It was going to be a system where they were in fact interacting with their VFB in their own space. However, we abandoned this approach as it was not practical for us to deploy such a system with the amount of time available given all the different environments where this system could be used. Additionally, unlike a touchscreen system, we did not already have an established codebase using AR already, rendering this approach even less practical. Instead, we pivoted to a system we had already implemented for the previous virtual buddy (VB) experience: a combined motion- and touch-based input system. This way we could leverage our familiarity with these types of controls and most of the UI was transferrable as it was largely on a touchscreen already. Based on our experiences deploying both the Virtual STEM Buddy (VSB-M) and VFB-A systems, we knew that touch controls likely were familiar to our participants. 

The resulting system used real-world iPad rotation to rotate the camera view and used touch controls, including virtual joysticks, for all other necessary inputs. They could also move their avatar around by moving in the real world, but we did not leverage this behavior when redesigning our minigames as we did not want lack of space to be an impediment for our participants. The skeleton avatar used during our previous studies was replaced by a virtual hand as shown in Figure 2 <!--- TODO: Figure ~\ref{fig:vfbh-avatar} ---> as this new version would be played in first person rather than the third person perspective we had been using for the previous VB systems.

<!--- TODO: Figure ~\ref{fig:vfbh-avatar} --->
<figure>
  <img class=scale-w50 
    src="vfbH_avatar-hand-cropped.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 2. The VFB-H user avatar was a hand that, when as item was being held, would change to that item.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.6\textwidth,height=50mm,keepaspectratio]{figures/VFB-H/avatar hand cropped.png}
    \caption{The VFB-H user avatar was a hand that, when as item was being held, would change to that item.}
    \label{fig:vfbh-avatar}
\end{figure} --->

As mentioned, we did design this to use both motion and touch controls. This is best exemplified by our new throwing system. We removed the shot zones from the VFB-A system as it was both difficult for our participants to use and was not practical to use with an iPad-based system. The shot zones were designed to show participants where to place their hands and make more precise aiming possible for the Basketball minigame. For this new system, they were no longer directly using the motion of their hands as their primary input system. Instead, the intent was to use the iPad's rotation to assist with aiming where an item should be thrown similar to some mobile games. In order to indicate when and how hard they wanted to throw, we added two red, virtual buttons for them to press down. The longer they held them down, the stronger their throw would be and the farther the item would go. In order to throw the item, they would release these buttons. The strength of the throw was displayed using an onscreen power meter (see Figure 3)<!--- TODO: (see Figure~\ref{fig:vfbh-powerMeter}) --->. Thus, our throwing system required the use of both touch (power up and throw) and motion inputs (aim) in order to work as intended. This system was used for the Basketball minigame, fetch, and the Frisbee minigame.

<!--- TODO: (see Figure~\ref{fig:vfbh-powerMeter}) --->
<figure>
  <img class=scale-w75 
    src="vfbH_Throw-Power-Meter2.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 3. While aiming an item, the user avatar temporarily changed to that item. They would also hold down the red circles to charge the power meter./figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.65\textwidth,height=65mm,keepaspectratio]{figures/VFB-H/Throw Power Meter2.png}
    \caption{While aiming an item, the user avatar temporarily changed to that item. They would also hold down the red circles to charge the power meter.}
    \label{fig:vfbh-powerMeter}
\end{figure} --->

Lastly, participants could now play fetch and perform tricks with their VFB at any time. During the VFB-A studies, participants had to navigate through the touchscreen menu and select the fetch or trick minigame prior to being able to throw a toy or give their VFB a command. Given that participants can now move around the park, we opted to add this mechanic so participants did not have to go to a specified station or even play a game in order to interact with their VFB. They could pick a toy from the popup menu and begin throwing it for their VFB or hold the mic button in order to issue a trick command. They could also navigate the popup menu to execute tricks without voice commands if desired. 

## VFB Park
In all of our previously discussed VFB studies, the environment was a park of some variety. This new VFB-H version was no different as we used the VFB-A park as a starting point for this new park. A core difference between VFB-H and those previous studies is that VFB-H was the first time our participants were able to move around the entire park rather than being anchored to a set position. With this new park to traverse and explore (Figure 4)<!--- TODO: (Figure ~\ref{fig:vfbh-side-view})--->, we needed to fill this park with things for participants to do. Instead of having each game played in the same location as we had done in the past, we setup "play stations" (Figure 5)<!--- TODO:(Figure ~\ref{fig:vfbh-minigame-locs}) ---> for each of our minigames (Agility, Bark It, Basketball, Frisbee, Soccer, and Volleyball). The implementation of these minigames will be discussed further in the Minigames section below. 

<!--- TODO: (Figure ~\ref{fig:vfbh-side-view})--->
<figure>
  <img class=scale-w100 
    src="vfbH_park_example.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 4. A view of the VFB-H dog park showing the various minigame stations.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/VFB-H/vfbH\_park\_example.png}
    \caption{A view of the VFB-H dog park showing the various minigame stations.}
    \label{fig:vfbh-side-view}
\end{figure} --->

<!--- TODO:(Figure ~\ref{fig:vfbh-minigame-locs}) --->
<figure>
  <img class=scale-w100
    src="vfbH_parkOverhead_withNumbers_example.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 5. The layout of the VFB-H dog park. Each minigame has its own designated play area: Agility (1), Bark-It (2), Basketball (3), Frisbee (4), Soccer (5), and Volleyball (6).</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/VFB-H/vfbH\_parkOverhead\_withNumbers\_example.png}
    \caption{The layout of the VFB-H dog park. Each minigame has its own designated play area: Agility (1), Bark-It (2), Basketball (3), Frisbee (4), Soccer (5), and Volleyball (6).}
    \label{fig:vfbh-minigame-locs}
\end{figure} --->

As shown in Figure 5<!--- TODO:(Figure ~\ref{fig:vfbh-minigame-locs}) --->, each of these play stations consisted of a virtual kiosk, a scoreboard, a court where applicable, and props that were necessary to play the associated game. The virtual kiosks (Figure 6)<!--- TODO:(Figure ~\ref{fig:vfbh-virtual-kiosk}) ---> served a similar function to the touchscreen from VFB-A, where they were used to start and stop the associated minigame, display its instructions on how to play, and display various high scores on a leaderboard. Similar to the high score leaderboards from VFB-A, the new leaderboards could display not only a participant's top three scores for the associated minigame but also could display their family's top three scores and the entire cohort's highest three scores, which they could cycle through with a button press. The remaining tablet functions, such as customizing their VFB and choosing a toy to throw, were placed inside a popup menu, using the same menu system from VFB-A. The courts were intended to resemble the courts used in the real world for each minigame, such as a half a Basketball court and an Agility course used in Agility competitions. Lastly, these play stations were all always displayed in the park, regardless of which game a participant was playing.

<!--- TODO:(Figure ~\ref{fig:vfbh-virtual-kiosk}) --->
<figure>
  <img class=scale-w50 
    src="vfbH_Virtual-Kiosk.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 6. A virtual kiosk used to start minigames, display instructions, and display high scores.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.5\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/VFB-H Virtual Kiosk.png}
    \caption{A virtual kiosk used to start minigames, display instructions, and display high scores.}
    \label{fig:vfbh-virtual-kiosk}
\end{figure} %TODO: add an image of the menu system??? --->

Many of the props in the play stations we had already used in the past during the VFB-A interventions, such as the Basketball and Soccer goals. For the games designed solely for this VFB-H system, many of the props needed to be generated. To reduce development time and to fit the theme of a dog park given that the VFB model was a virtual dog, we repurposed object models we already had, such as the arch model inspired by the University of Georgia (UGA) arch as weaving poles for Agility and treat bones used as various ramps as shown in Figure 7<!--- TODO: Figure ~\ref{fig:vfbh-bones} --->. 

<!--- TODO: Figure ~\ref{fig:vfbh-bones} --->
<figure>
  <img class=scale-w75
    src="vfbH_Treat-deco-examples.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 7. The treat model (top left) used during the VFB-A study was used as various ramps and columns for the Agility and Bark-It minigames during the VFB-H study. The UGA Arch model (middle left) also served as weaving poles during the Agility minigame.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.9\textwidth,height=80mm,keepaspectratio]{figures/VFB-H/treat-deco-examples.png}
    \caption{The treat model (top left) used during the VFB-A study was used as various ramps and columns for the Agility and Bark-It minigames during the VFB-H study. The UGA Arch model (middle left) also served as weaving poles during the Agility minigame.}
    \label{fig:vfbh-bones}
\end{figure} --->

## Minigames

When designing the VFB-H minigames, we still were constrained by the same three criteria from the VFB-A studies: they should be directly impacted by the health of the VFB (and thus, by the player’s PA), should provide a variety of experiences, and should be based on games that can be played with a real-world dog. Additionally, we did not want our participants to remain sedentary while using this new VFB-H app. Our previous systems had this requirement built into them given that we opted to use a Kinect as our primary VFB interaction method, which meant that our participants would need to move in order to interact with their VFB. An iPad does not inherently necessitate mobility as we could solely utilize the touchscreen. Thus, this new system had a fourth requirement to incorporate motion as much as possible into our minigame designs. This way engaging with these minigames would not be a strictly sedentary endeavor.

%In addition to this new requirement, we also needed to design for an entirely different environment than those from our previous systems. Overall, the previous real-world environments consisted of a relatively open space 

Our six minigames were designed and implemented across our pilot and first long-term cohort, beginning with a single Basketball minigame during the pilot and ending with six minigames complete with leaderboards by the end of the first long-term cohort. As mentioned earlier, the six games consisted of Agility, Basketball, Bark It, Frisbee, Soccer, and Volleyball. Minigames that we had implemented in prior studies drew inspiration from their previous iterations, such as continuing to use paddles for Soccer and Volleyball, while adjusting to accommodate the new control scheme. Our two new minigames, Agility and Bark It, were designed to provide experiences that were different from Basketball, Frisbee, Soccer, and Volleyball, where participants either needed to throw a toy at a given target or use paddles to hit an oncoming toy. This way we added more variety of gameplay to the system, especially for participants who may not be as deft at gauging throw distance.

### Agility
The Agility minigame was inspired by dog Agility competitions, where a dog and their trainer navigate an obstacle course with the goal of completing the course as quickly as possible, minimizing errors, such as hitting a hurdle while jumping over it. We had wanted to implement an Agility minigame for the VFB-C studies, but we were not able to conceptualize mechanics that we thought would work well for an Agility course and for the Kinect motion controls. However, with the new touch control scheme, an Agility minigame became a possibility. In lieu of throwing a toy, Agility required participants to navigate a series of obstacles while showing their VFB where to run next by placing treats along the way (Figure 8)<!--- TODO:(Figure ~\ref{fig:vfbh-agi}) --->.  

<!--- TODO:(Figure ~\ref{fig:vfbh-agi}) --->
<figure>
  <img class=scale-w75 
    src="vfbH_agility_example.png"
    alt="TODO:"
    title="TODO:">   <img class=scale-w75 
                        src="vfbH_agility5.png"
                        alt="TODO:"
                        title="TODO:">
  <figcaption>Figure 8. The Agility minigame from the VFB-H study, showing a VFB jumping over a hurdle to reach the treats on the other side. The blue banner indicates where the VFB should run next.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.7\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/vfbH\_Agility\_example.png} \includegraphics[width=0.4\textwidth,height=70mm]{figures/VFB-H/vfbH\_Agility5.png}
    \caption{The Agility minigame from the VFB-H study, showing a VFB jumping over a hurdle to reach the treats on the other side. The blue banner indicates where the VFB should run next.}
    \label{fig:vfbh-agi} %TODO: increase size to 70mm with hirez
\end{figure} --->

The course consisted of five obstacles that had to be completed in a specific order: weaving poles in the form of an arch, ramp, tunnel, seesaw, and hurdle jump. In order to assist participants, we added a blue banner to indicate which obstacle their VFB needed to complete next. This blue banner also served to indicate the exact location where a VFB needed to run in order to count the obstacle as completed. Given that the next obstacle banner may not be in the participant's view, we also implemented an arrow-based navigation system to help them navigate through the course. While the next banner was not in the participant's view, a guide arrow would appear at the top of the screen, pointing in the direction of the next banner. This guide arrow system would be reused for several other minigames. In addition to the guide arrow, we also reduced the complexity of the obstacle course by having the VFB automatically complete certain obstacles, such as waiting at the correct spot for the seesaw to come down and jumping over the hurdle. This way the Agility course was more about reducing their completion time rather than how to get their VFB to perform certain actions that were not utilized anywhere else.

Lastly, participants' scores were based on how much time they had remaining on the 60 second Agility timer. This meant that participants achieved higher scores if they had more time remaining on the timer. In turn, this meant that Agility required participants to become familiar not only with the Agility course route but also the touch joystick controls to become better at Agility and reduce their completion time. This scoring system also incorporated their VFB's fitness as it could complete the course more quickly as it was able to run faster and faster the fitter it became, reducing the time it needed to reach the next treat.

<!--- %#TODO: NEED HI REZ VERSIONS OF PICS!!!

%TODO: montage of the obstacles?
%TODO: over head of route? --->

### Bark It
The Bark It minigame (Figure 9)<!--- TODO: (Figure ~\ref{fig:vfbh-bark})--> was inspired by the BopIt toys, where players would need to memorize and complete an increasing series of actions in a specific order to continue playing. Our Bark It minigame was a trick memory game, where participants similarly had to memorize and issue the trick commands to their VFB in a specified order. The game would end when the participant missed a trick. Initially, our design included a “fatigue” element, where the VFB would have a random chance of failing (i.e., performing a trick different from the one commanded) after a certain time. As the VFB’s health improved, the chance of failure would decrease and would begin after an increased number of tricks. We did not implement this feature as this game was designed to test the player’s recall and not the VFB’s ability to perform commands. By having the VFB fail to perform the correct trick, the VFB no longer enhanced the player’s skill and inhibited it instead. As a result, we also thought that such a system being the sole way to play Bark It may provide unnecessary frustration for our players by having their high score attempt ruined by random chance. 

<!--- TODO: (Figure ~\ref{fig:vfbh-bark})-->
<figure>
  <img class=scale-h50
    src="vfbH_barkIt_example.png"
    alt="TODO:"
    title="TODO:">   <img class=scale-w75 
                        src="vfbH_barkIt2_example.png"
                        alt="TODO:"
                        title="TODO:">
  <figcaption>Figure 9. The Bark It minigame from the VFB-H study, showing a VFB performing the lay down (left) and spin (right) tricks on the Bark It stage. Behind the VFB, tricks are displayed in the order they need to be repeated on the Bark It screen.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.3\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/vfbH\_barkIt\_example.png} \includegraphics[width=0.7\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/vfbH_barkIt2_example.png}
    \caption{The Bark It minigame from the VFB-H study, showing a VFB performing the lay down (left) and spin (right) tricks on the Bark It stage. Behind the VFB, tricks are displayed in the order they need to be repeated on the Bark It screen.}
    \label{fig:vfbh-bark}
\end{figure} %desired settings: width=0.3\textwidth,height=70mm,keepaspectratio; width=0.7\textwidth,height=70mm,keepaspectratio --->

Given that Bark It scoring was solely based on how many levels (i.e., how many sets of tricks) the participant was able to complete, their VFB’s health still impacted this game. As their VFB became fitter, it could perform more commands in a single play session, which meant participants could achieve a higher maximum score by being able to complete more levels before their VFB ran out of energy. This also meant that the Bark It minigame did not require participants to become more and more proficient using the virtual joysticks as several other minigames did. It was solely based on memorizing tricks and did not have a time limit. Once again, expanding the variety of options participants had to play. It also included the guide arrow utilized by Agility to point towards the Bark It stage and screen if they were not in the participant's view. The game would also pause the screen if it was not visible to the participant so that the commands did not disappear before they had the opportunity to read them.

Bark It incorporated a revised voice command system. Our previous VFB studies had issues with voice commands working consistently, presumably due to a high level of ambient noise and proximity of the player to the microphone. However, given that the VFB-H system was intended to be used at home on an iPad, players would be closer to the microphone while playing and presumably would be in an environment that was less noisy than a cafeteria after school, reducing the interference between the participant and the microphone listening for their command.

Participants were able to issue these voice commands by pressing the microphone to issue short commands to their pet. This system was designed to respond to the first valid command, which meant that it would accept longer phrases so long as a valid command was part of that phrase. We also included words that may sound similar, such as park in lieu of bark, or could be used as alternate phrases for the same tricks, such as speak in lieu of bark. This system was also used to issue trick commands to the VFB at any time (except during minigames) during play as mentioned earlier. Unfortunately, we were unable to implement trick gestures using the touchscreen prior to either of the VFB-H cohorts.

<!--- %scoring something about how players didnt have to worry about getting vfb on stage as it did it automatically

%\subsubsection{Tricks and Voice Commands}
%    - tricks do not have gestures this time around
%    - tricks used voice commands again (or access through menu), or rather, still use voice commands as it was always available just not always consistent
%    - since ipad closer to source of sound for the commands, less interference --->

### Basketball
Since our participants have only been able to stay in a relatively stationary location up to this point, we redesigned two of our previous minigames (Basketball and Soccer) to incorporate this new ability to move throughout the world. Initially, Basketball only required participants to make the basket from any point on the court. Some participants realized they could simply stand near the hoop and keep throwing the ball quickly to achieve the highest scores. As a result, we updated Basketball for our long-term cohorts. Instead of being able to stand in a stationary location, participants would need to move to randomly designated locations around the court to score. These locations were indicated by a red pad on the ground, which would ding, turn green, and emit a faint green glow to let the participant know that they were at the correct spot (see Figure 10)<!--- TODO: (see Figure ~\ref{fig:vfbh-bb})--->. Given that the VFB was required to return the Basketball to the player, this update increased the impact of the VFB’s fitness on the Basketball scores while reducing those scores overall compared to those from the pilot. As their VFB became fitter, the faster that it could retrieve and return the Basketball to the participant, resulting in less wait time between throws which could then be used to make more throws. 

<!--- TODO: (see Figure ~\ref{fig:vfbh-bb})--->
<figure>
  <img class=scale-w75 
    src="vfbH_basketball_example2.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 10. The Basketball minigame from the VFB-H study. The throw power gauge changes color from red to green, increasing how far the toy will be thrown as it fills.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.9\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/vfbH\_Basketball\_example2.png}
    \caption{The Basketball minigame from the VFB-H study. The throw power gauge changes color from red to green, increasing how far the toy will be thrown as it fills.}
    \label{fig:vfbh-bb}
\end{figure} --->

Similar to the VFB-A Basketball minigame, participants increased their score by making more successful throws within 60 seconds. With the new throw system, we provided participants with a full trajectory that terminated when it hit a solid object. This was similar to the trajectory we used for the slingshot trajectory minigame from the Virtual STEM Buddy (VSB) system. Lastly, similar to Agility, Basketball used the guide arrow system to point towards the next throw location. When a participant was on the throw pad, the guide arrow would then point towards the Basketball goal.

<!--- %TODO more something about like how the guide arrow was helpful? --->

### Frisbee
The slingshot minigame from VFB-C was replaced by a new Frisbee throwing minigame. The goal remained the same: pop as many balloons before the 60 second timer runs out. Instead of their VFB collecting treats in the order they were popped, they could now catch the Frisbee to score additional points (see Figure 11)<!--- TODO: (see Figure ~\ref{fig:vfbh-Frisbee})--->. This change was made so that players would not always maximize their throw power every time, which would be a relatively easy way to score points as the Frisbee was guaranteed to go far enough to hit its target. In order to get the highest score, they would need to account for the speed of their VFB along with hitting each balloon. As during the VFB-A study, the player’s PA improved the fitness of their VFB, which also increased its speed. By increasing their VFB’s speed, it could complete its minigame tasks more quickly, which increased the highest potential score that could be earned playing Frisbee. Like the other minigames, Frisbee also used the arrow navigation system to point toward the balloons if they were not in the participant's view.

<!--- TODO: (see Figure ~\ref{fig:vfbh-Frisbee})--->
<figure>
  <img class=scale-w75 
    src="vfbH_frisbee_example.png"
    alt="TODO:"
    title="TODO:">   <img class=scale-w75 
                        src="vfbH_frisbee4c.png"
                        alt="TODO:"
                        title="TODO:">
  <figcaption>Figure 11. The Frisbee minigame from the VFB-H study. During Frisbee, players must gauge how hard to throw the Frisbee so that it both hits the target and is caught by their VFB before hitting the ground to earn the most points.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.7\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/vfbH\_Frisbee\_example.png} \includegraphics[width=0.3\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/vfbH\_Frisbee4c.png}
    \caption{The Frisbee minigame from the VFB-H study. During Frisbee, players must gauge how hard to throw the Frisbee so that it both hits the target and is caught by their VFB before hitting the ground to earn the most points.}
    \label{fig:vfbh-Frisbee}%TODO increase back to 70
\end{figure} --->

### Soccer
Similar to Basketball, the Soccer minigame had players move to random locations around the field in order to kick the Soccer ball into the goal while avoiding the blocker, utilizing the guide arrow system to point towards the next location and then towards the goal (Figure 12)<!--- TODO: (Figure ~\ref{fig:vfbh-Soccer})--->. The goal was to earn the most points in 60 seconds. The VFB would roll the ball towards the player once they were facing the goal. If the ball missed the goal or was blocked, the VFB would retrieve the ball and roll it back towards the player. This meant that the VFB’s health impacted how quickly the VFB could retrieve the ball and return back to its rolling location, where a faster VFB would complete these tasks more quickly. In turn, this meant that the player had more time to score points and, thus, increased the number of points that could be earned. Instead of using the throwing system, motion controls were used to kick the ball towards the goal, where the player would move the iPad as if it were a paddle. This paddle-like system was similar to the one used for both the Soccer and Volleyball minigames from the VFB-C studies except that there was no paddle visualization. 

<!--- TODO: (Figure ~\ref{fig:vfbh-Soccer})--->
<figure>
  <img class=scale-w75 
    src="vfbH_soccer_example.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 12. The Soccer minigame from the VFB-H study. During Soccer, a foot avatar replaces the hand avatar, using this virtual foot to kick the ball. Lastly, the arrow navigation system (right) was used to direct players’ attention to the next objective for each minigame.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.8\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/vfbH\_Soccer\_example.png}
    \caption{The Soccer minigame from the VFB-H study. During Soccer, a foot avatar replaces the hand avatar, using this virtual foot to kick the ball.}% Lastly, the arrow navigation system (right) was used to direct players’ attention to the next objective for each minigame.}
    \label{fig:vfbh-Soccer}
\end{figure} --->

        
### Volleyball
The Volleyball minigame remained almost identical to its VFB-C counterpart (see Figure 13)<!--- TODO: (see Figure ~\ref{fig:vfbh-volley})--->. It used a paddle-like system similar to the one used for Soccer, where a participant would need to use their iPad as if it were a paddle to hit the Volleyball back to their VFB. While we did incorporate elements to make Volleyball a competitive game, we realized that would present a similar problem as Soccer from the VFB-A system, where the game became harder as the VFB became faster as it could reach the ball faster. Thus, we opted to make Volleyball a cooperative game. The player would work with their VFB to maintain the longest streak of volleys in 60 seconds without the ball hitting the ground. Similar to Bark It, we were going to implement a "fatigue" system where their VSB would randomly fail after a certain number of volleys.Similar to Bark It, we did not want the sole version of Volleyball to rely on the VFB not randomly failing in order to make the highest score.

During the first part of C1-H, the Agility minigame score did not compute properly. It would seemingly randomly jump all over the place rather than maintaining the longest streak count. This was addressed and corrected by the minigame update during C1-H and persisted through C2-H.

<!--- TODO: (see Figure ~\ref{fig:vfbh-volley})--->
<figure>
  <img class=scale-h50 
    src="vfbH_volleyball_example.png"
    alt="TODO:"
    title="TODO:">   <img class=scale-h50 
                        src="vfbH_volleyball2_example.png"
                        alt="TODO:"
                        title="TODO:">
  <figcaption>Figure 13. The Volleyball minigame from the VFB-H spackagetudy. During Volleyball, players work with their VFB (shown serving the ball (middle)) to maintain the longest serve streak using their virtual hands to serve.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.7\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/vfbH\_Volleyball\_example.png} \includegraphics[width=0.3\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/vfbH_Volleyball2_example.png}
    \caption{The Volleyball minigame from the VFB-H spackagetudy. During Volleyball, players work with their VFB (shown serving the ball (middle)) to maintain the longest serve streak using their virtual hands to serve.}
    \label{fig:vfbh-volley}
\end{figure} --->
    

## Social Elements
In addition to these new minigames, we also expanded the social elements included with the VFB-H system. The messaging app from VFB-A returned, where players could text their parents from within the app. Given positive feedback from VFB-A where some of our participants were motivated by the overall and weekly PA leaderboards, we implemented a minigame high score leaderboard system. As mentioned in the VFB Park section above, these leaderboards would maintain three different sets of high scores: personal, family, and public. The public leaderboard consisted of the highest scores from all of the participants of a cohort. It was a way to connect players to each other as they could do in person during the VFB-A study. Lastly, we incorporated “family reviews”, where parents would discuss their children’s PA progress every week, explaining their progress and encouraging them to engage in more PA throughout the week. This family review would be required both to improve their VFB’s health through their PA and to be rewarded points through meeting PA goals. The rationale for this requirement was that it would incentivize children to remind their parents to complete their family reviews so that they could play new games and buy new items. These new additions were designed to increase players’ feeling of connectedness to each other, their family, and/or their VFB.

### Trophy System
In addition to earning points by completing PA, we also designed and implemented a trophy system. Everyday players would unlock trophies that would change based on their PA, increasing in size as they completed higher PA goals (see Figure 14)<!--- TODO: (see Figure ~\ref{fig:vfbh-trophy-sizing})--->. Additionally, if they met a very high goal, a copy of their VFB performing a random trick was placed atop the trophy (see Figure 15)<!--- TODO: (see Figure ~\ref{fig:vfbh-dynamic-trophy})--->.These trophies lined the park perimeter so that players could see their progression over time. By providing our participants with a tangible representation of meeting their PA goals, we thought that we could potentially further increase players’ motivations to meet those goals.

<!--- TODO: (see Figure ~\ref{fig:vfbh-trophy-sizing})--->
<figure>
  <img class=scale-h50
    src="vfbH_Trophy_Sizing.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 14. A series of PA trophies, which increase in size as higher PA goals are met. The leftmost plaque is awarded when daily goals are not met. Lastly, if a daily PA goal exceeds 11,000 steps, a randomly animated copy of the VFB is placed on top of the trophy.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=70mm,keepaspectratio]{figures/VFB-H/Trophy Sizing.png}
    \caption{A series of PA trophies, which increase in size as higher PA goals are met. The leftmost plaque is awarded when daily goals are not met. Lastly, if a daily PA goal exceeds 11,000 steps, a randomly animated copy of the VFB is placed on top of the trophy.}
    \label{fig:vfbh-trophy-sizing}
\end{figure}--->

<!--- TODO: (see Figure ~\ref{fig:vfbh-dynamic-trophy})--->
<figure>
  <img class=scale-h50
    src="vfbH_trophy2.png"
    alt="TODO:"
    title="TODO:">   <img class=scale-h50
                        src="vfbH_trophy3.png"
                        alt="TODO:"
                        title="TODO:">
  <figcaption>Figure 15. Examples of a VFB performing sit (left) and stand (right) atop a PA goal trophy.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.5\textwidth,height=60mm,keepaspectratio]{figures/VFB-H/vfbH\_trophy2\_example.png}\includegraphics[width=0.5\textwidth,height=60mm,keepaspectratio]{figures/VFB-H/vfbH\_trophy3\_example.png}
    \caption{Examples of a VFB performing sit (left) and stand (right) atop a PA goal trophy.}
    \label{fig:vfbh-dynamic-trophy}
\end{figure}--->

## Physical Activity Data Syncing
Lastly, given our previous troubles with syncing participants’ Fitbit data, we changed our methods for syncing. Each family was provided with one iPad (treatment) or iPod touch (control), which meant that our primary participant would have a dedicated device syncing their Fitbit in the background. Since we pivoted to using the Fitbit application for syncing rather than our own system, neither Fitbit detection nor a recent Fitbit sync were required to login. Both of these were pain points of our previous systems. To login, players entered their family code and then selected themselves from the family member list. This code could be saved for convenience as the iPad stayed with the same family for the duration of the study. In our experience, we found this new system less frustrating to use during testing.
<!---%they could still login without syncing, just wouldnt have progress-->

## Results and Observations
The goal of this dissertation is not only explaining our lessons learned by implementing these systems but also to discern if there are particular elements that increased participant engagement. As such, this was an exploration of the depth of data that we have from this study. For the purposes of analyzing this data it should be noted that where participants are not explicitly labeled as belonging to C1-H or C2-H, their cohort can still be determined by both their participant and family ids, where C1-H participants have ids in the 50,000 (5000 family) range and C2-H participants have ids in the 60,000 (6000 family) range.

[^diss]: [Ball, Catherine. Design and Field Implementation of Virtual Buddy-Based Serious Games for Children. Diss. University of Georgia, 2023.](https://esploro.libs.uga.edu/esploro/outputs/doctoral/Design-and-Field-Implementation-of-Virtual/9949618127102959)