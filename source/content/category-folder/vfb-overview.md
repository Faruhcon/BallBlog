---
title: Virtual Fitness Buddy Overview
#issueNo: 1
---

<div class="article-header">

# What is the Virtual Fitness Buddy?

</div>

<img src="vfbH_frisbee1.png" width="600" height="400"> 

TODO: Center and caption, resize?
is there already a concept of figure or do I need to make one?

I was a core developer for the Virtual Fitness Buddy (VFB) system and its prototypes for nearly a decade, ending with my graduation from the University of Georgia in Fall 2023. The guiding priciple for the VFB system is to encourage children to engage in healthier physical activity (PA) habits. This was achieved using a customizable virtual dog and a PA tracker. As a child engaged in PA, their VFB could play for longer and could unlock new minigames and tricks to perform. As that child met their daily PA goals, they would earn points to purchase VFB and toy customizations. This distinction was made so that all PA would be rewarded in becoming healthier while still encouraging the child to set realistic PA goals without penalizing them from new playable content. During this time, we grew this system from our pilot studies at a single summer camp site with xxx children total to yyy children across zzz sites utilizing a mulimillion dollar grant.

TODO navigations buttons here too or just below?

## My Responsibilities

Given our team size, I performed many tasks for the Virtual Fitness Buddy (VFB) project over its life cycle ranging from brainstorming initial designs to deploying it on-site. For simplicity, I have condensed these tasks into the following roles:

- Programmer
- Game Designer
- UI/UX Designer
- Hardware Designer
- QA
- Development Team Lead
- Data Engineer
- On-site/Field Consultant
- Tech Support

TODO navigations buttons here too???

TODO: add subheaders for each of the roles above?? with links in the above list to these subsections with even more info than is contained in the paragraphs below? Markdown headings to autogenerate list?

Additional information regarding these roles are enumerated in the following sections.

### Programmer

