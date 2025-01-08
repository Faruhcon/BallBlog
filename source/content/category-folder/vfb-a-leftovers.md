---
title: VFB-A Leftovers
draft: true
---

<!--- ~\ref{fig:vfba-basic-game-plays-perDay-plays} --->
<figure>
  <img class=scale-w100
    src="vfbA_C2_gamePlays-perday_byGame.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 11. Graphs depicting the number of plays controlled for number of days unlocked for each game played during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/Results_C2-A/C2_gamePlays-perday_byGame.png}
    \caption{Graphs depicting the number of plays controlled for number of days unlocked for each game played during C2-A.}
    \label{fig:vfba-basic-game-plays-perDay-plays}
\end{figure} --->

<!--- ~\ref{fig:vfba-basic-game-plays-perDay-time} --->
<figure>
  <img class=scale-w100
    src="vfbA_C2_timeplayed-perday_byGame.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 12. Graphs depicting the amount of time played controlled for number of days unlocked for each game played during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/Results_C2-A/C2_timeplayed-perday_byGame.png}
    \caption{Graphs depicting the amount of time played controlled for number of days unlocked for each game played during C2-A.}
    \label{fig:vfba-basic-game-plays-perDay-time}
\end{figure} --->

It is plausible that Volleyball was played for approximately an hour each day given that there were 4 sites and 124 participants. However, both Volleyball and Slingshot did not have a time limit on how long they could be played for a single game, and we did not implement a force logout feature. This means that if a participant walked away from the kiosk during either of these minigames and no other participant logged in, these games would run until the kiosk was shutdown for the day as our intended exit for these games was for a participants' VFB to run out of energy. However, the VFB only used energy while it was running, which it would not do if no one threw a toy for it to fetch. This combination of factors could account for the play differences between these two minigames and Basketball and Soccer, which had time limits of 60 real-world seconds. As shown in Table 2<!---TODO: Table ~\ref{table:vfba-minigame-play-times} --->, about two-thirds of game plays ended in 60 seconds or less and around 99\% of game plays ended in 300 seconds (5 minutes) or less. However, there are 13 plays which exceeded 17 minutes (1000 seconds). 

<!---TODO: Table ~\ref{table:vfba-minigame-play-times} --->
| Play Duration (s) | \# Game Plays | % of Total Plays |
| ----------------- | ------------- | ---------------- |
| No Limit          | 1461          | 100%             |
| <= 60s            | 893           | 61.12%           |
| <= 180s           | TODO:         | 94.73%           |
| <= 300s           | TODO:         | 98.63%           |
| <= 1000s          | 1448          | 99.11%           |
| \> 1000s          | 13            | 0.89%            |
<i>Table 2. Number of all minigames played at different play times.</i>

<!--- \begin{table}[!htbp]
    \centering
    \begin{tabular}[c]{|c|c|c|c|c|c|c|}
        \hline
        Play Duration (s) & \# Game Plays & \% of Total Plays\\
        \hline
        No Limit & 1461 & 100\%\\
        \hline
        <= 60s & 893 & 61.12\%\\
        \hline
        <= 180s & 893 & 94.73\%\\
        \hline
        <= 300s & 893 & 98.63\%\\
        \hline
        <= 1000s & 1448 & 99.11\%\\
        \hline
        > 1000s & 13 & 0.89\%\\
        \hline
    \end{tabular}
    \caption{Number of all minigames played at different play times.}
    \label{table:vfba-minigame-play-times}
\end{table} --->

Given this information, we implemented time limits for the max amount of time played for further analysis. Each play was still counted, but if the play time exceeded the limit, the time for that play would be capped at the time limit. Figure 13 <!--- TODO: Figure ~\ref{fig:vfba-timelimited-game-plays-5} --->shows the amount of time played with a 5 minute time limit and Figure 14 <!--- TODO: Figure ~\ref{fig:vfba-timelimited-game-plays-1} --->shows the amount of time played with a 1 minute time limit. With both limits, Slingshot at least 3 times as much play time as the rest of the minigames. Limiting plays to the max time allowed for Basketball and Soccer (60 seconds), Soccer and Volleyball have similar play times with Basketball at around half of their play time.  

<!--- TODO: Figure ~\ref{fig:vfba-timelimited-game-plays-5} --->
<figure>
  <img class=scale-w100
    src="vfbA_C2_timeplayed_byGame-5minMax.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 13. Graph depicting the amount of time played limited to 5 minutes per play for each game during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/Results_C2-A/C2_timeplayed_byGame-5minMax.png}
    \caption{Graph depicting the amount of time played limited to 5 minutes per play for each game during C2-A.}
    \label{fig:vfba-timelimited-game-plays-5}
