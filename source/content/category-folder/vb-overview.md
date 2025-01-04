---
title: Virtual Buddy Projects Overview
#draft: true
---

# TODO: Page Header

TODO: intro blurb

This page contains info on some of the virtual buddy applications that I built through the course of my PhD work. Primarily, this includes two major versions of the Virtual Fitness Buddy system and the Virtual STEM Buddy system, which encouraged children to engage in healthier exercise habits and to learn about various STEM concepts respectively. <!-- TODO: more specific info on these projects can be found on their individual pages (links). -->

TODO: find the vfb video I made?? should be on youtube
## Virtual Fitness Buddy at Home

### boop
>
<details open>
    <summary>VFB-H Info TODO: keep title?</summary>
    <figure class=img-fig>
        <img class=scale-w100 src="vfbH_interface_example.png">
        <figcaption>The VFB-H iPad interface.</figcaption>
    </figure>
    <p>The Virtual Fitness Buddy Home (VFB-H) project was designed to encourage children to engage in healthier physical activity (PA) habits through the use of a virtual dog buddy. As a child completed PA, tracked using a Fitbit PA tracker, their VFB's health would increase, which meant that they could play for longer, unlock new games and tricks, and earn points to spend on various customizations. VFB-H was built as an iPad app that children could use at home, utilizing touchscreen, voice-activation, and real-life motion as ways to interact with the system.</p>
    <details open>
        <summary>VFB-H Stats</summary>
        <div class="table-container">
            <table>
                <tbody>
                    <tr>
                        <td>Name</td>
                        <td>Virtual Fitness Buddy At-Home (VFB-H)</td>
                    </tr>
                    <tr>
                        <td>Dates</td>
                        <td>Fall 2021 to Spring 2022</td>
                    </tr>
                    <tr>
                        <td>Location</td>
                        <td>At-Home</td>
                    </tr>
                    <tr>
                        <td>Cohorts</td>
                        <td>2</td>
                    </tr>
                    <tr>
                        <td>Duration</td>
                        <td>4.5 months each</td>
                    </tr>
                    <tr>
                        <td>Participants</td>
                        <td>25 Treatment (44 Total)</td>
                    </tr>
                    <tr>
                        <td>Focus</td>
                        <td>Physical Activity</td>
                    </tr>
                    <tr>
                        <td>Controls</td>
                        <td>Motion, Touch, and Voice </td>
                    </tr>
                </tbody>
            </table>
        </div>
    </details>
    <!--- <figure class=img-fig>
        <img class=scale-w100 src="vfbA_petCustomizations_example.png">
        <figcaption>VFB coat, tag, collar, and hat customizations.</figcaption>
    </figure>
    <figure class=img-fig>
        <img class=scale-w100 src="vfbA_petToys_example.png">
        <figcaption>Toy options and customizations.</figcaption>
    </figure> --->
    <figure class=img-fig>
        <img class=scale-w100 src="vfbA_petCustomizations-and-toys.png">
        <figcaption>VFB coat, tag, collar, hat, and toy customizations.</figcaption>
    </figure>
    <p>As part of this app, I designed six different minigames: agility, bark it, basketball, frisbee, soccer, and volleyball. See below for more details on these games. I implemented leaderboards that would track their top 3 personal scores in addition to the top 3 scores for their family and across the entire study for each minigame. In addition to these games, children were able to get their VFB to perform tricks using their voice and could play fetch without having to interact with a minigame.</p>
    <details open>
        <summary>VFB-H Minigames</summary>
        <!--- VFB-H Minigame Table --->
        <!--- Agility --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vfbH_agility_example.png">
            </div> <!--- End Pic --->
            <div class="mgTable-list"> <!--- List --->
                <p class="mgTable-title">Agility</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Obstacle course</li>
                    <li><u>Goal:</u> Guide VFB through obstacles as quickly as possible</li>
                    <li><u>Scoring:</u> Time remaining on 60 second timer</li>
                    <li><u>Controls:</u> Virtual joystick (touchscreen)</li>
                    <li><u>Aids:</u> Guide arrow to next obstacle</li>
                </ul>
            </div> <!--- End List --->
        </div> <!--- End Table Cell --->
        <!--- End Agility --->
        <!--- Bark It --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-listLeft"> <!--- List --->
                <p class="mgTable-title">Bark It</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Trick memory game</li>
                    <li><u>Goal:</u> Complete longest trick streak</li>
                    <li><u>Scoring:</u> Number of correct tricks performed</li>
                    <li><u>Controls:</u> Voice or touchscreen</li>
                    <li><u>Aids:</u> Guide arrow to stage</li>
                </ul>
            </div> <!--- End List --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vfbH_barkIt2_example.png">
            </div> <!--- End Pic --->
        </div> <!--- End Table Cell --->
        <!--- End Bark It --->
        <!--- Basketball --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vfbH_basketball_example2.png">
            </div> <!--- End Pic --->
            <div class="mgTable-list"> <!--- List --->
                <p class="mgTable-title">Basketball</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Goal throws from random locations game</li>
                    <li><u>Goal:</u> Maximize basketballs scored in 60 seconds</li>
                    <li><u>Scoring:</u> Goals scored</li>
                    <li><u>Controls:</u> Virtual joystick and buttons (touchscreen) and iPad AR movement</li>
                    <li><u>Aids:</u> Guide arrow to next location and hoop</li>
                </ul>
            </div> <!--- End List --->
        </div> <!--- End Table Cell --->
        <!--- End Basketball --->
        <!--- Frisbee --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-listLeft"> <!--- List --->
                <p class="mgTable-title">Frisbee</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Balloon popping game</li>
                    <li><u>Goal:</u> Maximize balloons popped in 60 seconds</li>
                    <li><u>Scoring:</u> Sum of balloon values plus VFB catch bonuses</li>
                    <li><u>Controls:</u> Virtual buttons (touchscreen) and iPad AR movement</li>
                    <li><u>Aids:</u> Guide arrow to current balloon</li>
                </ul>
            </div> <!--- End List --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vfbH_frisbee_example.png">
            </div> <!--- End Pic --->
        </div> <!--- End Table Cell --->
        <!--- End Frisbee --->
        <!--- Soccer --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vfbH_soccer_example.png">
            </div> <!--- End Pic --->
            <div class="mgTable-list"> <!--- List --->
                <p class="mgTable-title">Soccer</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Goal kicks from random locations game</li>
                    <li><u>Goal:</u> Maximize soccer balls scored in 60 seconds </li>
                    <li><u>Scoring:</u> Goals scored</li>
                    <li><u>Controls:</u> Virtual joystick and buttons (touchscreen) and virtual paddle using iPad AR movement</li>
                    <li><u>Aids:</u> Guide arrow to next location and goal</li>
                </ul>
            </div> <!--- End List --->
        </div> <!--- End Table Cell --->
        <!--- End Soccer --->
        <!--- Volleyball --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-listLeft"> <!--- List --->
                <p class="mgTable-title">Volleyball</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Serve streak game</li>
                    <li><u>Goal:</u> Perform longest serve streak in 60 seconds</li>
                    <li><u>Scoring:</u> Length of streak</li>
                    <li><u>Controls:</u> Virtual paddle using iPad AR movement</li>
                    <li><u>Aids:</u> Guide arrow to net</li>
                </ul>
            </div> <!--- End List --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vfbH_volleyball_example.png">
            </div> <!--- End Pic --->
        </div> <!--- End Table Cell --->
        <!--- End Volleyball --->
        <!--- End VFB-H Minigame Table --->
    </details>
    <p>In addition to designing and implementing these minigames, I was also responsible for the following:</p>
    <ul>
        <li>Lead designer and software engineer</li>
        <li>Designing and implementing:</li>
        <ul>
            <li>New park layout to allow for exploration</li>
            <li>Virtual kiosks to start/stop games, display instructions, and show leaderboards</li>
            <li>Speech to text (STT) for VFB tricks using Google's STT API</li>
            <li>Arrow navigation system to show players where to go for their next objective</li>
            <li>Trophy system that dynamically changed size as players met higher and higher physical activity goals</li>
            <li>New iPad-based input system (touchscreen, AR motion, and voice)</li>
        </ul>
        <li>Adding sound effects to the park, including ball bouncing sounds, cheers, and dings</li> 
        <li>These sound effects were used to add some more realism to the app</li>
        <li>Additionally, they were used to provide feedback that the player was completing tasks correctly</li>
        <li>Recording and editing a video to show how to use the VFB-H app (for the pilot, include?)</li>
        <li>Setting up the iPads to auto-update when we issued updates to the app</li>
        <li>Bug troubleshooting and fixes for both VFB app and Fitbit syncing</li>
        <li>Tech support and troubleshooting iPads and physical activity trackers</li>
        <li>Data analysis on game play metrics</li>
    </ul>
