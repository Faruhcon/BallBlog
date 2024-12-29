---
title: VFB-C and VFB-F&V
draft: true
---

Disclaimer: The following was initially written as part of my dissertation, which was submitted as partial fulfillment of the requirements for my degree at the University of Georgia.[^diss]

TODO: go through and make whatever adjustments to chapter writing - straight from dissertation atm
TODO: add links to other pages

<div class="article-header">

# Summer Camp-Based Virtual Buddy Systems
</div>
   
Early pilot studies for the Virtual Fitness Buddy (VFB) system all took place at various weekly summer camps [^j2014mixed] [^a2015using] [^a2019points] [^a2016using]. They established the overall pattern of design across each of these studies where the team would implement the current version and pilot test it. After the pilot, we would then innovate and iterate on that design based on feedback from that pilot. Upon implementing these new designs, they would then be pilot tested out in the field and so on. While we tested these systems ourselves as we implemented their updates, all of the participant testing was done in the field. This allowed us to see how our participants would behave and how well our system worked “in the real world”. We quickly discovered some elements of these systems were not as effective or simply did not work outside of a laboratory setting, where only a few people tested it. The following sections elaborate on two of these systems. One where the goal was to encourage increased fruit and vegetable consumption [^a2016using] and another where the goal was to encourage healthier physical activity habits [^a2019points]. Both utilized a similar virtual buddy that was placed in a similar virtual world where the participant interactions with these buddies varied given their different goals. They also had similar design constraints, where they needed to have shorter interactions that could be completed by many children promptly, their apps needed to have a focus on health-related concepts, and the children should be able to walk up and play with relative ease.

## Virtual Buddy Fruit and Vegetable System

The Virtual Buddy Fruit and Vegetable (VB-F\&V) system was designed to encourage children to consume more F\&V by providing them a virtual buddy (VB). It targeted 25 children attending a weekly summer camp, where it was deployed for 3 days during a single summer camp in 2014 [^a2016using]. In addition to this treatment group, we included two control groups, where one group used the computer to track their F\&V consumption but did not have a virtual pet (22 children) and the other had their F\&V consumption tracked by the camp counselors (21 children). This brings the study to a total of 68 children (ages 7 to 13) across all conditions.
        
<!--- TODO: (Figure ~\ref{fig:vfbc-size}) --->
<figure>
  <img class=scale-w100 src="vfbC_vfb_size.png">
  <figcaption>Figure 1. The range of VB sizes from the least healthy (left) to the most healthy (right).</figcaption>
</figure>
<!--- 
\begin{figure}[h]
    \centering\includegraphics[width=0.75\textwidth,height=60mm,keepaspectratio]{figures/VFB-C/old_vfb_size.png}
    \caption{The range of VB sizes from the least healthy (left) to the most healthy (right).}
    \label{fig:vfbc-size}
\end{figure} --->

Prior to this system, the team had developed the original Virtual Fitness Buddy (VFB-O) system, which targeted physical activity (PA) instead of F\&V consumption [^j2014mixed] [^a2015using] and utilized a motion-based tracking system. The new VB-F\&V system was heavily based on this prior system, consisting of a customizable VB, which became slimmer, faster, and able to perform more tricks as their child consumed F\&V for lunch in the real world (Figure 1)<!--- TODO: (Figure ~\ref{fig:vfbc-size}) --->. F\&V consumption was collected and recorded by camp counselors during lunch and then uploaded into the system. This F\&V consumption was then used to unlock more tricks for the VB to perform. In order to perform these tricks, a child needed to spend trick credits. These credits were earned as a child reached their F\&V consumption goals, where the number of credits earned scaled with the size of their goal. Instead of using the VFB-O motion-based tracking system, the VB-F\&V system used a haptic joystick (Novint Falcon) to interact with the virtual world (see Figure 2)<!--- TODO: (see Figure ~\ref{fig:fnv-interface})--->. Using this new system, children were tasked with checking the health of their VB through three interactions: pumping their VB’s heart, checking the major artery, and observing how quickly they completed tricks.

<!--- TODO: (see Figure ~\ref{fig:fnv-interface})--->
<figure>
  <img class=scale-w100 src="vbFV_interface.png">
  <figcaption>Figure 2. A play station for the VB-F\&V system (A, left), including the Novint Falcon haptic joystick (B, left). An example of the VB-F\&V virtual world, showing a VB and give paw trick (C, right), where the red sphere shown represents the virtual cursor controlled by the haptic joystick (B, left).</figcaption>