- designed intuitive interface for children that required 0 training
- designed interface that stayed working with no problems for 5 years** maybe hardware
- Unity3D application scripting was largely me (C#)
- iOS, VR, AR, and PC development
- SQL to interact with database and query it
- Python/Pandas for data analysis and visualizations
- Minigames
- user controls
- VB behavior (state machine)
- game loop
- user input processing
- UI
- retrieving/uploading/processing data
- Game script architecture design
  - MVC and MVVM approaches
  - make user controls independent of agent behavior
    - easier to swap out hardware without having to change a million different broken scripts
    - easier to swap other stuff too
- Worked with navigation meshes
- Data architecture design (JSON)
- Audio execution and looping
- Terrain design and some optimizing
- Some shader knowledge
- Basic database interactions
- Remote viewing/updating
- Created and mainted both control and treatment applications


### Game Designer

- Overlap with UX
- translated "abstract" study goals into game concepts
- designed games to fit time and hardware constraints
- translated real world concepts into game mechanics
  - intuitive system
- Trophy system
  - built in reward for meeting daily PA goals
  - incentive for setting and meeting higher PA goals
  - also quick visual feedback on meeting PA goals
- Bones as decoration --> dog themed
- Dog house as VFB starting point
  - give consistent place to start
  - VFB doesn't just pop into existence
- Agility course design and scoring
- Frisbee mechanics
  - decaying value over time
- minigames designed to have it easier to get higher score as VFB becomes healthier (faster)
  - faster to return ball (Basketball, Frisbee, Soccer)
  - run through agility course faster
  - Easier to return volleyball serves 
    - helps for the cooperative mode
    - would make competitive harder
  - Made Bark It harder because more tricks to remember
    - Theoretical fix would link VFB health to random less skill-based with random fails
      - As VFB health increases, so would the maximum guaranteed trick completion succcesses
    - OR easier to teach tricks as VFB health increases
- Lever hero updates: auto balancing vs intentional balancing
- Minigame design choices
- Dabbled with art and audio design
- Tweaking game mechanics to better fit time constraints
- VSB needed better tutorial where the VSB was more involved and interactive

### UI/UX Designer

- designed interface in case things went wrong with instructions on how to fix
- VFB-C cursor mode
- Shot zones? (gestures/throwing)
- Multiple ways to trigger something
  - Optional voice activation
  - or menu selection
- Touchscreen select with motion controls --> more intuitive
- 3D Keyboard
- Shop Menu
- Inventory and Inventory Menu
- Blaster?
- Trophy System
- Login Mechanisms
- VFB-H Popup menus
- VFB-H in world menus for minigames
- Buddy naming and customizations
- Grab and other gestures
- Virtual Joysticks
- Updated interaction systems based on user feedback
- power meter/other meters to have visual representation of otherwise ambiguous measurements/values
- navigation arrow to show where to go
- multiple ways to let user know that they are in the correct location
  - audio chime
  - particle effect
  - visual cue
    - spot on ground
    - color change
    - guide arrow disappears
- real world concepts --> baked into minigame mechanics
- kiosk design --> low maintenance by staff ("self-contained")
- Agility course route indicators
- App relaunch software in case of crash
- audio and text for CMOA in case user without parents and cannot read (well)
- haptics for F&V
- Leverage common application mechanics (virtual joysticks)
- Messaging?
- Environmental considerations --> safety, convenience, voice
- Voice control as easter egg because of environmental noise levels and mic location
- Changing lever hero from auto balance to balance when placed
  - less convenient but enforced the learning mechanics more
- Trajectory for slingshot shown --> higher difficulties would be removed or shortened
- Data syncing evolution
  - sync on login so immediate feedback
  - became problem because of extended study duration so had more data to sync which then prevented folks from logging in
  - sync in background instead
    - still had issues with extended syncing times
  - sync with different application so as to not obstruct login
- family review fail
  - idea was to try to get kids to bug parents to go over what they had done, reinforcing the study goals
  - failed to achieve this and then kids were demotivated because they could not see the impact of their physical activity until review happened
  - plan would be to change this and maybe add something like a multiplier to points for completing family review
    - similar logic to VFB health and point split for PA and meeting goals
- PA rewards split --> All PA rewarded but goals earn points (study target)
- Leaderboards
  - both overall and recent so folks behind at first would be less discouraged
  - utilized to encourage competitive folks
  - both for PA and scores
  - for individual, family when applicable, site when application, and overall study if opted in
- virtual kiosks scalable to accommodate more game modes
- translating study goals into actionable game designs
- lever hero rotate arrows as visual aids
- Adapting motion/kinect minigames to iPad controls
  - broadened what we could do
- show upcoming unlocks as additional incentive 

### Hardware Designer

- Based on study goals and environmental constraints
- Hide cabling --> to help avoid hardware failures
- Mobile to make easier to get out of the way for school day
- Wood and metal design so wireless signals are less blocked 
- Kiosk not practical in home --> iPad instead
- Touchscreen >>> mid air interactions
  - intuitive
  - familiarity
  - ease of use
  - more precise
- Should largely be self-contained
  - reduce site staff burden
- Kids hard on sensitive hardware
  - Novint Falcon fail (VB-F&V)
- Able to accommodate a lot of throughput
- VSB ran years without fail except for early hardware hiccups
  - graphics card fail *2 (faulty? --> overheat)
  - twist cord break
- Fail: VFB-A could not auto on TV because hardware limitation was not considered while purchases were being made for kiosk
- Reduce points of failure
- Robust system 
  - How to do VR with minimal supervision???
- VFB sites run with minimal aid across many sites
- Syncing fail?
- Minimize unwanted use of hardware
  - ex: watch youtube on pc
  - solution: hide keyboard and mouse inside locked kiosk 

### QA

- lab testing for hardware and software

### Development Team Lead

- Lead a team of undergraduate artists and programmers for VFB-A
- art direction aid

### Data Engineer

- Designed data structure (JSON) for saving VFB data
  - for processing in game
  - for data analysis
- Processed data into easier analyzable format for larger data team
- Exploring data analysis approaches
  - looking at timing of events for clues
  - looking beyond basic play data into why this may have happened
  - connections to family reviews
  - control looking family review and level ups (because intrinsically linked)
  - how did relative minigame plays change over time?
    - because unlock timing?
    - fave game or variety of play?
- Both for quick idea analysis and deeper analysis
- Quick for game to down/upload and process

### On-site/Field Consultant

- would go out and visit sites in person
  - to observe and record how folks used systems
  - why fitbit syncing breaking?
  - hardware troubles

### Tech Support

- Fitbit setup
- Web troubles
- kiosk troubles
- fitbit tracking troubles

Expand on the list above with what I did for each role so folks know what they're getting when hiring me for these roles. Don't forget the buzzwords like SQL, etc

For this project, my primary focus was designing, programming, and testing the VFB Unity3D application itself, which included the script architecture, user interfaces, world layout, minigame implementation, data formatting and processing, and input control systems. I even dabbled with basic art and audio design. Basically, if you see it in the game, I more than likely had my hand in it. Additionally, I helped to design our second kiosk in terms of testing the potential new hardware and hardware upgrades for feasibility and assembly. Lastly, while we largely had two developers for these apps, I did lead a team of undergrads consisting of both programmers and artists for some time.

In terms of the overall study, I had additional responsibilites while working with our interdisciplinary team. Since I was one of the primary developers, I was tasked with system troubleshooting both remotely and on-site once our systems were deployed in the field, communicating with site directors for any issues or pain points that they noticed. I also was a primary tech support when a parent and/or child had any issues with data entry or PA trackers, walking parents through tracker setup when necessary. For our statisticians, I aided in gathering system and application data, getting the desired data into a more readily processible format. For our psychologists and kinesiologists, I translated study goals into actionable application elements. Lastly, I both designed the program to perform data analysis and analyzed gameplay metrics, looking for information on what to adjust for future versions of the VFB system.  

Header: Overall Study Statistics? or maybe something like additional study info? and include both the study metrics and then the system setup over time? then a chart like has minigames? focus? etc

Insert discussion and chart for overview of participant data across all of the VFB studies

Header: ??? System Overview --> change to

insert the kiosk, ipad, and headset pictures here? or break them up between paragraphs? which looks better

Various systems were used throughout the lifetime of the VFB project. Our first two systems (refx2?) utilized a mobile kiosk which consisted of a large screen TV along with a PC and Microsoft Kinect (ref?), where children used their physical bodies as the primary method of interacting with their VFB (fig ref?). The idea was to avoid having the children engage in sedentary activity when playing with their VFB while also mimicking real life motions to aid in fostering the bond between a child and their VFB. From both these early studies and the Virtual STEM Buddy (VSB) (make into link to its page) project, we learned that utilizing a touchscreen for more complex selection interactions was much easier and understandable over mid-air interaction techniques with the Kinect. Thus, we added a touchscreen to the second iteration of our kiosk (fig ref?).

These kiosks were designed to be used in public spaces. Thus with the onset of the COVID pandemic, we needed to change our approach to continue conducting these studies. This resulted in our iPad iteration of the VFB system (ref) (fig ref?). We sought to keep as much of the real-world movement as possible, utilizing augmented reality (AR) techniques for camera movement and aiming while utilizing the touchscreen through the use of digital joysticks and buttons for locomotion and throwing. Additionally, we were better able to utilize voice activated interactions for performing tricks as the microphone would be close to the child while they interacted with their VFB. This shift allowed the VFB system to be usable in many different home setups.

The last iteration of the VFB system I worked on was the immersive, virtual reality (VR) based system which utilized the Meta Quest 2 (dissertation ref?). We returned to the real world movement of our kiosk-based VFB systems, adapting several of the minigames to the new explorable VFB world designed for the iPad-based VFB system. I also briefly worked on early prototypes of the watch companion app that was in development as I was graduating. This was an idea my professor and I had talked about for a long time. The watch app would allow children to take their VFB with them on walks, which we thought would help foster their bond.

For, more detailed information on each of our VFB iterations, please use the buttons below to navigate to the desired page.

Add buttons here

Add references to papers here as footnotes?

Some additional notes:

While all version of vfb had voice activation, it was often hard to use in the afterschool settings because loud

Our second iteration of this kiosk added a touchscreen because mid air interaction hard

This journey began in summer camp settings

more details for each of these projects can be found...

learned and grew from the older projects and also vb-f&v and vsb-m, which will be discussed in more detail on the following pages

something something (on the specific page for it): tried to have the physical fitness go down but we were too harsh on it and for the sake of the study, opted to remove this feature as we did not have time to properly test it in the lab before the next iterations

vb-f&v offshoot/spinoff of VFB projects

Something something more details on the following pages and add buttons

click here for the narrative history

history of VFB page in lieu of individual pages for each project?
About me and "cv" pages? one click link on how to make me stand out as a good candidate


# Job Win Notes

- ???
- win is one sentence to impress someone who wants to hire you






| Project Name         | Virtual Buddy Fruit and Vegetable (VB-F&V) | Virtual Fitness Buddy Camp Intervention (VFB-C) | Virtual STEM Buddy Museum Intervention (VSB-M) | Virtual Fitness Buddy Afterschool Intervention (VFB-A) | Virtual Fitness Buddy At-Home Intervention (VFB-H) |
| ------------ | ------------------------------------------ | ----------------------------------------------- | ---------------------------------------------- | ------------------------------------------------------ | -------------------------------------------------- |
| Date         | Summer 2014                                | Summer 2015                                     | January 2017 to May 2022                       | Spring 2018 to Fall 2019                               | Fall 2021 to Spring 2022                           |
| Location     | Summer Camp                                | Summer Camp                                     | Children's Museum of Atlanta (CMOA)            | Afterschool Programs                                   | At-Home                                            |
| Sites        | 1                                          | 1                                               | 1                                              | 11 Treatment (21 Total)                                | N/A                                                |
| Cohorts      | 1                                          | 1                                               | 1                                              | 3                                                      | 2                                                  |
| Total Duration     | 3 Days                                     | 3 Days                                          | 5 Years                                        | 1 Year                                    | 9 Months                                         |
| Participants | 25 Treament (68 Total)                     | 67 Treatment                                    | Unknown – 28,122 recorded plays over 2 years   | 318 Treatment (464 Total)                              | 25 Treatment (44 Total)                            |
| Focus        | Fruit and Vegetable Consumption            | Physical Activity                               | STEM Education                                 | Physical Activity                                      | Physical Activity                                  |
| Controls     | Haptic Joystick                            | Motion and Voice                                          | Motion, Touch, and Voice                       | Motion, Touch, and Voice                               | Motion, Touch, and Voice                           |