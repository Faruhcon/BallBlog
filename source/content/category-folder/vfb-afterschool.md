---
title: VFB-A
draft: true
---

Disclaimer: The following was initially written as part of my dissertation, which was submitted as partial fulfillment of the requirements for my degree at the University of Georgia.[^diss]

TODO: go through and make whatever adjustments to chapter writing - straight from dissertation atm
TODO: add links to other pages
TODO: TABLES

<div class="article-header">

# What is VFB?
</div>


# Virtual Fitness Buddy - Afterschool Systems

We have explored using both a virtual buddy and motion-based games to encourage children to engage in healthier physical activity (PA) habits with our previous camp-based Virtual Fitness Buddy (VFB-C) projects [^j2014mixed] [^a2015using] [^a2019points]. The results showed that the VFB-C system did encourage children to engage in more PA during their time at the summer camps. However, these studies were only across the course of a few days, which does not provide sufficient longitudinal data to know how the VFB-C system impacted these PA habits over time. To explore the long-term impacts, we redesigned the VFB-C system into the afterschool-based Virtual Fitness Buddy (VFB-A) system. The design of this system was informed by our experiences and our lessons learned from both the VFB-C and Virtual STEM Buddy (VSB-M) systems, which were virtual agent, motion-based systems for children that were deployed unassisted in public spaces.

<!--- TODO: (see Figure ~\ref{fig:vfba-kiosk-n-VFB} (second from left)) --->
<figure>
  <img class=scale-w100 src="vfbA_kioskComparison.png">   <img class=scale-w100 src="VFB-A-H and VFB-C Comparison - Motion Blur.png">
  <figcaption>Figure 1. (Left) Kiosks used during the VFB-A pilot (left) and C1-A and C2-A (right). The pilot kiosk resembles the original kiosk from the VFB-C study. The C1-A/C2-A kiosk added a touchscreen display for menu selection. (Right) The evolution of the VFB model from the VFB-O system (left) to the VFB-A system (right) with the UGA Arch in the background.</figcaption>
</figure>
<!---\begin{figure}[h]
    \centering\includegraphics[width=0.55\textwidth,height=70mm,keepaspectratio]{figures/VFB-A/vfbA\_kioskComparison\_example.png}\includegraphics[width=0.45\textwidth,height=70mm,keepaspectratio]{figures/VFB-A/VFB-A-H and VFB-C Comparison - Motion Blur.png}
    \caption{(Left) Kiosks used during the VFB-A pilot (left) and C1-A and C2-A (right). The pilot kiosk resembles the original kiosk from the VFB-C study. The C1-A/C2-A kiosk added a touchscreen display for menu selection. (Right) The evolution of the VFB model from the VFB-O system (left) to the VFB-A system (right) with the UGA Arch in the background.}
    \label{fig:vfba-kiosk-n-VFB}
\end{figure}--->

Like the VFB-C system, the VFB-A system was designed to encourage children to engage in healthier PA habits. Three cohorts of 223 children across 11 sites used this new system. These cohorts consisted of a 6-week long pilot cohort of 31 children at a single site and two larger, 6-month cohorts of 124 children across 6 sites and 68 children across 4 sites respectively (C1-A and C2-A). We also had control groups at each of these sites, resulting in a total of 42 children across 2 sites for the pilot starting in Spring 2018 and 257 children across 12 sites and 165 children across 7 sites for the two 6-month cohorts starting in Fall 2018 and Fall 2019 respectively. The VFB-A system consisted of an updated kiosk, using a large screen TV and Microsoft Kinect for Windows for motion-tracking (see Figure 1 (second from left)) <!--- TODO: (see Figure ~\ref{fig:vfba-kiosk-n-VFB} (second from left)) --->. Given the success of the mobile kiosk design during the VFB-C study, we continued to use it for the updated kiosks as it was convenient for the site staff to deploy, power on/off (using a single cable) and store every day. Additionally, we opted to use an avatar similar to the VSB-M skeleton avatar (see Figure 2) <!--- TODO: (see Figure ~\ref{fig:vfba-skeleton}) --->. This new avatar featured a semi-transparent body (to make it easier to see the virtual world) and opaque, green-colored “hands” (to indicate which sphere could interact with the VFB and other virtual objects). Lastly, unlike the VFB-C study, where the player’s avatar was off to the side of the screen, this new avatar existed in the world alongside the VFB.

