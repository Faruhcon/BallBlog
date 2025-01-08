---
title: Virtual STEM Buddy
draft: true
---

Disclaimer: The following was initially written as part of my dissertation, which was submitted as partial fulfillment of the requirements for my degree at the University of Georgia.[^diss]

TODO: add links to other pages

<div class="article-header">

# What is the Virtual STEM Buddy?

TODO: make the kiosk the background??
</div>

TODO: how do figure references? Pandoc?

TODO: link to VSB-C page

<!---
\chapter{Museum-Based Virtual Buddy System}
    Following our summer camp-based virtual buddy (VB) systems, we departed from a health-centered focus for our next system, focusing instead on sparking interest in science, technology, engineering, and math (STEM) concepts. This new system would also be used inside a children's museum rather than a summer camp. The design challenges were similar to our previous systems, where the system needed to be designed around relatively short interaction times and to accommodate the ability to begin playing quickly and easily. In addition to these design requirements, we also needed to design the interactions and the hardware system such that they would work in a limited space with children playing at nearby stations. We also wanted participants to have more options in customizing both their buddy and their experience interacting with the system. This way participants may become more invested in their buddy and the system itself, which in turn could impact their learning outcomes.
--->

The Virtual STEM (Science, Technology, Engineering, and Mathematics) Buddy system (VSB-M) was designed both to engage children with and to attempt to teach children STEM concepts by providing them with a virtual STEM buddy (VSB). It targeted children and parents attending the Children’s Museum of Atlanta (CMOA) and was deployed for over 5 years (January 2017 to May 2022) as an exhibit at CMOA. This deployment resulted in 28,122 recorded plays over a 2-year period (January 2017 to January 2019)[^vsb1].

## Hardware

The VSB-M system utilized a kiosk consisting of a large-screen TV and Microsoft Kinect for Windows (see Figure 1) <!--- TODO: \ref{fig:vsb-kiosk} --->, allowing us to track a child’s real-world movements. These movements were then used to interact with the virtual world. Given our troubles with hover selection from the Virtual Fitness Buddy Camp-based system (VFB-C)[^vfb-c1], we needed to implement a different selection interface for this new system so that our participants could easily customize their VSB and select which minigame to play. 

<!--- TODO: \ref{fig:vsb-kiosk} --->
<figure class=img-fig>
  <img class=scale-w100 
    src="vsb_kiosk.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 1. The VSB Kiosk at the Children’s Museum of Atlanta.</figcaption>
</figure>

Given the prevalence of smartphones and touchscreens being used for other CMOA exhibits, we opted to include an Android tablet alongside this kiosk as a likely familiar interface. In the field, we found that participants were able to learn and use this new touch interface much more easily than the hover selection interface. However, we did have an issue where the tablet and its encasing were rotated in such a way that snapped the tablet's charging cable. This was quickly addressed by restricting the movement of the tablet and there was no subsequent incident of the charge cable breaking for the duration of the installation of the VSB-M kiosk. We opted to have the tablet and kiosk computer communicate via bluetooth. Fortunately, we did not experience any issues with this communication stream in the field.

This kiosk was largely self-maintained and seldom needed further assistance from museum staff beyond turning the kiosk on in the morning and off at the end of the day. We had the kiosk set up such that once the pc, locked behind the wooden doors of the kiosk, was turned on, it automatically logged in and launched the VSB-M app. Similarly, the tablet was locked down to only run the VSB-M app, which could be reset by museum staff by pressing an invisible button several times and entering a passcode. Early in the study, we had an issue where the graphics card in the computer failed twice. The first time, we simply installed a new one, suspecting it might be a faulty graphics card. The second time, we realized that maybe the computer was overheating inside the kiosk as its design did not incorporate openings for ventilation. This was then addressed, and we had no further issues with the computer nor with the graphics card.

## Software

Prior to working on VFB-M, we had not designed games solely using the Kinect motion-based interaction system without a physical button. This means that we always had at least one physical button to signal intentionality with a button press. Additionally, we knew that the hover-based selection technique we designed for the VFB-C system was challenging for our participants to use. Designing these motion-only interactive games proved to be more of a challenge than we had anticipated. We found that it was very hard to signal intentionality without a physical button or the hover selection. For example, if a player wanted to pick up an object, they could not merely point at it and click a button or hover over it to pick it up. We did know from our previous virtual buddy systems that gestures seemed to translate well using a motion-based system<!---, such as the gestures used to perform tricks with their virtual pet in the VFB-C study---> [^vfb-c1].