</figure>
<!--- \begin{figure}[h]
    \centering\includegraphics[width=0.9\textwidth,height=70mm,keepaspectratio]{figures/VFB-FnV/old_vfb_interface_example.png}
    \caption{A play station for the VB-F\&V system (A, left), including the Novint Falcon haptic joystick (B, left). An example of the VB-F\&V virtual world, showing a VB and give paw trick (C, right), where the red sphere shown represents the virtual cursor controlled by the haptic joystick (B, left).}
    \label{fig:fnv-interface}
\end{figure} --->

Each child needed to pump their VB’s virtual heart and feel the elasticity of their major artery (Figure 3)<!--- TODO: (Figure ~\ref{fig:fnv-heart}) --->. As their VB became healthier, it was easier to pump the heart as their VB’s artery became more elastic. They could feel the ease of pumping the heart and this elasticity as the amount of resistance provided by the haptic joystick as they pressed into the artery. The harder the heart was to pump and the less elastic the artery was, the more resistance was provided. In order to provide an on-screen representation of the VB’s health, a meter was displayed ranging from red to green in color, where red indicating that the VB’s health was low (Figure 3)<!--- TODO: (Figure ~\ref{fig:fnv-heart}) --->. This meter was intended to provide a visual reference point for the children to gauge the health level of their VB between interactions with them. Children then had their VB perform tricks, testing their VB’s mental health. As their VB became healthier, it was able to complete tricks more quickly. Although we did provide multiple VB-F\&V stations, we still designed the interactions to be short as the children only had a limited amount of time to play after lunch. We set these stations up in their own area near the cafeteria, making it easier for children to play with their VB following lunch. 

<!--- TODO: (Figure ~\ref{fig:fnv-heart}) --->
<figure>
  <img class=scale-w100 src="vbFV_heart_interface.png">
  <figcaption>Figure 3. The VB-F\&V heart pumping (A, left) and artery checking minigames (B, right). The sliders on the bottom left represent the health of the VB, ranging from min health (left/red) and max health (right/green).</figcaption>
</figure>
<!---
\begin{figure}[h]
    \centering\includegraphics[width=0.9\textwidth,height=70mm,keepaspectratio]{figures/VFB-FnV/old\_vfb\_heart\_interface\_example.png}
    \caption{The VB-F\&V heart pumping (A, left) and artery checking minigames (B, right). The sliders on the bottom left represent the health of the VB, ranging from min health (left/red) and max health (right/green).}
    \label{fig:fnv-heart}
\end{figure}--->

These minigames were designed to demonstrate tangible impacts a child’s F\&V consumption had on the health of their VB quickly. Due to their bond with their VB and seeing the impacts F\&V consumption has on their health, the child would be encouraged to consume more F\&V. Lastly, the health of their VB was intended to demonstrate those same impacts on their own health, which were on a much slower time scale than the impacts on their VB’s health. By making this real-world connection between F\&V consumption and health, the child may continue to consume more F\&V even beyond the scope of this study. 

### Results and Observations
We found that the VB-F\&V system was successful with treatment participants consuming significantly more F\&V than the control (no VB) groups [^a2016using]. We found that the children were excited to use the system and, thus, were not very delicate on the haptic joysticks even with supervision. Given the delicate and cumbersome nature of the haptic joysticks, we did not use them in a future system. Additionally, since the amount of F\&V consumed during lunch had to be manually calculated, it took a long time to incorporate every child’s results into the system. This caused frustration as they could not immediately play with their VB after they finished eating lunch. Lastly, given the success of the VB health check interactions, upcoming systems will use them as the basis for designing minigames for our participants to play with their VBs.

    
## Virtual Fitness Buddy - Summer Camp System

Based on prior systems [^j2014mixed] [^a2015using], the Virtual Fitness Buddy Camp (VFB-C) system was designed to encourage children to engage in healthier physical activity (PA) habits by providing them with a virtual fitness buddy (VFB). Similar to the Virtual Buddy Fruit and Vegetable (VB-F\&V) system, this system targeted children who were attending a weekly summer camp. It was deployed for 3 days and consisted of 67 children (ages 9 to 13) at a single summer camp in 2015, where 39 children were in the treatment (received points) condition and 28 children were in the control (received no points) condition [^a2019points]. The children were only able to interact with their VFB during the time that they were attending the camp.
    