<!--- TODO: (see Figure ~\ref{fig:vfba-skeleton} (left)) --->
<figure>
  <img class=scale-h50 src="vfbA_skeleton_example.png">
  <figcaption>Figure 2. The VFB-A skeleton avatar featured in the VFB-A virtual park.</figcaption>
</figure>
<!---\begin{figure}[h]
    \centering\includegraphics[width=0.7\textwidth,height=60mm,keepaspectratio]{figures/VFB-A/vfbA\_skeleton\_example.png}  \includegraphics[width=0.7\textwidth,height=60mm,keepaspectratio]{figures/VFB-A/vfbA\_kioskInteraction\_example.png}
    \caption{(left) The VFB-A skeleton avatar featured in the VFB-A virtual park. This avatar uses participants’ real-world motions to interact with the virtual world (right).}
    \label{fig:vfba-skeleton}
\end{figure}--->

## Interaction Systems

In addition to the new kiosk, we also updated the primary interaction systems, incorporating what we learned both from the VFB-C and VSB-M systems. From the VFB-C studies, we incorporated participant feedback from both mid-air hover selection system and the trick gesture systems. From VSB-M, we incorporated the success of the new avatar system, the new tablet interface, and VFB-C inspired grab gesture interaction technique. Both of these sources of inspiration and their resulting systems will be discussed in further detail across the next few sections.

### Pilot: 3D Virtual Keyboard Input System

Given participants’ frustration using the mid-air hover selection interface during the VFB-C study, we designed and implemented a new selection interface for the VFB-A pilot study. Although we knew that the addition of the tablet to the VSB-M system was successful, we still wanted to try to find a system that solely relied on the Kinect as the input system because additional devices still meant additional complexity and, potentially, additional development time. Given that this new system would be used across many more sites and participants than we ever had previously, we wanted to minimize hardware complexity in order to reduce the strain on site staff as well as potential points of failure in this new system.
    
We tried several ideas, including a bin system that would use the grab gesture from the VSB-M system. Participants would bring their hands together to grab a choice block that would then be released when they moved their hands apart over the bin they desired to select. However, we wanted to have this new VFB-C system to incorporate VFB setup into the VFB app itself rather than having participants fill out a paper form that then had to be manually uploaded and verified. This meant that participants needed to be able to name their VFB using the VFB-C app. In turn, this meant we needed to have many bins on screen in order to accommodate a 3D keyboard. We were not satisfied with the screen clutter these bins entailed and, thus, decided to try a different interaction technique.

<!--- TODO: (see Figure ~\ref{fig:vfba-3dbutton}) --->
<figure>
  <img class=scale-h50 src="vfbA_keyboardButton_example.png">   <img class=scale-h50 src="vfbA_setGoal_example.png">
  <figcaption>Figure 3. Examples of the “keyboard” keys used for the VFB-A pilot. Similar to a computer keyboard, the red button is pressed in until it “pushes” on the black cylinder.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.5\textwidth,height=40mm,keepaspectratio]{figures/VFB-A/vfbA_keyboardButton_example.png}  \includegraphics[width=0.5\textwidth,height=40mm,keepaspectratio]{figures/VFB-A/vfbA\_setGoal\_example.png}
    \caption{Examples of the “keyboard” keys used for the VFB-A pilot. Similar to a computer keyboard, the red button is pressed in until it “pushes” on the black cylinder.}
    \label{fig:vfba-3dbutton}
\end{figure}--->

We opted to build a menu system using virtual “keyboard key” buttons (see Figure 3) <!--- TODO: (see Figure ~\ref{fig:vfba-3dbutton}) --->. Similar to how keyboard keys are pressed, participants would “press” these buttons using their virtual hand in order to make a selection. This system worked well during our lab testing as we knew how these keys were intended to work and became more adept throughout testing. Unfortunately, this did not translate to a success in the field. Our pilot participants struggled to use this new system even after using it several times, especially the larger keyboard used during VFB creation, where it was much easier to accidentally press the wrong button. As a result, we ceased our attempts at making a Kinect-only input system and returned to the Kinect and tablet input system from the VSB-M system.

### C1 and C2: Touchscreen Based Selection System