</details>

## Virtual Fitness Buddy Afterschool

<details open>
    <summary>VFB-A Info TODO: keep title?</summary>
    <figure class=img-fig>
        <img class=scale-w100 src="vfbA_kioskComparison.png">
        <figcaption>  Kiosks used during the VFB-A pilot (left) and C1-A and C2-A (right). The C1-A/C2-A kiosk added a touchscreen display for menu selection.</figcaption>
    </figure>
    <p>The Virtual Fitness Buddy Afterschool (VFB-A) project was designed to encourage children to engage in healthier physical activity (PA) habits through the use of a virtual dog buddy. As a child completed PA, tracked using a Fitbit PA tracker, their VFB's health would increase, which meant that they could play for longer, unlock new games and tricks, and earn points to spend on various customizations. VFB-A was built as a kiosk station to be used in afterschool programs consisting of a large screen display, touchscreen, and Microsoft Kinect.</p>
    <details open>
        <summary>VFB-A Stats</summary>
        <div class="table-container">
            <table>
                <tbody>
                    <tr>
                        <td>Name</td>
                        <td>Virtual Fitness Buddy Afterschool (VFB-A)</td>
                    </tr>
                    <tr>
                        <td>Dates</td>
                        <td>Spring 2018 to Fall 2019</td>
                    </tr>
                    <tr>
                        <td>Location</td>
                        <td>Afterschool Programs</td>
                    </tr>
                    <tr>
                        <td>Sites</td>
                        <td>11 Treatment (21 Total)</td>
                    </tr>
                    <tr>
                        <td>Cohorts</td>
                        <td>3</td>
                    </tr>
                    <tr>
                        <td>Duration</td>
                        <td>6 months each</td>
                    </tr>
                    <tr>
                        <td>Participants</td>
                        <td>318 Treatment (464 Total)</td>
                    </tr>
                    <tr>
                        <td>Focus</td>
                        <td>Physical Activity</td>
                    </tr>
                    <tr>
                        <td>Controls</td>
                        <td>Motion, Touch, and Voice </td>
                    </tr>
                </tbody>
            </table>
        </div>
    </details>
    <figure class=img-fig>
        <img class=scale-w75 src="VFB-A-H and VFB-C Comparison - Motion Blur.png">
        <figcaption>The evolution of the VFB model from older systems (left) to the VFB-A system (right) with the UGA Arch in the background.</figcaption>
    </figure>
    <p>As part of this app, I designed six different minigames: agility, bark it, basketball, frisbee, soccer, and volleyball. See below for more details on these games. In addition to these games, children were able to get their VFB to perform tricks using their voice and could play fetch without having to interact with a minigame. To achieve this, I implemented various midair gesture-based systems that players would use to perform the necessary actions for the minigames, tricks, and fetch.</p>
    <details open>
        <summary>VFB-A Minigames</summary>
        <!--- Basketball --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vfbA_basketball.png">
            </div> <!--- End Pic --->
            <div class="mgTable-list"> <!--- List --->
                <p class="mgTable-title">Basketball</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Goal scoring game</li>
                    <li><u>Goal:</u> Maximize basketballs scored in 60 seconds</li>
                    <li><u>Scoring:</u> Goals scored</li>
                    <li><u>Controls:</u> Shot zone system and Kinect movement</li>
                </ul>
            </div> <!--- End List --->
        </div> <!--- End Table Cell --->
        <!--- End Basketball --->
        <!--- Slingshot --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-listLeft"> <!--- List --->
                <p class="mgTable-title">Slingshot</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Balloon popping game</li>
                    <li><u>Goal:</u> Maximize balloons popped in 60 seconds</li>
                    <li><u>Scoring:</u> Sum of balloon values</li>
                    <li><u>Controls:</u> Kinect grabbing gesture and movement</li>
                </ul>
            </div> <!--- End List --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vfbA_slingshot.png">
            </div> <!--- End Pic --->
        </div> <!--- End Table Cell --->
        <!--- End Slingshot --->
        <!--- Soccer --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vfbA_soccer.png">
            </div> <!--- End Pic --->
            <div class="mgTable-list"> <!--- List --->
                <p class="mgTable-title">Soccer</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Goal scoring game</li>
                    <li><u>Goal:</u> Maximize soccer balls scored in 60 seconds </li>
                    <li><u>Scoring:</u> Goals scored</li>
                    <li><u>Controls:</u> Virtual paddle attached to foot for kicking</li>
                </ul>
            </div> <!--- End List --->
        </div> <!--- End Table Cell --->
        <!--- End Soccer --->
        <!--- Volleyball --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-listLeft"> <!--- List --->
                <p class="mgTable-title">Volleyball</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Serve streak game</li>
                    <li><u>Goal:</u> Perform longest serve streak in 60 seconds</li>
                    <li><u>Scoring:</u> Length of streak</li>
                    <li><u>Controls:</u> Virtual paddle attached to hand to return serve</li>
                </ul>
            </div> <!--- End List --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vfbA_volleyball.png">
            </div> <!--- End Pic --->
        </div> <!--- End Table Cell --->
        <!--- End Volleyball --->
    </details>
    <p>In addition to designing and implementing these minigames, I was also responsible for the following:</p>
    <ul>
        <li>Lead designer and software engineer</li>
        <li>Lead a small team of artists and programmers</li>
        <li>Designed and implemented:</li>
        <ul>
            <li>Avatar</li>
            <li>Touchscreen selection system</li>
            <li>Two different throwing and trick gesture systems</li>
            <li>Leaderboards</li>
            <li>Data logging and data structures</li>
        </ul>
        <li>Setting up and maintaining both control and treatment kiosks</li>
        <li>Tech support and troubleshooting for both kiosks and physical activity trackers</li>
        <li>Data engineer</li>
        <ul>
            <li>Creating notes on what each data point meant</li>
            <li>Converting this data into a format our statisticians could use to process the data easily</li>
        </ul>
        <li>TODO: my responsibilities list</li>
    </ul>