Similar to the VB-F\&V system, the VFB-C system consisted of a customizable VFB, which became slimmer, faster, and able to perform more tricks as their child engaged in PA in the real-world. The only VFB customization available at this time was changing the VFB’s tag color. By tying the VFB’s health to the child’s PA, they could quickly see tangible benefits of their PA that were intended to reflect their own real-world health benefits, which sometimes can be hard to see overtime. For this new study, we switched to using a new PA tracker (the Fitbit Zip) instead of using the PA tracker from the original VFB (VFB-O) system. The Fitbit Zip also served as the method of logging into the system. By requiring these trackers to login, the child’s PA was downloaded prior to playing with their VFB, allowing them to be rewarded in real time rather than needing to wait for it to be manually uploaded as in the VB-F\&V study.
     
<!--- TODO: (Figure ~\ref{fig:vfbc-kiosk} (left)) --->
<!--- <figure>
  <img class=scale-w100 src="vfbC_kiosk.png">
  <figcaption>Figure 4. A child interacting with their VFB. The VFB-C mobile kiosk is shown on the left with the hover selection system shown on the right. The hover select cursor is shown as a pink circle on the right (located on the bottom of the image in the center near the VFB’s foot).</figcaption>
</figure>--->
<!---
\begin{figure}[h]
    \centering\includegraphics[width=0.9\textwidth,height=70mm,keepaspectratio]{figures/VFB-C/old\_vfb\_kiosk\_example.png}
    \caption{A child interacting with their VFB. The VFB-C mobile kiosk is shown on the left with the hover selection system shown on the right. The hover select cursor is shown as a pink circle on the right (located on the bottom of the image in the center near the VFB’s foot).}
    \label{fig:vfbc-kiosk}
\end{figure}-->
     
Each child played with their VFB using a mobile kiosk system, consisting of a large-screen TV and Microsoft Xbox360 Kinect (Figure 4 (left))<!--- TODO: (Figure ~\ref{fig:vfbc-kiosk} (left)) --->. The Kinect allowed us to track and to utilize the child’s real-world movements in order to interact with their VFB, intending to make them feel as if they were interacting directly with their VFB. These movements were mimicked by their virtual avatar, which was displayed as a collection of spheres on the side of the screen (see Figure 5) <!--- TODO: (see Figure ~\ref{fig:vfbc-skele}) --->. Our goal with using these real-world movements and moving the player’s avatar to be in proximity of the VFB was to help foster a bond between the child and their VFB, helping to satisfy the psychological need of relatedness [^d2012self]. 

<!--- TODO: (see Figure ~\ref{fig:vfbc-skele}) --->
<figure>
  <img class=scale-h50 src="vfbC_skeleton.png">
  <figcaption>Figure 5: An example of the virtual avatar used to represent the player. This avatar was displayed on the side of the screen.</figcaption>
</figure>
<!---
\begin{figure}[h]
    \centering\includegraphics[width=0.7\textwidth,height=60mm,keepaspectratio]{figures/VFB-C/old\_vfb\_skeleton\_example.png}
    \caption{An example of the virtual avatar used to represent the player. This avatar was displayed on the side of the screen.}
    \label{fig:vfbc-skele}
\end{figure} --->
    
Given that a single kiosk would be used for all of the participants, interactions with the VFB were designed to be short and intuitive. These interactions were modeled after behaviors that a real-world dog could perform, which included a throwing gesture used to play fetch and verbal commands in addition to a menu to initiate tricks. Following a command, the child would also need to complete the corresponding gesture to guide their VFB as they completed the trick. The VFB was able to fetch the ball and complete tricks faster as their health improved. These tricks were unlocked as the child earned points by meeting their PA goals. Each child was allowed to set and meet as many of these goals as they desired throughout the day. Lastly, they were not allowed to interact with their VFB again until they met their current PA goal. By allowing them to set their own goals, we gave each child autonomy over their experience, where they could gain a sense of mastery by meeting these goals more quickly. Additionally, we included the opportunity to give voice commands as a way to aid in improving participants' attachment to their VFBs.

In addition to these PA goals, we implemented a messaging system where a child’s parent would receive a text message when their child met one of these goals. If the parent responded to this message, their message would be displayed for the child the next time they played with their VFB. This messaging system was intended to serve as additional encouragement for a child to meet their PA goals and as another avenue to foster a sense of connectedness to their parents.

### Results and Observations

During the previous study, there was a significant difference in PA outcomes for the treatment group over the control (no VFB) group [^j2014mixed] [^a2015using]. However, this new VFB-C system only briefly increased PA. The children set significantly less vigorous PA goals while setting significantly more light intensity PA goals when compared to the control (no point) group. This is likely a result of all goals rewarding the same number of points regardless of PA intensity [^a2019points]. 