\end{figure} --->

<!--- TODO: Figure ~\ref{fig:vfba-timelimited-game-plays-1} --->
<figure>
  <img class=scale-w100
    src="vfbA_C2_timeplayed_byGame-1minMax.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 14. The VSB Kiosk at the Children’s Museum of Atlanta.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/Results_C2-A/C2_timeplayed_byGame-1minMax.png}
    \caption{Graph depicting the amount of time played limited to 1 minute per play for each game during C2-A.}
    \label{fig:vfba-timelimited-game-plays-1}
\end{figure} --->

Figures 15 and 16 <!--- TODO: Figures ~\ref{fig:vfba-timelimited-game-plays-perDay-5} and ~\ref{fig:vfba-timelimited-game-plays-perDay-1} --->depict the amount of time played controlling for the number of days each participant had each minigame unlocked limited to 5 minutes and 1 minute of play, respectively. The overall trend is similar to the overall play time data. With a 5-minute max time limit, Slingshot has the most play time followed by Volleyball then Soccer and finally Basketball. With a 1-minute max time limit, Slingshot still has the most play time followed by Soccer and Volleyball with Basketball having the least play time. Thus, even accounting for the number of days unlocked, Slingshot still has the most amount of play time and Basketball has the least. All of this seemingly indicates that participants preferred Slingshot the most, Volleyball and Soccer approximately the same, and Basketball the least. 

<!--- TODO: Figures ~\ref{fig:vfba-timelimited-game-plays-perDay-5} --->
<figure>
  <img class=scale-w100
    src="vfbA_C2_timeplayed-perday_byGame-5minMax.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 15. Graph depicting the amount of time played controlled for number of days unlocked and limited to 5 minutes per play for each game during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/Results_C2-A/C2_timeplayed-perday_byGame-5minMax.png}
    \caption{Graph depicting the amount of time played controlled for number of days unlocked and limited to 5 minutes per play for each game during C2-A.}
    \label{fig:vfba-timelimited-game-plays-perDay-5}
\end{figure} --->

<!--- TODO: Figures ~\ref{fig:vfba-timelimited-game-plays-perDay-1} --->
<figure>
  <img class=scale-w100
    src="vfbA_C2_timeplayed-perday_byGame-1minMax.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 16. Graph depicting the amount of time played controlled for number of days unlocked and limited to 1 minute per play for each game during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/Results_C2-A/C2_timeplayed-perday_byGame-1minMax.png}
    \caption{Graph depicting the amount of time played controlled for number of days unlocked and limited to 1 minute per play for each game during C2-A.}
    \label{fig:vfba-timelimited-game-plays-perDay-1}
\end{figure} --->

However, as mentioned earlier, Slingshot was the only game available to play for around the first month of the study with Soccer and Volleyball being the last two games to unlock. As shown in Figure 17 <!--- TODO: Figure ~\ref{fig:vfba-weekly-plays}--->, Slingshot has many more plays in roughly the first two-thirds of the study compared to the other games. The update unlocking the ability to play Basketball, Soccer, and Volleyball occurred between weeks 4 and 5 of the study. However, this does not mean that every participant was able to play these games immediately as they still needed to meet the requisite VFB level in order to unlock them. There is an overall trend of less games played over time. However, this is a small spike of plays the week following Thanksgiving break on week 11. Potentially, this could mean that participants were excited to play with their VFB again after a week without access.

<!--- TODO: Figure ~\ref{fig:vfba-weekly-plays}--->
<figure>
  <img class=scale-w100
    src="vfbA_C2_gamePlays_byGame-perWeek.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 17. Graph depicting minigame plays per week during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=120mm,keepaspectratio]{figures/Results_C2-A/C2_gamePlays_byGame-perWeek.png}
    \caption{Graph depicting minigame plays per week during C2-A.}
    \label{fig:vfba-weekly-plays}
\end{figure}--->

Figure 18 <!--- TODO: Figure ~\ref{fig:vfba-weekly-plays-perDay} --->depicts the number of games played per week controlling for the number of days each minigame was available to play for each participant. After roughly week 8, Soccer and Volleyball both have more plays per day unlocked than Slingshot with Basketball plays decreasing over time as these two games were unlocked. Additionally, the discrepancy between Slingshot and the other minigames is reduced once the number of days unlocked is considered. This means that Slingshot was still played more during the first half of the study but the other games were played proportionally more once days unlocked are considered.