Given the success of the VSB-M tablet menu system, we designed and implemented a similar system for the next two cohorts. There were two parts of this system that we wanted to change for the VFB-A kiosk: tablet installation location and bluetooth communication. As previously stated, we had an issue where the tablet and its encasing were rotated in such a way that snapped the tablet's charging cable. Although this was addressed by restricting the movement of the tablet, we sought to design the kiosk in such a way that the needed cabling was self-contained. Additionally, we wanted to reduce system complexity by eliminating the need for bluetooth communication between the tablet and the touchscreen. To address both of these concerns, we opted to use a touchscreen (see Figure 1 (second from left)) <!--- TODO: (see Figure ~\ref{fig:vfba-kiosk-n-VFB} (second from left)) --->that was connected directly to the computer, making it an additional display for the computer. By making this switch, we reduced the development complexity of this new menu system as we did not need to develop and test a separate menu application as we did for the VSB-M system. Similar to the VSB-M participants, we found that participants were familiar with how to use touchscreens, learning the new interface much more easily than the previous virtual button interface. 
    
Occasionally, there would be an issue where either the TV or the touchscreen were not turned on prior to the system loading the VFB app. This would cause an issue where the desired component of the app was not displayed properly. Since the problem required an individual to turn on the TV in person, we could not address this problem remotely. We did try to have the TV turn on as the computer booted up, but we were not able to In an attempt to mitigate the impact of this problem prior to the study, we did attempt to have the TV turn on automatically as the computer booted. However, due to hardware limitations, this was not an option. Instead, we added a screen within the VFB-A app that would be displayed on either the TV or the tablet with instructions on how to turn on the respective device and reboot the app. If we saw this issue remotely, we were able to call site staff in order to address it. In the future, if we were return to this kiosk-touchscreen style of interaction, we would ensure that the TV was capable of turning on along with the computer.

## Expanding the VFB Experience

As this system would be used for 6-months as opposed to 3 days, we needed to expand the interactions with the VFB beyond the trick system, which was used for both VFB-C and Virtual Buddy Fruit and Vegetable (VB-F\&V) studies. In order to expand these interactions, we introduced the concept of VFB stats (beyond size), a stamina (energy) system, built a new minigame system, and expanded the available VFB customization options. Across the new few sections, we will explore both the inspirations, rationale behind, and implementations of these new systems.

### VFB Stats, Stamina, and Leveling
As with the previous VFB studies, a participant's VFB should become fitter as they complete more physical activity (PA) and meet more goals in the real world. Previously, this meant that a VFB would complete tricks more quickly and shrink in size as they became fitter. For this new system, we introduced additional VFB-health related statistics (stats): happiness and stamina. All of the VFB stats were allowed to both increase and decrease in C1 in order to mimic how our fitness fluctuates over time based on our PA. We discovered that all of these stats were rather low overall, indicating that we may have let the stat penalties be higher than intended. As a result, we opted to only let VFB stats increase during C2. 
    
VFB happiness was affected by how often a participant visited their VFB. The more often a participant visited their VFB, the happier they became. We intended to have happiness increase both the VFB's tail wagging speed and its likelihood of successfully performing a given command (trick). Due to limited time constraints and prioritizing other mechanics, we were not able to implement the system where the VFB may not perform the correct trick if they have lower happiness. Thus, across all of these cohorts, VFB happiness only impacted its tail wag speed.

With the addition of stamina, size no longer dictated neither a VFB's max trick nor max run speed. Across all of the VFB-A cohorts, size only affected how small or large the VFB appeared in the app. Stamina controlled how much time participants had to play with their VFB and how quickly their VFB moved.

#### VFB Stamina System

Part of expanding VFB interactions included extending the duration of play sessions beyond the duration from the previous VFB studies. However, given that there were many kids at each site, and they only had limited time to play afterschool, these interactions still needed to be relatively short. As a result, we limited play time for each participant to 3 to 5 minutes per day depending on the fitness of their VFB, increasing as their VFB became fitter. This time did not roll over to subsequent days so participants could not stack time and play beyond their allocated 3-5 minutes per day. Unlike the VFB-C studies, participants could revisit their VFB multiple times a day as long as they did not exceed their play time.  

In this context, the fitness of a VFB refers to their stamina (energy) stat, where play time changed as stamina changed. As a VFB's stamina stat increased, the amount of energy it had to spend also increased, which, in turn, resulted in increased playtime for participants. Initially, the stamina system only acted as a play timer, where play time decreased every second a VFB was running or performing a trick. Starting in C2, minigames and tricks had an associated energy cost in order to play. If a VFB did not meet this energy cost, it did not have enough energy to complete the game or trick and it meant that participants could not play that game or trick until the next day. This system allowed us to increase play time and play variety over our previous studies while restricting how long participants could play so that many participants could interact with their VFBs on any given day.

#### VFB Level System