With all of this in mind, we designed a "grab" mechanic that seemed to work well to indicate a player's intention with the system based on our results. This grab mechanic will be further discussed in the Slingshot section below. Additionally, as mentioned earlier, we included a tablet for interactions which required finer controls, such as menu selection. This allowed us to design games that without needing to consider how they would select the different game options using the motion-based system, reducing the complexity when designing these motion-based games. 

### STEM Buddy

<!---TODO: (see Figure ~\ref{fig:vsb-buddies}) --->
<figure class=img-fig>
  <img class=scale-h75 
    src="vsb_buddies_combo.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 2. The VSB customization interface (left) along with six customized VSBs showing the various color and shape options (right).</figcaption>
</figure>

The VSB was designed to be a personalizable buddy which was intended to act both as a motivating buddy and as a teacher. It would help children and their parents understand the underlying STEM concepts of each minigame while encouraging them as they solved each problem, cheering for them from the sidelines. Since part of our intended audience may not be able to read, these VSBs utilized both text and audio to convey both how to play each minigame and facts about the underlying STEM concepts. Each component of the VSB could be customized prior to starting a minigame, allowing children to design their own unique VSB (see Figure 2) <!--- TODO: ~\ref{fig:vsb-buddies}--->. If a child did not wish to customize the VSB, the system would simply use the previous VSB. Each VSB could be saved using a randomized, unique code which could be texted to a parent. This allowed a child to bring back their personalized VSB during a return visit to the exhibit. An area of interest was also chosen as part of the VSB personalization. This area of interest was used to customize the minigames, where players would complete an image based on the area of interest as they progressed in the minigames. The goal with the personalizable VSB and area of interest was to increase player investment while interacting with the system. It was intended to feel like their own experience and their personal buddy, which in turn was intended to gain their interest while playing the minigames. 

We designed an entire system for participants to customize their buddy, where they could choose not only their VSB's name but also the color and shape of each body part (see Figure 2) <!--- TODO: ~\ref{fig:vsb-buddies}--->. This vastly increased the amount of customization participants could have when compared to our previous virtual buddy systems, where they could only choose the name, collar, and tag of their buddy. This more detailed customization system was possible due to our inclusion of the touchscreen. It allowed participants to use an interaction system they were more likely to have interacted with before as compared to our motion-based, hover selection technique.

The larger vision of the buddy was to design a system where they could take their saved buddy with them once they had finished at the museum. The buddy would be tailored towards their learning needs, adjusting difficulty based on their responses to the system questions. Unfortunately, we were only able to implement the buddy saving system, leaving this "take along" feature for future work.

### Minigames

We designed two motion-based minigames, where the child would use their real-world body to interact with the virtual world. This body was displayed as a collection of spheres in the virtual world (see Figure 3) <!--- TODO: ~\ref{fig:vsb-skeleton}-->. Given that we knew the exact amount of space we were able to use at CMOA, we were able to scale the child’s movements to ensure they were able to reach the necessary areas of the virtual world safely. Before designing the games, we decided the STEM concepts that we wanted those minigames to convey. These concepts were then integrated into the primary game mechanics of each game. This integration demonstrated the concept while the VSB explained the concept behind it. 

<!---TODO: (see Figure ~\ref{fig:vsb-skeleton})-->
<figure class=img-fig>
  <img class=scale-h50 
    src="vsb_skeleton.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 3. The skeleton avatar representing the player from the VSB system.</figcaption>
</figure>

Additionally, we designed the area of interest system with the goal of the virtual world to showing growth with them as participants became better at playing these minigames. For example, this would have included displaying the images they completed along the virtual wall. The goal of this area of interest was to get participants to become more invested in the system as it was tailored to them and their experiences. It would change based upon their work and progress. This system would have complemented the one where their VSB tailored their experience based upon their interests and game performance. For the purposes of this study, the area of interest only impacted what image participants completed as they played the minigames. 

The goal of both of these minigames was to be entertaining while providing information about the underlying STEM concepts of the minigames. Lastly, since the VSB-M system was being used as a museum exhibit, these minigames were designed to have shorter interactions (under 3-5 minutes) that could be played multiple times. They also needed to be playable in the limited amount of space allocated to our exhibit. Both of our minigames will be explained in more detail in the following sections.