<!--- TODO: Figure ~\ref{fig:vfba-weekly-plays-perDay} --->
<figure>
  <img class=scale-w100
    src="vfbA_C2_gamePlays-perday_byGame-perWeek.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 18. Graphs depicting minigame plays controlled for number of days unlocked per week during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=120mm,keepaspectratio]{figures/Results_C2-A/C2_gamePlays-perday_byGame-perWeek.png}
    \caption{Graphs depicting minigame plays controlled for number of days unlocked per week during C2-A.}
    \label{fig:vfba-weekly-plays-perDay}
\end{figure} --->
        
Finally, all of this data seems to indicate that Basketball is the least preferred minigame as it never had the most plays over time. It would be worthwhile to explore what led to this outcome. Potentially, this could be attributed to the shot zone mechanic being difficult for our participants to use as none of the other minigames utilized this feature. Slingshot used the grab and release mechanic from the Virtual STEM Buddy's (VSB) Slingshot minigame, and both Soccer and Volleyball used the new paddle mechanic developed for C2-A. This would also mean that the grab and release mechanic was relatively successful as it was during the VSB study and that the paddle mechanic would be another mechanic to utilize for other games during future studies given that both Soccer and Volleyball exceeded Slingshot in plays as the study progressed.

### Participant Play Metrics

To determine if there were game play outliers that may be skewing our play data, we also looked at the number of plays for each participant both in terms of overall plays (Figure 19) <!--- TODO: (Figure ~\ref{fig:vfba-participant-play-info}) --->and controlling for number of days each minigame was unlocked (Figure 20) <!--- TODO: (Figure ~\ref{fig:vfba-participant-play-info-per})--->. There are participants who played more games but not to a degree that one would be considered at outlier.

<!--- TODO: (Figure ~\ref{fig:vfba-participant-play-info}) --->
<figure>
  <img class=scale-w100
    src="vfbA_C2_gamePlays_byMem.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 19. Graph depicting the number of plays for each participant during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/Results_C2-A/C2_gamePlays_byMem.png}
    \caption{Graph depicting the number of plays for each participant during C2-A.}
    \label{fig:vfba-participant-play-info}
\end{figure} --->

<!--- TODO: (Figure ~\ref{fig:vfba-participant-play-info-per})--->
<figure>
  <img class=scale-w100
    src="vfbA_C2_gamePlays-perday_byMem.png"
    alt="TODO:"
    title="TODO:">
  <figcaption>Figure 20. Graphs depicting the number of plays controlled for days unlocked for each participant during C2-A.</figcaption>
</figure>
<!--- \begin{figure}[!htbp]
    \centering\includegraphics[width=0.99\textwidth,height=100mm,keepaspectratio]{figures/Results_C2-A/C2_gamePlays-perday_byMem.png}
    \caption{Graphs depicting the number of plays controlled for days unlocked for each participant during C2-A.}
    \label{fig:vfba-participant-play-info-per}
\end{figure} --->
    
<!--- \FloatBarrier--->

## Conclusions

Overall, we did see a decline in game plays over time. We suspect that there were not enough customizations and/or minigame options and/or that the existing customizations and minigames were able to be unlocked too quickly to sustain interest over the course of several months. Our small team combined with our shortened timeline compared to professional game development makes it difficult to design, create, and implement many VFB customizations and minigames prior to the beginning of our studies. Additionally, given this shortened timeline for development, it was difficult to test the reasonability of the rate at which the VFB leveled up, participants earned points and unlocked customizations/minigames, or points were scored during each minigame in our lab prior to running our studies. 

Additionally, there was a unique circumstance for each study which may have also contributed to this decline in engagement. The pilot study was effectively a testing ground for the new system. We tested and updated much of our core code during this time. For C1-A, participants had much difficulty in leveling up their VFBs as we had implemented a system where they could also level down, mimicking how our bodies fluctuate based on our PA habits. The rate at which VFB levels decreased was too extreme. By the time we realized this, it was already too late in the study. It makes sense that participants would be less motivated to continue engaging with the VFB-A system if they were unable to make reasonable progress over time. For all future studies, VFBs were only allowed to level up so that this did not happen again. C2-A was interrupted by the COVID-19 pandemic about halfway through the study at the beginning of 2020. As schools shut down and children transitioned to online learning, they could no longer access the VFB-A system. We were unable to test the effects of our new updates as a result.

While engagement was reduced overall, participants continued to interact with their VFB throughout Cohort 2. As a result, this indicates that participants were still excited to interact with their VFB throughout the study. Participants played a variety of minigames throughout the course of the study with Slingshot receiving more plays early in the study and Soccer and Volleyball receiving more plays as the study progressed. This provides support for participants preferring a variety of games to play or other activities to do over time. With this knowledge, we would expand the number of games available to participants for our next study. 

### Fitbit Physical Activity Syncing