Starting in C2, we introduced many more minigames that a participant could play with their VFB. As a result, we wanted to limit access to which games and tricks a participant could perform based on their overall PA. We achieved this by implementing a pet "level" system, where a VFB's stats only increased when their participant had completed sufficient PA in order to increase their VFB's overall level. Each stat, except happiness, had a threshold at which it no longer increased the fitness of the VFB, where it would no longer continue decreasing in size nor continue increasing in speed and play time. As a result, all participants had the potential to reach a max stat pet; it just varied how many VFB levels it took to get there. 

Additionally, as we added more minigames beginning in C2, this new level system was used to restrict access to minigames and tricks. Given that the amount of PA required to increase a VFB's level was constant across all participants, it allowed us to uniformly set limits on what a participant could access at certain levels of PA. If a VFB could not play a given game or perform a certain trick, this was conveyed to the participant in the menu system, where they could see all of the upcoming activities they could unlock as their VFB leveled. We opted to show participants the upcoming activities in order to provide a potential additional source of motivation to continue completing more PA over time.
        
### Minigames

<!--- TODO: (see Figure ~\ref{fig:vfba-games}) --->
<figure>
  <img class=scale-w100 src="vfbA_minigame_example.png">
  <figcaption>Figure 4. The minigames and tricks from the VFB-A study: Basketball (top left), fetch (top middle), Slingshot (top right), Soccer (bottom left), roll over (bottom middle), sit (bottom middle), and Volleyball (bottom right).</figcaption>
</figure>
<!--- \begin{figure}[h]
        \centering\includegraphics[width=0.99\textwidth,height=90mm,keepaspectratio]{figures/VFB-A/vfbA\_minigame\_example.png}
        \caption{The minigames and tricks from the VFB-A study: Basketball (top left), fetch (top middle), Slingshot (top right), Soccer (bottom left), roll over (bottom middle), sit (bottom middle), and Volleyball (bottom right). }
        \label{fig:vfba-games}
\end{figure} --->

As previously mentioned, participants' interactions with the VFB-A system could be longer than those from the previous studies’, these interactions would still need to be relatively short as there were many kids at each site and they only had a limited time to play afterschool. With this in mind, we designed minigames (see Figure 4) <!--- TODO: (see Figure ~\ref{fig:vfba-games}) --->that were limited to 60 seconds each and limited the number of minigames and tricks a VFB could complete each day. This limit increased as the VFB became healthier. Ultimately, we designed 4 new minigames (Basketball, Slingshot, Soccer, and volleyball) in addition to the trick gestures from the VFB-C system. At the beginning of the study, participants only had access to fetch and a few tricks. Access to these minigames and remaining tricks were earned over time as the fitness of the VFB improved and “leveled up” (see Figure 5) <!--- TODO: (see Figure ~\ref{fig:vfba-size}) --->. This way participants had incentive to keep engaging in PA so that they could unlock these minigames. Across the the following sections, an overview of our general minigame design approach will be described along with descriptions of the available minigames and their inspirations from previous studies.

<!--- TODO: (see Figure ~\ref{fig:vfba-size}) --->
<figure>
  <img class=scale-w100 src="vfbA_petSize_example.png">
  <figcaption>Figure 5. A sampling of different body weights of the VFB, starting at maximum health (left) and ending at minimum health (right) both from the side (top row) and above (bottom row).</figcaption>
</figure>
<!--- \begin{figure}[h]
        \centering\includegraphics[width=0.8\textwidth,height=70mm,keepaspectratio]{figures/VFB-A/vfbA\_petSize\_example.png}
        \caption{A sampling of different body weights of the VFB, starting at maximum health (left) and ending at minimum health (right) both from the side (top row) and above (bottom row).}
        \label{fig:vfba-size}
\end{figure} --->

#### Design Overview

When designing these new minigames, we had three primary criteria: they should be directly impacted by the health of the VFB (and thus, by the player’s PA), should provide a variety of experiences, and should be based on games that can be played with a real-world dog. As in the VFB-C study, a participant’s PA impacted their VFB’s health, which, in turn, impacted their speed, size, and stamina (number of minigames/tricks available each day). The linkage was intended to quickly show participants the tangible benefits of continuing to engage in PA over time. By making the VFB’s health (and, thereby, participant PA) impact the minigames, we reinforce this linkage. The primary way we incorporated the VFB’s health was through their speed. We designed minigame mechanics which would increase the highest achievable score as the VFB became faster, providing additional incentive to engage in more PA. For example, with increased speed, a VFB could fetch the toys/treats used for the Basketball, Slingshot, and Soccer minigames much more quickly, resulting in more throws and potential points during their 60 second timer. For volleyball, the increased speed allowed a VFB to reach a return serve more quickly, resulting in a longer chain of serves along with a higher max score. 