</details>

## Virtual STEM Buddy at Museum

<details open>
    <summary>VSB-M Info TODO: keep title?</summary>
    <figure class=img-fig>
        <img class=scale-w100 src="vsb_kiosk.png">
        <figcaption>The VSB Kiosk at the Children’s Museum of Atlanta.</figcaption>
    </figure>
    <p>The Virtual STEM Buddy Museum (VSB-M) project was designed to encourage children to learn more about various STEM concepts through the use of a virtual robot buddy. As a child played the minigames, their VSB would provide instructions on how to play in addition to information on the underlying STEM concept being used, such as levers and trajectories. This info was conveyed both through text and audio as it could not be assumed that all of its players would be able to read. VSB-M was built as an exhibit at the Children's Museum of Atlanta (CMOA) consisting of a large screen display, Android tablet, and Microsoft Kinect.</p>
    <details open>
        <summary>VSB-M Stats</summary>
        <div class="table-container">
            <table>
                <tbody>
                    <tr>
                        <td>Name</td>
                        <td>Virtual STEM Buddy Museum (VSB-M)</td>
                    </tr>
                    <tr>
                        <td>Dates</td>
                        <td>January 2017 to May 2022</td>
                    </tr>
                    <tr>
                        <td>Location</td>
                        <td>Children's Museum of Atlanta (CMOA)</td>
                    </tr>
                    <tr>
                        <td>Sites</td>
                        <td>1</td>
                    </tr>
                    <tr>
                        <td>Cohorts</td>
                        <td>1</td>
                    </tr>
                    <tr>
                        <td>Duration</td>
                        <td>5 years</td>
                    </tr>
                    <tr>
                        <td>Participants</td>
                        <td>Unknown – 28,122 recorded plays over 2 years</td>
                    </tr>
                    <tr>
                        <td>Focus</td>
                        <td>STEM Education</td>
                    </tr>
                    <tr>
                        <td>Controls</td>
                        <td>Motion and Touch</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </details>
    <p>TODO: talk about how buddy was customizable, kinect which meant they used their bodies to interact, maybe talk about gestures and adding the touchscreen because familiar interface?</p>
    <p>The tablet provided a familiar museum exhibit interface that was used for complex selection tasks, such as customizing their VSB. While the Kinect provided a more novel interface where players used their real world movements to interact with their VSB and play the minigames.</p>
    <figure class=img-fig>
        <img class=scale-h75 src="vsb_buddies_combo.png">
        <figcaption>The VSB customization interface (left) along with six customized VSBs showing the various color and shape options (right).</figcaption>
    </figure>
    <p>As part of this app, I designed two different minigames: Lever Hero and Slingshot. They were designed to target the concepts of lever balancing and trajectories respectively. See below for more details on these games.</p>
    <details open>
        <summary>VSB-M Minigames</summary>
        <!--- Lever Hero --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vsb_leverHero.png">
            </div> <!--- End Pic --->
            <div class="mgTable-list"> <!--- List --->
                <p class="mgTable-title">Lever Hero</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Lever balancing game</li>
                    <li><u>STEM Concept: </u>Levers</li>
                    <li><u>Goal:</u> Balance levers as quickly and accurately as possible </li>
                    <li><u>Controls:</u> Kinect grabbing gesture and movement</li>
                </ul>
            </div> <!--- End List --->
        </div> <!--- End Table Cell --->
        <!--- End Lever Hero --->
        <!--- Slingshot --->
        <div class="mgTable"> <!--- Table Cell --->
            <div class="mgTable-listLeft"> <!--- List --->
                <p class="mgTable-title">Slingshot</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Trajectory game</li>
                    <li><u>STEM Concept:</u> Trajectories</li>
                    <li><u>Goal:</u> Complete picture with minimal paint splats</li>
                    <li><u>Controls:</u> Kinect grabbing gesture and movement</li>
                </ul>
            </div> <!--- End List --->
            <div class="mgTable-pic"> <!--- Pic --->
                <img src="vsb_slingshot.png">
            </div> <!--- End Pic --->
        </div> <!--- End Table Cell --->
        <!--- End Slingshot --->
    </details>
    <p>In addition to designing and implementing these minigames, I was also responsible for the following:</p>
    <ul>
        <li>Lead designer and software engineer</li><!-- TODO: instructions and text to voice, game play logic and loop-->
        <li>Designing and implementing:</li>
        <ul>
            <li>VSB interactivity</li>
            <li>Data logging system and its data structures</li>
            <li>New player avatar system</li>
        </ul>
        <li>Worked with CMOA staff to:</li>
        <ul>
            <li>Scale the interactions to the exhibit's allocated physical space</li>
            <li>Design game mechanics that would fit well and safely into the museum environment</li>
        </ul>
        <li>Observing and recording interactions in person in order to update the system to address any issues that arose</li>
        <li>Data analysis on game play metrics</li>
        <li>Tech support and troubleshooting the kiosk</li>
    </ul>
    <p>TODO: my responsibilities list</p>