#### Lever Hero

 Our first minigame, Lever Hero, was designed around levers and how to balance them (see Figure 4 (left)) <!--- TODO: ~\ref{fig:vsb-minigames} --->. As it was played, see-saws (a form of lever) approached the player with a weight placed at a randomized location. The child then needed to place a counterweight at the appropriate position to balance the see-saw. When they answered correctly, an image based on their chosen area of interest would be built in the background (see Figure 4) <!--- TODO: ~\ref{fig:vsb-minigames} --->. 

 Originally, we had the weight following the player's position as they moved left and right in front of the kiosk, reducing complexity by only allowing their virtual body to move left and right. This way participants did not need to consider forward and back when it came to placing their counterweight. We thought that this would be an easier to use system than our previously used hover technique. However, this mechanic also meant the weight moved along the board, allowing the player to follow the tilt of the lever to adjust their answer accordingly. This means that the lever hero minigame became less about deciding the correct spot to place the counterweight and more about watching the lever balance as they moved, even as the lever approached. Our goal was for them to intentionally set down the weight at the correct spot and not simply move towards the correct answer based on the visualization. We did not change this mechanic in our first major update, but we did change this system to match the "grab" mechanic we designed for our next minigame. This grab technique allowed participants to bring their hands together to snap the weight to their hands. They could then move their bodies in the real world to move the virtual weight to the location they desired to drop it on the lever, which they were able to do by moving their hands apart. This change resulted in increased plays of the lever hero game.

 We designed a system that could handle both multiple weights and weights of different sizes. This system would have allowed us to increase the complexity of the lever hero problems without changing how participants interacted with them. However, we opted to leave this feature out of this iteration of the VSB system in order to teach the concept of lever balancing on a basic level. This decision was made given that we would largely be targeting likely single session interactions with our participants as opposed to sustained interactions with the same participants over time. This idea would work well if we chose to expand upon allowing participants to take their buddies back home with them.

<!--- TODO: (see Figure ~\ref{fig:vsb-minigames}) --->
TODO: same line? hq images where?
<!--- <figure class=img-fig>
  <img class=scale-h100 src="vsb_leverHero.png">   <img class=scale-h100 src="vsb_slingshot.png">
  <figcaption>Figure 4. The Lever Hero (left) and Slingshot (right) minigames from the VSB-M system. There is an image being built in the background based on the player’s area of interest.</figcaption>
</figure> --->
<figure class=img-fig>
  <img class=scale-w100 
    src="vsb_minigame_combo.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 4. The Lever Hero (left) and Slingshot (right) minigames from the VSB-M system. There is an image being built in the background based on the player’s area of interest.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.5\textwidth]{figures/VSB-M/vsb\_leverHero\_example.png}\includegraphics[width=0.5\textwidth]{figures/VSB-M/vsb\_slingshot\_example.png}
    \caption{Figure 9. The Lever Hero (left) and Slingshot (right) minigames from the VSB-M system. There is an image being built in the background based on the player’s area of interest.}
    \label{fig:vsb-minigames}
\end{figure} --->

#### Slingshot

Our second game, Slingshot, was designed around trajectories and how to use them to hit a target (see Figure 4 (right)) <!--- TODO: ~\ref{fig:vsb-minigames} --->. It used a stationary slingshot that children had to aim with the aid of a visible trajectory based on their relative location and distance from the slingshot. As they hit each target, the block then moved to the background, forming an image similar to Lever Hero. The goal of this game was to complete the image without paint splats obscuring it, meaning the child needed to hit the top or sides of the target block. As mentioned in the lever hero section, we designed a grab technique that allowed the slingshot pouch to snap to a participant's virtual hands as they brought their real-world hands close together. When they were ready to fire the slingshot, they pulled their hands apart to let go of the slingshot pouch (see Figure 5) <!-- TODO: (see Figure ~\ref{fig:vsb-slingshot}) --->. Similar to lever hero, we also designed a system to scale difficulty by gradually reducing the length of the trajectory. This would then require participants to rely on their understanding of trajectories more than an on-screen indicator in order to hit the blocks.

<!-- TODO: (see Figure ~\ref{fig:vsb-slingshot}) --->
<figure class=img-fig>
  <img class=scale-w100 
    src="vsb_slingshot_shot.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 5. A player attempting to shoot a block during the slingshot minigame from the VSB-M system.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.8\textwidth]{figures/VSB-M/vsb\_slingshot\_shot\_example.png}
    \caption{A player attempting to shoot a block during the slingshot minigame from the VSB-M system.}
    \label{fig:vsb-slingshot}
\end{figure}
--->