Our second criterion targeted our requirement to expand this system to provide engagement over the longer 6-month time frame. It stated that these minigames should provide a variety of experiences. This meant that there should be minigames which have different interaction mechanics and/or goals. This criterion was established both to cater to different player preferences and to increase the longevity of the system by adding a variety of different experiences and rewards. Participants were likely to have different preferences on which minigames they would enjoy or even partake in the real-world. Participants could be excited to see their real-world sport of choice represented as a part of the VFB-A system, which may serve to further increase their engagement with the system and bond with their VFB. Additionally, if every minigame provided the same experience with the same mechanics, participants would likely become bored and stop engaging with the system much more quickly. By adding this variety, every day could be a different combination of experiences with the VFB, potentially making interacting with it more exciting day-to-day. This criterion resulted in us designing and implementing different gestures and mechanics around which we could design different minigames. 

We drew inspiration from our previous systems for some of these gestures. For example, we used the hand-distance-based gesture from VSB-M Slingshot minigame to implement a new Slingshot minigame and used both the hand-based throw gesture and the hand-based trick gestures from the VFB-C system to implement Basketball and tricks minigames. We designed a new paddle mechanic where a paddle was attached to a specific joint on a participant’s avatar, allowing them to hit an incoming toy. This mechanic resulted in Soccer (foot-mounted) and volleyball (hand-mounted) paddle-based minigames. We found that it was hard to aim the Basketball using a throw gesture, replacing it with a new mechanic called the “shot zone” (see Figure ~\ref{fig:vfba-games}). Participants would touch the “shot zone” (a sphere) to initiate the throw, use the angle between their hand and the sphere (represented by a series of arrows) to aim it, and touch the sphere from this desired angle to complete the throw.    

TODO: put another figure here with an image of a shot zone rather than referring back up a few pages?

Finally, our third criterion states that these minigames should be based on games that can be played with a real-world dog. We designed many of these minigames to have the VFB’s primary role as fetching a toy or performing a trick, which, obviously, are actions that a real-world dog can do. This criterion was important because it grounded the VFB-A system in real-world actions. This grounding was intended to reinforce the connection between a participant’s PA and their real-world health benefits by watching their VFB become healthier and capable of engaging in more “PA” themselves. The intended result of this reinforcement was our primary goal with the VFB-A system: to generate a sense of autonomy and mastery which would motivate participants to continue to engage in more PA after they were no longer able to interact with their VFB.
    
<!--- \subsubsection{Basketball}

Initially designed for the pilot, the Basketball minigame was designed such that a participant would have the capability of throwing more balls (earning more points) as their VFB became healthier and ran faster. This could be attributed to their VFB being able to retrieve the Basketball and return it to their participant more quickly.
        
s because the VFB had to retrieve the Basketball before the player could throw it again. For throwing, we kept the throwing gesture from the VFB-C system to pick up and throw a ball. However, we found that this throwing gesture made it hard to aim the ball. For C2-A (?), we implemented a new mechanic we called the “shot zone” (see Figure 4-VFB-A). This shot zone was based on the Slingshot minigame from the VSB-M system (see Figure 4-VSB-M). A child would touch the center sphere with their virtual hand then aim their shot relative to this sphere, placing their hand behind their back when they were ready to throw. We also used this system to overhaul our trick gestures, where the child would perform the motion shown to complete a trick. We found that this system was confusing and hard to use for the children. We replaced this shot zone system in our next at-home VFB system, which is described further in the next section. 
--->

<!--- \subsubsection{Item Blaster}
Introduced during the pilot...