From field observations, we found that it was difficult for the system to detect voice commands as the kiosk was placed near the cafeteria, which was a loud area of the camp. Additionally, we had trouble detecting who was trying to log into the VFB-C system using their Fitbit. In our lab tests, we noticed a problem where it was difficult to isolate the single Fitbit that we were using to login. Thus, we implemented an icon-based list for the detected Fitbits to address this problem. However, once the system was deployed in the field, these detection issues arose again. We suspect that the system was overwhelmed with the number of active Fitbits in close proximity. Lastly, we implemented a mid-air, dwell (“hover”) selection system (see Figure 4 (right)), where a child would put a hand out in front of them and move it around to hover over the desired selection for a few seconds. This system was used to select the desired child from a list, set PA goals, and select a trick to buy and perform. We found that it was difficult and cumbersome for the children to use.

Given the success of the VFB-C system in encouraging children to engage in PA, we based our subsequent systems on it. These new systems expanded and improved this VFB-C system, adding more minigames for children to play with their VFB and ways to interact with the system itself. These PA-based systems will be explored in more detail in Chapters 4 and 5. The VFB-C system was also used as inspiration for a virtual buddy system designed to aid children in understanding various science, technology, engineering, and math (STEM) concepts. This system will be discussed further in Chapter 4.

Not only was the system a success in encouraging PA, the mobile kiosk was a robust design that was easy to break down for transport and withstood being used by the children at the camp without issue. Additionally, the kiosk was easily setup as it only needed to be plugged into power with a single cable for use everyday at the camp. For these reasons, this kiosk system would also be used in the studies in the upcoming chapters.

## Conclusions and Lessons Learned

Across both of these studies we learned several lessons to apply going forward. First, from the VB-F\&V intervention, we realized that children excited to play with their VBs are more likely to be rough on study hardware, meaning we should choose hardware that would be robust enough to sustain interactions across the duration of the desired study. In turn, this also could afford us the ability to leave hardware at a given site to be used without our personal observation, which, in turn, could increase the number of sites that could be using the VB system at a given time. We also realized how frustrating it was for the participants to have to wait for us to upload their data in order to play with their VFB. For future VB systems, autonomous data uploading and downloading was given a much higher priority. 

Second, from VFB-C intervention, we discovered how difficult it was for the Kinect to detect participants' voice commands due to the ambient noise level from all of the individuals attending the summer camp. We kept this lesson in mind when planning where future VB stations should be setup and when designing future trick systems, where there should be an alternative way to initiate games or tricks in case the system has difficulties in hearing and understanding participants' verbal commands. Additionally, we realized that having a system function where a participant could simply walk up and play may be more difficult than we previously thought due to hardware limitations. This meant that we should more thoroughly consider the mechanism by which participants would login to play with their VBs rather than simply trying to rely on the strongest signal. We also realized how difficult it was for participants to use the mid-air hover selection system, meaning we should design different input mechanisms for future VB systems.

Lastly, the mobile kiosk, Fitbits, skeletal avatar, parent messaging, and the point-based system were all a success. As previously mentioned, the kiosk was easily assembled and operated without issues across the VFB-C study, meaning it required little from site staff to setup and maintain. Many of the children in the VFB-C study were excited to receive Fitbits despite our struggles with Fitbit detection. All of these features would be reused in the studies discussed in the upcoming chapters.
      
[^diss]: Ball, Catherine. Design and Field Implementation of Virtual Buddy-Based Serious Games for Children. Diss. University of Georgia, 2023.
[^j2014mixed]: Johnsen, Kyle, et al. "Mixed reality virtual pets to reduce childhood obesity." IEEE transactions on visualization and computer graphics 20.4 (2014): 523-530.
[^a2015using]: Ahn, Sun Joo, et al. "Using virtual pets to promote physical activity in children: An application of the youth physical activity promotion model." Journal of health communication 20.7 (2015): 807-815.
[^a2019points]: Ahn, Sun Joo, Kyle Johnsen, and Catherine Ball. "Points-based reward systems in gamification impact children’s physical activity strategies and psychological needs." Health Education & Behavior 46.3 (2019): 417-425.
[^a2016using]: Ahn, Sun Joo, et al. "Using virtual pets to increase fruit and vegetable consumption in children: A technology-assisted social cognitive theory approach." Cyberpsychology, Behavior, and Social Networking 19.2 (2016): 86-92.
[^d2012self]: Deci, Edward L., and Richard M. Ryan. "Self-determination theory." Handbook of theories of social psychology 1.20 (2012): 416-436.