## Results and Observations
The VSB-M system was played 28,122 times in about two years from 1/10/2017 to 1/21/2019. We found that early on Slingshot was more popular than Lever Hero, being played about twice as often. We attributed this to a new mechanic we implemented in Slingshot. Upon updating Lever Hero to use this same mechanic, the discrepancy between the game plays was reduced. We also found that the problems solved increased for both games (see Figure 6) <!--- TODO: (see Figure ~\ref{fig:vsb-stats}) --->. Unfortunately, we did not record how many times the default VSB was changed and only 176 customized VSBs were saved with a code in about a year and a half (9/6/2017 to 1/21/2019) during which 20,825 total games were played. We attribute this low number of saved VSBs both to a lack of tangible benefit for saving the VSB and to the VSB not being directly engaged with the player. It was not salient that the VSB was encouraging and aiding the child as they play. Lastly, we had some hardware issues early on due to overheating caused by poor ventilation. Once those issues were addressed, the VSB-M system continued to run unassisted without further issue from 8/10/2017 to 1/21/2019 [^vsb1].

For future iterations, we conceptualized a tutorial system where a participant's VSB would play the game along with them the first time, showing them how to mechanically play the game. This system would move the VSB from being a stationary figure off to the side to one that would have been actively involved during gameplay. Along with the increased minigame difficulty mentioned earlier, their VSB could also aid them in completing problems. For example, it could be holding an additional counterweight during Lever Hero, giving the opportunity for the VSB to expand participants' understanding on how lever balancing works while further incorporating itself into gameplay.

<!--- TODO: (see Figure ~\ref{fig:vsb-stats}) --->
<figure class=img-fig>
  <img class=scale-w100 
    src="vsb_resultsTable.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 6. Play statistics for the VSB-M minigames after each system upgrade.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.8\textwidth]{figures/VSB-M/vsb\_resultsTable\_example.png}
    \caption{Play statistics for the VSB-M minigames after each system upgrade.}
    \label{fig:vsb-stats}
\end{figure} --->

## Conclusions and Lessons Learned

From these results, we concluded that our upgrades to the minigames were a success, resulting in more games being played and more problems were solved per play session. This indicated that we succeeded in making these minigames increasingly entertaining. We did not track the long-term educational outcomes of the minigames. As a result, we do not know how well the underlying STEM concepts were conveyed and retained. Given the low number of saved VSBs, making the VSB a focal point of the exhibit was not successful. From this system, we gained more experience both in designing both buddy-based and motion-based games and in implementing such a system unassisted in the field. We learned that the VSB needs to be more directly and saliently involved in the experience. We also learned how to better implement hardware and software in the field so that it can be run unassisted for long periods of time.

For our subsequent studies and in terms of hardware, we learned that tablet or touchscreen-based input was actually a viable possibility to use in conjunction with an otherwise motion-based app. Participants were able to use such an interface rather quickly, which we attributed to familiarity of such systems given that there are many examples of touchscreens that can be used in everyday life. We learned that we could secure additional hardware and be able to keep the cabling safe. That being said, it would be better to hide the cabling where it cannot be accessed easily unless by authorized individuals. 

In terms of software, we learned that we should prioritize incorporating the virtual buddy as a core part of the experience, interacting directly with the participant. We also learned that our grab gesture works well as an interaction mechanic and minigames could be designed around this mechanic. Lastly, we learned that a system could be deployed in the field for an extended period with minimal input required by site staff and that being able to remotely apply updates or debug problems was very beneficial.


[^diss]: [Ball, Catherine. Design and Field Implementation of Virtual Buddy-Based Serious Games for Children. Diss. University of Georgia, 2023.](https://www.proquest.com/dissertations-theses/design-field-implementation-virtual-buddy-based/docview/2917424271/se-2?accountid=14537)
[^vsb1]: [Ball, Catherine, Sun Joo Ahn, and Kyle Johnsen. "Design and field study of motion-based informal learning games for a children’s museum." 2019 IEEE 5th workshop on everyday virtual reality (WEVR). IEEE, 2019.](https://wevr.adalsimeone.me/2019/WEVR2019_Ball.pdf)
[^vfb-c1]: [Ahn, Sun Joo, Kyle Johnsen, and Catherine Ball. "Points-based reward systems in gamification impact children’s physical activity strategies and psychological needs." Health Education & Behavior 46.3 (2019): 417-425.](https://pmc.ncbi.nlm.nih.gov/articles/PMC6566098/)
TODO: cite cmoa website??