Prior to the shot zone update, we wanted to have a game where the precision of shots mattered. This minigame used a blaster (see Figure 6-VFB-A) to fire balls at balloons with the goal of scoring the most points in 60 seconds (? or was it to clear the balloons?). The VFB would run and collect treats that dropped from each balloon in the order they were shot. These balloons came in various sizes with smaller balloons granting more points than the larger balloons as they were harder to hit. Since earning points in this minigame relied on the speed of the VFB, the player had the capability of earning more points as their VFB became healthier and able to run faster. We designed this game to require more strategy to maximize score, where the player needs to decide the optimal order in which their VFB fetches the treats. Given the size of the blaster, we incorporated a camera view, making it easier for players to see where the balloons were, viewing objects “down the barrel” of the blaster. Similar to the Slingshot minigame from VSB-M, the player would grab the handles by touching the virtual handles bringing their hands close together to grab them and then pull them apart to fire. We also wanted players to be able to disengage from the blaster by pressing the handles into the blaster. However, this caused problems, making it harder for the system to detect what was an attempt to grab the handles and what was an attempt to disengage. Due to these issues and feedback indicating frustration with this blaster, we changed the blaster into a Slingshot after the pilot for C1-A (or C2-A?), where the player simply needs to bring their hands together to “grab” the Slingshot pouch as in the Slingshot minigame from VSB-M. The rest of the minigame stayed the same. 


Prior to the shot zone update, we wanted to have a game where the precision of shots mattered. This minigame used a blaster (see Figure 6-VFB-A) to fire balls at balloons with the goal of scoring the most points in 60 seconds (? or was it to clear the balloons?). The VFB would run and collect treats that dropped from each balloon in the order they were shot. These balloons came in various sizes with smaller balloons granting more points than the larger balloons as they were harder to hit. Since earning points in this minigame relied on the speed of the VFB, the player had the capability of earning more points as their VFB became healthier and able to run faster. We designed this game to require more strategy to maximize score, where the player needs to decide the optimal order in which their VFB fetches the treats. Given the size of the blaster, we incorporated a camera view, making it easier for players to see where the balloons were, viewing objects “down the barrel” of the blaster. Similar to the Slingshot minigame from VSB-M, the player would grab the handles by touching the virtual handles bringing their hands close together to grab them and then pull them apart to fire. We also wanted players to be able to disengage from the blaster by pressing the handles into the blaster. However, this caused problems, making it harder for the system to detect what was an attempt to grab the handles and what was an attempt to disengage. Due to these issues and feedback indicating frustration with this blaster, we changed the blaster into a Slingshot after the pilot for C1-A (or C2-A?), where the player simply needs to bring their hands together to “grab” the Slingshot pouch as in the Slingshot minigame from VSB-M. The rest of the minigame stayed the same. 
--->

<!--- \subsubsection{Soccer}

Given the mechanical similarities between Basketball and Slingshot, we wanted to design new minigames based around a different mechanic for C2-A (were there more for C1-A?), which resulted in the new paddle system. A paddle was attached to a joint on the child’s virtual body and could then be used to hit a ball. We used this system for two new minigames: Soccer and volleyball. Soccer attached the paddle to the ankle joint, allowing the child to “kick” the ball toward the goal. Their VFB (?) would act as a blocker, trying to prevent the ball from making it into the goal. Inadvertently, Soccer did become harder as the VFB became healthier, allowing them to move faster and, thus, making it easier for them to block the ball. Volleyball attached the paddle to the hand joint, allowing the child to hit the ball over the net to their VFB. Unlike our previous games, volleyball was a cooperative minigame <<**actually most of the games were cooperative except for the first iteration of Soccer where the VFB was the goalie**>>, where the goal was to get the longest hit streak with their VFB before the ball hit the ground. These two games did not have a scoring system for the VFB-A system. This was added during the VFB-H system, which will be discussed in further detail in the next section. <Do we have some play metrics for these handy?>

%\subsubsection{Volleyball} --->

### VFB Customizations, Toys, and the Points System

<!--- TODO: (see Figure ~\ref{fig:vfba-customize}) --->
<figure>
  <img class=scale-w100 src="vfbA_petCustomizations_example.png">
  <figcaption>Figure 6. Several VSBs using the upgraded customization options, which included collars, hats, tags, and VFB color skins.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.75\textwidth,height=60mm,keepaspectratio]{figures/VFB-A/vfbA\_petCustomizations\_example.png}
    \caption{Several VSBs using the upgraded customization options, which included collars, hats, tags, and VFB color skins.}
    \label{fig:vfba-customize}
\end{figure} --->

In addition to these minigames, we added many more customization options for the VFB (see Figure 6) <!--- TODO: (see Figure ~\ref{fig:vfba-customize}) ---> as another way to potentially extend engagement with the VFB-A system. We expanded the collar and VFB skin color options, added new collar tags and hat accessories, and added more toy options (see Figure 7) <!--- TODO: (see Figure ~\ref{fig:vfba-toys}) --->. Given that the VFB-A system was intended to be grounded in reality, the VFB’s skin color could not be changed once the VFB had been made. However, implemented an inventory system where the remaining customizations were stored once they had been purchased, giving participants the ability to update their VFB’s collar, tag, and toy designs. Additionally, the new toy designs were not merely cosmetic as their bounciness and drag when thrown varied.