</details>

<!--- TODO: ## Virtual Fitness Buddy Summer Camp

    <details open>
        <summary>VFB-C Info TODO: keep title?</summary>
        <p>TODO: I was responsible for the following:</p>
        <ul>
            <li>Designing and implementing</li>
            <ul>
                <li>Updated user interface (UI)</li>
                <li>Hover selection technique for menu selection</li>
                <li>Trick shop</li>
                <li>Trick and Fitbit selection systems</li>
            </ul>
            <li>Observing and troubleshooting VFB-C system throughout the study</li>
            <li>Fitbit setup and troubleshooting</li>
            <li>Administering post-treatment questionnaires</li>
        </ul>
    </details>
--->
<!--- TODO: ## Virtual Buddy Fruit and Vegetable Summer Camp

    <details open>
        <summary>VB-F&V Info TODO: keep title?</summary>
        <p>TODO: I was responsible for the following:</p>
        <ul>
            <li>Designing and implementing:</li>
            <ul>
                <li>Haptic joystick input system</li>
                <li>Reward system based on fruit and vegetable consumption</li>
                <li>RFID login system</li>
                <li>Heart and artery testing minigames</li>
                <li>Updating gesture system to use the haptic joystick</li>
            </ul>
            <li>Observing and troubleshooting VB-F&V system throughout the study</li>
            <li>Administering post-treatment questionnaires</li>
        </ul>
    </details>
--->