Fitbit syncing problems continued to plague us throughout all of these studies. Given our issues detecting Fitbits during the VFB-C study, we tried testing if we could reliably detect Fitbits within a certain physical distance from the kiosk. However, there were troubles detecting the closest Fitbit in the field. With further experimentation, we found that the value we were using to determine this distance was not consistent with real-world distance from the kiosk. With this in mind, we opted to have the system start looking for a participant’s specific Fitbit once they had already logged into the system for C1-A. However, we had issues where the Fitbit would not always maintain a connection to the computer while syncing, which was largely due to participants not always syncing consistently and, as a result, having a lot of data to sync at once. This caused the Fitbit to no longer broadcast a signal for approximately 5 minutes. Since we required the Fitbit to be recently synced in order to play with their VFB, our participants either had to wait or try soft resetting their Fitbit (which was also difficult) to try again. Obviously, this caused a lot of frustration for our participants. For C2-A, we returned to detecting and syncing nearby Fitbits in the background similar to the VFB-C system. This method seemed to work better than it had for the VFB-C study. However, we had issues where our detection process would crash, and the VFB-A system would need to be restarted. Although we did automate this restart process, this was still a big source of frustration for participants.

<!--- %With this in mind, we would no longer have our VFB application perform the physical activity (PA) data syncing. Instead, we would utilize the Fitbit mobile app to perform these syncs rather than pursue fixes for these issues further. As discussed in the next chapter, this approach did not have the same pitfalls as we experienced during these studies. Thus, although it was a problem during these studies, we utilized this knowledge to adapt our approach for future studies. 

%Finally, it should be noted that the cause of our syncing issues was not due to failures with the Fitbits themselves nor with the Fitbit API. The crux of our syncing issues was due to our choice to have our VFB applications sync the Fitbit data as we needed to regularly sync hundreds of participants' Fitbits. This choice was made due to the quantity of Fitbits that needed to be regularly synced as part of our study while not adding additional 
%...steps that would cause delay in them interacting with VFB. But we also needed PA data to improve experiences.

%It would not have been practical for us to require participants to remember their Fitbit login information. in addition to using our app to sync many Fitbits at once.

%while we tried to leverage syncing at home with parents' devices, did not always happen causing a pile up of data to sync

%we did not have any issues with the Fitbit PA trackers nor with the Fitbit API. --->

## Lessons Learned

From the VFB-A studies, we learned that PA data should be synced prior to the user interacting with the system as it has caused numerous problems for many of our studies. Even with these PA syncing issues, it needs to be mentioned that we have not had any issue recruiting participants for these studies. The children and their parents are excited to receive their Fitbit and especially their VFB. Additionally, participants continue to engage with their VFB throughout the course of the study. Thus, it is not a matter of lack of interest in the VFB system. It is a matter of fitting the application design to the environment and audience while also having enough content to support extended use over time. Given that we have limited time to generate this content and that we have consistently revamped some major system for each subsequent study, it has been difficult to build up this pool of content that is required for sustained engagement. However, we have accumulated several mechanics and other approaches that would be useful for designing games and interactions for future studies with each subsequent iteration.
    
We would also use many of the minigame designs and implementations as a starting point for future minigames. For example, the paddle system used for Soccer and Volleyball seemed to work well in the field, and we would apply a similar system in the following study. We also learned that a precise aiming system would be beneficial to a game like Basketball where the goal is to get the ball to a precise location. Although we would no longer use the shot zone system, as it was hard for participants to understand and use the shot zones, especially without a researcher present to aid by explaining how they worked, they still inspired our aiming system used in the next study. Instead of shot zones, we would use a power meter with aiming by tilting the iPad, which is a mechanism also utilized by other mobile games. We would also continue to use the leaderboards we introduced as a part of this system as our participants enjoyed having these leaderboards available to compare scores and PA. 

Once again, this kiosk-based system was robust with a design inspired by the Virtual STEM Buddy (VSB) kiosk. We ensured that there was sufficient ventilation to keep the system running cool inside the kiosk cabinet and hid the majority of the cabling inside the kiosk itself. Across both cohorts, there was not a major hardware failure. This means that for 6 weeks at a single site during the pilot, for 6 months across 6 sites during cohort 1, and roughly 4.5 months across 4 sites during cohort 2 there was not a hardware failure. Not to mention, these kiosks were used by hundreds of children during that time. The only update we would recommend on this mobile kiosk design would be to ensure that the TV has the capability to turn on alongside the computer receiving power, as it had done for the VSB kiosk. Additionally, the combination of a touchscreen for menu selection alongside motion controls for interacting with the VFB continued to work well as it had for the VSB system. This combination would continue to be used for our next study although it would utilize an iPad for both the touch and motion controls in lieu of an independent touchscreen and Kinect.