<!--- TODO: (see Figure ~\ref{fig:vfba-toys}) --->
<figure>
  <img class=scale-w100 src="vfbA_petToys_example.png">
  <figcaption>Figure 7. The expanded VFB toy options for VFB-A, which include a frisbee, bone treat, stick, tennis ball, red wiffle ball, Soccer ball, blue wiffle ball, Basketball, striped ball, and beach ball.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.75\textwidth,height=60mm,keepaspectratio]{figures/VFB-A/vfbA\_petToys\_example.png}
    \caption{The expanded VFB toy options for VFB-A, which include a frisbee, bone treat, stick, tennis ball, red wiffle ball, Soccer ball, blue wiffle ball, Basketball, striped ball, and beach ball.}
    \label{fig:vfba-toys}
\end{figure} --->

Participants earned points to purchase these customizations by meeting their PA goals. Unlike the VFB-C study, where participants could set and meet multiple goals a day, VFB-A participants could only meet one goal per day given the increased longevity of the study. Additionally, the number of points earned scaled with the PA goal selected, where higher goals gave proportionally more points than lower goals. This was done to address the issue where participants would set and meet multiple less vigorously active goals to earn points more quickly during the VFB-C study. As with the new minigames, these new customizations were intended to provide an incentive to engage in more PA and to extend engagement with the VFB-A system. Lastly, these customizations were added to aid in forming the bond between a participant and their VFB by providing the autonomy to customize their VFB as they desired.

<!--- TODO: (see Figure ~\ref{fig:vfba-messaging}) --->
<figure>
  <img class=scale-w100 src="vfbA_messaging_example.png">
  <figcaption>Figure 8. The messaging interface from the VFB-A system. Certain phrases were customized based on the participant’s name, their VFB’s name, and who was listed as the primary guardian.</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.8\textwidth,height=80mm,keepaspectratio]{figures/VFB-A/vfbA\_messaging\_example.png}
    \caption{The messaging interface from the VFB-A system. Certain phrases were customized based on the participant’s name, their VFB’s name, and who was listed as the primary guardian.}
    \label{fig:vfba-messaging}
\end{figure} --->

#### Social Elements

In addition to these minigames and customizations, we further improved and increased the number of social elements for the VFB-A system. We implemented a new messaging system which allowed messages to be sent between children and their parents rather than solely allowing parents to text their child as in the VFB-C study. This system consisted of a newly implemented scrollable chat history and a virtual keyboard (see Figure 8) <!--- TODO: (see Figure ~\ref{fig:vfba-messaging}) --->. In order to prevent inappropriate messages from being written and sent, we opted to preload this keyboard with various phrases. Once sent, the participant’s message would be added to the displayed chat history and be sent to their parent as a text message. 

In order to engage participants with their peers, we implemented a personal top 3 high score leaderboard for each minigame along with weekly and overall PA and VFB interaction leaderboards for each site. The weekly leaderboards were added so that participants would have a new chance every week to reach the top of the leaderboards. They were designed to provide incentive to continue to complete PA throughout the course of the study beyond unlocking all of the customizations, minigames, and tricks. Additionally, for more competitive participants, these leaderboards could provide additional motivation to engage in more and more PA over time. All of these new social systems were designed to facilitate a sense of relatedness between participants and both their parents and their peers. The goal of fostering this sense of relatedness was to motivate participants to continue to engage in PA even after they were no longer participating in this study.

All of these games were intended to provide entertainment, facilitate a bond between a child and their VFB, and demonstrate how PA can improve one’s overall health. We added the scoring systems for three reasons: to provide incentive to beat the high score, to foster competition between players, and to provide a metric which improved as the VFB became healthier. The first two help facilitate a sense of relatedness and mastery and the last one provides another salient benefit of completing PA (in addition to the speed and size of the VFB). By allowing players to set their own goals and select which games to play, players should feel a sense of autonomy over their experience. The result is that these minigames are intended to facilitate all the psychological needs enumerated in previously mentioned self-determination theory TODO: [12].


## Results and Observations

These results and analyses are focused on VFB-A cohort 2 (C2-A) as many of the minigames covered in the previous sections were introduced at that time. Specifically, we will only be covering the Fall 2019 data as schools were closed during Spring 2020, concluding this study earlier than intended as our participants could no longer access their VFB kiosk. This analysis will include all participants across all four of the treatment sites. Additionally, until an update in mid-October 2019, participants could only play the Slingshot minigame. After this update, they were able to play all of the remaining minigames (Basketball, Soccer, and Volleyball) once their VFB reached the requisite level shown in Table 1<!---TODO: Table ~\ref{table:minigame-unlock-levels-vfba} --->. 

<!---TODO: Table ~\ref{table:minigame-unlock-levels-vfba} --->
| Game       | Level Unlocked |
| ---------- | -------------- |
| Basketball | 4              |
| Slingshot  | 2              |
| Soccer     | 10             |
| Volleyball | 8              |

<i>Table 1. The VFB-A levels needed to unlock each minigame.</i>

<!--- \begin{table}[!htbp]
\centering
\begin{tabular}[c]{|c|c|c|c|c|c|c|}
    \hline
    Game & Level Unlocked\\
    \hline
    Basketball & 4\\
    \hline
    Slingshot & 2\\
    \hline
    Soccer & 10\\
    \hline
    Volleyball & 8\\
    \hline
\end{tabular}
\caption{The VFB-A levels needed to unlock each minigame. }
\label{table:minigame-unlock-levels-vfba}
\end{table} --->

We did not begin recording VFB level increases until November 2019. Thus, we used this level increase log along with an event log to approximate the number of days each participant had each minigame unlocked. Prior to November 2019, the first day a minigame was played or a trick was performed, that date would be considered the unlock date for a minigame at or below the required VFB level for that minigame or trick. After November 2019, any minigame that had not already been unlocked for a given participant would be considered unlocked when their VFB reached the requisite level. Lastly, the number of days unlocked were only those days in which participants had access to their VFB. This means that weekends and school breaks did not contribute to the total available play days.

### Game Play Metrics

As shown in Figures 9 and 10 <!---  Figures ~\ref{fig:vfba-basic-game-plays-plays} and ~\ref{fig:vfba-basic-game-plays-time} --->, Slingshot was the most played minigame in terms of number of games played overall. However, it is also the first minigame to unlock at VFB level 2 and the only minigame accessible until approximately a month into the study. Volleyball has the greatest overall duration played, which is interesting given that it is the second to last minigame to unlock. However, the overall number of plays and play time varies for each game based upon when participants unlocked them. Thus, we need to account for these discrepancies regarding the number of days each minigame was available for each participant. As shown in Figures 11 and 12 <!--- ~\ref{fig:vfba-basic-game-plays-perDay-plays} and ~\ref{fig:vfba-basic-game-plays-perDay-time} --->, there is a similar trend even controlling for the number of days each game was available to play.

<!---  Figures ~\ref{fig:vfba-basic-game-plays-time} --->
<figure>
  <img class=scale-w100 src="vfbA_C2_gamePlays_byGame.png">
  <figcaption>Figure 9. Graph depicting the number of plays for each game played during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/Results_C2-A/C2_gamePlays_byGame.png}
    \caption{Graph depicting the number of plays for each game played during C2-A.}
    \label{fig:vfba-basic-game-plays-plays}
\end{figure} --->

<!---  Figures ~\ref{fig:vfba-basic-game-plays-time} --->
<figure>
  <img class=scale-w100 src="vfbA_C2_timeplayed_byGame.png">
  <figcaption>Figure 10. Graph depicting the amount of time played for each game played during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/Results_C2-A/C2_timeplayed_byGame.png}
    \caption{Graph depicting the amount of time played for each game played during C2-A.}
    \label{fig:vfba-basic-game-plays-time}
\end{figure}

TODO: grab rest from VFB-A Leftovers




[^diss]: Ball, Catherine. Design and Field Implementation of Virtual Buddy-Based Serious Games for Children. Diss. University of Georgia, 2023.
[^j2014mixed]: Johnsen, Kyle, et al. "Mixed reality virtual pets to reduce childhood obesity." IEEE transactions on visualization and computer graphics 20.4 (2014): 523-530.
[^a2015using]: Ahn, Sun Joo, et al. "Using virtual pets to promote physical activity in children: An application of the youth physical activity promotion model." Journal of health communication 20.7 (2015): 807-815.
[^a2019points]: Ahn, Sun Joo, Kyle Johnsen, and Catherine Ball. "Points-based reward systems in gamification impact children’s physical activity strategies and psychological needs." Health Education & Behavior 46.3 (2019): 417-425.