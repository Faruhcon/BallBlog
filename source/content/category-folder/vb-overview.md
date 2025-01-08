---
title: Virtual Buddy Projects Overview
#draft: true
---

# TODO: Page Header

TODO: intro blurb

This page contains info on the virtual buddy applications that I built through the course of my PhD work, which includes two major versions of the Virtual Fitness Buddy system and the Virtual STEM Buddy system, which encouraged children to engage in healthier exercise habits and to learn about various STEM concepts respectively. These systems took a <!-- TODO: more specific info on these projects can be found on their individual pages (links). -->

TODO: find the vfb video I made?? should be on youtube
## Virtual Fitness Buddy at Home

<details open> <!-- VFB-H -->
    <summary>VFB-H Info TODO: keep title?</summary>
    <figure class=img-fig>
        <img class=scale-w100 
            src="vfbH_interface-example2.png"
            alt="A game with dog and stage on iPad."
            title="VFB-H iPad interface">
        <figcaption>The VFB-H iPad interface.</figcaption>
    </figure>
    <p>The Virtual Fitness Buddy Home (VFB-H) project was designed to encourage children to engage in healthier physical activity (PA) habits through the use of a virtual dog buddy. As a child completed PA, tracked using a Fitbit PA tracker, their VFB's health would increase, which meant that they could play for longer, unlock new games and tricks, and earn points to spend on various customizations. VFB-H was built as an iPad app that children could use at home, utilizing touchscreen, voice-activation, and real-life motion as ways to interact with the system.</p>
    <details open> <!-- VFB-H Stats -->
        <summary>VFB-H Stats</summary>
        <div class="table-container"> <!-- VFB-H Stats Table -->
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
                    <tr>
                        <td>Hardware</td>
                        <td>iPad</td>
                    </tr>
                    <tr>
                        <td>Publication</td>
                        <td><a href="https://www.proquest.com/dissertations-theses/design-field-implementation-virtual-buddy-based/docview/2917424271/se-2?accountid=14537">Dissertation Ch. 5</a></td>
                    </tr>
                </tbody>
            </table>
        </div> <!-- End VFB-H Stats Table -->
    </details> <!-- End VFB-H Stats -->
    <!-- <figure class=img-fig>
        <img class=scale-w100 src="vfbA_petCustomizations_example.png">
        <figcaption>VFB coat, tag, collar, and hat customizations.</figcaption>
    </figure>
    <figure class=img-fig>
        <img class=scale-w100 src="vfbA_petToys_example.png">
        <figcaption>Toy options and customizations.</figcaption>
    </figure> -->
    <figure class=img-fig>
        <img class=scale-w100 
            src="vfbA_petCustomizations-and-toys.png"
            alt="Eight customized virtual dogs and ten fetch toys on a bench."
            title="VFB-H customization options">
        <figcaption>VFB coat, tag, collar, hat, and toy customizations.</figcaption>
    </figure>
    <p>As part of this app, I designed six different minigames: agility, bark it, basketball, frisbee, soccer, and volleyball. See below for more details on these games. I implemented leaderboards that would track their top 3 personal scores in addition to the top 3 scores for their family and across the entire study for each minigame. In addition to these games, children were able to get their VFB to perform tricks using their voice and could play fetch without having to interact with a minigame.</p>
    <details open> <!-- VFB-H Minigame Table -->
        <summary>VFB-H Minigames</summary>
        <!-- Agility -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vfbH_agility_example.png"
                    alt="A virtual dog jumping over a hurdle."
                    title="VFB-H Agility Minigame">
            </div> <!-- End Pic -->
            <div class="mgTable-list"> <!-- List -->
                <p class="mgTable-title">Agility</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Obstacle course</li>
                    <li><u>Goal:</u> Guide VFB through obstacles as quickly as possible</li>
                    <li><u>Scoring:</u> Time remaining on 60 second timer</li>
                    <li><u>Controls:</u> Virtual joystick (touchscreen)</li>
                    <li><u>Aids:</u> Guide arrow to next obstacle</li>
                </ul>
            </div> <!-- End List -->
        </div> <!-- End Table Cell -->
        <!-- End Agility -->
        <!-- Bark It -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-listLeft"> <!-- List -->
                <p class="mgTable-title">Bark It</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Trick memory game</li>
                    <li><u>Goal:</u> Complete longest trick streak</li>
                    <li><u>Scoring:</u> Number of correct tricks performed</li>
                    <li><u>Controls:</u> Voice or touchscreen</li>
                    <li><u>Aids:</u> Guide arrow to stage</li>
                </ul>
            </div> <!-- End List -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vfbH_barkIt2_example.png"
                    alt="A virtual dog chasing its tail on a stage."
                    title="VFB-H Bark It Minigame">
            </div> <!-- End Pic -->
        </div> <!-- End Table Cell -->
        <!-- End Bark It -->
        <!-- Basketball -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vfbH_basketball_example2.png"
                    alt="A virtual dog standing on a basketball court with a scoreboard."
                    title="VFB-H Basketball Minigame">
            </div> <!-- End Pic -->
            <div class="mgTable-list"> <!-- List -->
                <p class="mgTable-title">Basketball</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Goal throws from random locations game</li>
                    <li><u>Goal:</u> Maximize basketballs scored in 60 seconds</li>
                    <li><u>Scoring:</u> Goals scored</li>
                    <li><u>Controls:</u> Virtual joystick and buttons (touchscreen) and iPad AR movement</li>
                    <li><u>Aids:</u> Guide arrow to next location and hoop</li>
                </ul>
            </div> <!-- End List -->
        </div> <!-- End Table Cell -->
        <!-- End Basketball -->
        <!-- Frisbee -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-listLeft"> <!-- List -->
                <p class="mgTable-title">Frisbee</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Balloon popping game</li>
                    <li><u>Goal:</u> Maximize balloons popped in 60 seconds</li>
                    <li><u>Scoring:</u> Sum of balloon values plus VFB catch bonuses</li>
                    <li><u>Controls:</u> Virtual buttons (touchscreen) and iPad AR movement</li>
                    <li><u>Aids:</u> Guide arrow to current balloon</li>
                </ul>
            </div> <!-- End List -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vfbH_frisbee_example.png"
                    alt="A virtual dog excited to chase a frisbee."
                    title="VFB-H Frisbee Minigame">
            </div> <!-- End Pic -->
        </div> <!-- End Table Cell -->
        <!-- End Frisbee -->
        <!-- Soccer -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vfbH_soccer_example.png"
                    alt="A virtual dog holding a soccer ball on a soccer field with a scoreboard."
                    title="VFB-H Soccer Minigame">
            </div> <!-- End Pic -->
            <div class="mgTable-list"> <!-- List -->
                <p class="mgTable-title">Soccer</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Goal kicks from random locations game</li>
                    <li><u>Goal:</u> Maximize soccer balls scored in 60 seconds </li>
                    <li><u>Scoring:</u> Goals scored</li>
                    <li><u>Controls:</u> Virtual joystick and buttons (touchscreen) and virtual paddle using iPad AR movement</li>
                    <li><u>Aids:</u> Guide arrow to next location and goal</li>
                </ul>
            </div> <!-- End List -->
        </div> <!-- End Table Cell -->
        <!-- End Soccer -->
        <!-- Volleyball -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-listLeft"> <!-- List -->
                <p class="mgTable-title">Volleyball</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Serve streak game</li>
                    <li><u>Goal:</u> Perform longest serve streak in 60 seconds</li>
                    <li><u>Scoring:</u> Length of streak</li>
                    <li><u>Controls:</u> Virtual paddle using iPad AR movement</li>
                    <li><u>Aids:</u> Guide arrow to net</li>
                </ul>
            </div> <!-- End List -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vfbH_volleyball_example.png"
                    alt="A virtual dog serving a beach ball over a volleyball net."
                    title="VFB-H Volleyball Minigame">
            </div> <!-- End Pic -->
        </div> <!-- End Table Cell -->
        <!-- End Volleyball -->
    </details> <!-- End VFB-H Minigame Table -->
    <p>In addition to designing and implementing these minigames, I was also responsible for the following:</p>
    <ul> <!-- VFB-H responsibilities list -->
        <li>Lead designer and software engineer</li>
        <li>Designing and implementing:</li>
        <ul> <!-- VFB-H design and implement list -->
            <li>New park layout to allow for exploration</li>
            <li>Virtual kiosks to start/stop games, display instructions, and show leaderboards</li>
            <li>Speech to text (STT) for VFB tricks using Google's STT API</li>
            <li>Arrow navigation system to show players where to go for their next objective</li>
            <li>Trophy system that dynamically changed size as players met higher and higher physical activity goals</li>
            <li>New iPad-based input system (touchscreen, AR motion, and voice)</li>
        </ul> <!-- End VFB-H design and implement list -->
        <li>Adding sound effects to the park, including ball bouncing sounds, cheers, and dings</li> 
        <li>These sound effects were used to add some more realism to the app</li>
        <li>Additionally, they were used to provide feedback that the player was completing tasks correctly</li>
        <li>Recording and editing a video to show how to use the VFB-H app (for the pilot, include?)</li>
        <li>Setting up the iPads to auto-update when we issued updates to the app</li>
        <li>Bug troubleshooting and fixes for both VFB app and Fitbit syncing</li>
        <li>Tech support and troubleshooting iPads and physical activity trackers</li>
        <li>Data analysis on game play metrics</li>
    </ul> <!-- End VFB-H responsibilities list -->
</details> <!-- End VFB-H -->

## Virtual STEM Buddy at Museum

<details open> <!-- VSB-M -->
    <summary>VSB-M Info TODO: keep title?</summary>
    <figure class=img-fig>
        <img class=scale-w100 
            src="vsb_kiosk.png"
            alt="Large screen television with a tablet displaying a game."
            title="Virtual STEM Buddy Kiosk">
        <figcaption>The VSB Kiosk at the Children’s Museum of Atlanta.</figcaption>
    </figure>
    <p>The Virtual STEM Buddy Museum (VSB-M) project was designed to encourage children to learn more about various STEM concepts through the use of a virtual robot buddy. As a child played the minigames, their VSB would provide instructions on how to play in addition to information on the underlying STEM concept being used, such as levers and trajectories. This info was conveyed both through text and audio as it could not be assumed that all of its players would be able to read. VSB-M was built as an exhibit at the Children's Museum of Atlanta (CMOA) consisting of a large screen display, Android tablet, and Microsoft Kinect.</p>
    <details open> <!-- VSB-M Stats -->
        <summary>VSB-M Stats</summary>
        <div class="table-container"> <!-- VSB-M Stats table -->
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
                    <tr>
                        <td>Hardware</td>
                        <td>TV, PC, Kinect, Android Tablet</td>
                    </tr>
                    <tr>
                        <td>Publications</td>
                        <td>
                            <a href="https://wevr.adalsimeone.me/2019/WEVR2019_Ball.pdf">Paper</a>
                            <a href ="https://www.proquest.com/dissertations-theses/design-field-implementation-virtual-buddy-based/docview/2917424271/se-2?accountid=14537">Dissertation Ch. 3</a>
                        </td>
                    </tr>
                </tbody>
            </table>
        </div> <!-- End VSB-M Stats Table -->
    </details> <!-- End VSB-M Stats -->
    <p>TODO: maybe talk about gestures and adding the touchscreen because familiar interface?</p>
    <p>The tablet provided a familiar museum exhibit interface that was used for complex selection tasks, such as customizing their VSB. While the Kinect provided a more novel interface where players used their real world movements to interact with their VSB and play the minigames.</p>
    <figure class=img-fig>
        <img class=scale-h75 
            src="vsb_buddies_combo.png"
            alt="Ten customized robots with various colors and shapes."
            title="Various VSB Buddy Examples">
        <figcaption>The VSB customization interface (left) along with six customized VSBs showing the various color and shape options (right).</figcaption>
    </figure>
    <p>As part of this app, I designed two different minigames: Lever Hero and Slingshot. They were designed to target the concepts of lever balancing and trajectories respectively. See below for more details on these games.</p>
    <details open> <!-- VSB-M Minigame Table -->
        <summary>VSB-M Minigames</summary>
        <!-- Lever Hero -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vsb_leverHero.png"
                    alt="A virtual person holding a cube over a lever with a robot buddy."
                    title="VSB-M Lever Hero Minigame">
            </div> <!-- End Pic -->
            <div class="mgTable-list"> <!-- List -->
                <p class="mgTable-title">Lever Hero</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Lever balancing game</li>
                    <li><u>STEM Concept: </u>Levers</li>
                    <li><u>Goal:</u> Balance levers as quickly and accurately as possible </li>
                    <li><u>Scoring:</u> Remaining time to solve problems</li>
                    <li><u>Controls:</u> Kinect grabbing gesture and movement</li>
                </ul>
            </div> <!-- End List -->
        </div> <!-- End Table Cell -->
        <!-- End Lever Hero -->
        <!-- Slingshot -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-listLeft"> <!-- List -->
                <p class="mgTable-title">Slingshot</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Trajectory game</li>
                    <li><u>STEM Concept:</u> Trajectories</li>
                    <li><u>Goal:</u> Complete picture with minimal paint splats</li>
                    <li><u>Scoring:</u> Remaining time to solve problems</li>
                    <li><u>Controls:</u> Kinect grabbing gesture and movement</li>
                </ul>
            </div> <!-- End List -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vsb_slingshot.png"
                    alt="A virtual person releasing a slingshot pouch with a robot buddy."
                    title="VSB-M Slingshot Minigame">
            </div> <!-- End Pic -->
        </div> <!-- End Table Cell -->
        <!-- End Slingshot -->
    </details> <!-- End VSB-M Minigame Table -->
    <p>In addition to designing and implementing these minigames, I was also responsible for the following:</p>
    <ul> <!-- VSB-M responsibilities list -->
        <li>Lead designer and software engineer</li><!-- TODO: instructions and text to voice, game play logic and loop-->
        <li>Designing and implementing:</li>
        <ul> <!-- VSB-M design and implement list -->
            <li>VSB interactivity</li>
            <li>Data logging system and its data structures</li>
            <li>New player avatar system</li>
        </ul> <!-- End VSB-M design and implement list -->
        <li>Worked with CMOA staff to:</li>
        <ul>
            <li>Scale the interactions to the exhibit's allocated physical space</li>
            <li>Design game mechanics that would fit well and safely into the museum environment</li>
        </ul>
        <li>Observing and recording interactions in person in order to update the system to address any issues that arose</li>
        <li>Data analysis on game play metrics</li>
        <li>Tech support and troubleshooting the kiosk</li>
    </ul> <!-- End VSB-M responsibilities list -->
    <p>TODO: my responsibilities list</p>
</details> <!-- End VSB-M -->

## Virtual Fitness Buddy Afterschool

<details open> <!-- VFB-A -->
    <summary>VFB-A Info TODO: keep title?</summary>
    <figure class=img-fig>
        <img class=scale-w100 
            src="vfbA_kioskComparison.png"
            alt="Two mobile, locking cabinets with large screen televisions on top."
            title="Virtual Fitness Buddy Afterschool Kiosks">
        <figcaption>  Kiosks used during the VFB-A pilot (left) and C1-A and C2-A (right). The C1-A/C2-A kiosk added a touchscreen display for menu selection.</figcaption>
    </figure>
    <p>The Virtual Fitness Buddy Afterschool (VFB-A) project was designed to encourage children to engage in healthier physical activity (PA) habits through the use of a virtual dog buddy. As a child completed PA, tracked using a Fitbit PA tracker, their VFB's health would increase, which meant that they could play for longer, unlock new games and tricks, and earn points to spend on various customizations. VFB-A was built as a mobile kiosk station to be used in afterschool programs consisting of a large screen display, touchscreen, and Microsoft Kinect.</p>
    <details open> <!-- VFB-A Stats -->
        <summary>VFB-A Stats</summary>
        <div class="table-container"> <!-- VFB-A Stats Table -->
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
                    <tr>
                        <td>Hardware</td>
                        <td>TV, PC, Kinect, Touchscreen</td>
                    </tr>
                    <tr>
                        <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9016571/">Paper</a>
                        <a href="https://www.proquest.com/dissertations-theses/design-field-implementation-virtual-buddy-based/docview/2917424271/se-2?accountid=14537">Dissertation Ch. 4</a>
                    </tr>
                </tbody>
            </table>
        </div> <!-- End VFB-A Stats Table -->
    </details> <!-- End VFB-A Stats -->
    <figure class=img-fig>
        <img class=scale-w75 
            src="VFB-A-H and VFB-C Comparison - Motion Blur.png"
            alt="A comparison of two versions a virtual dog."
            title="VFB-A and VFB-C Buddy Comparison">
        <figcaption>The evolution of the VFB model from older systems (left) to the VFB-A system (right) with the UGA Arch in the background.</figcaption>
    </figure>
    <p>As part of this app, I designed six different minigames: agility, bark it, basketball, frisbee, soccer, and volleyball. See below for more details on these games. In addition to these games, children were able to get their VFB to perform tricks using their voice and could play fetch without having to interact with a minigame. To achieve this, I implemented various midair gesture-based systems that players would use to perform the necessary actions for the minigames, tricks, and fetch.</p>
    <details open> <!-- VFB-A Minigame Table -->
        <summary>VFB-A Minigames</summary>
        <!-- Basketball -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vfbA_basketball.png"
                    alt="A virtual person throwing a basketball with a dog."
                    title="VFB-A Basketball Minigame">
            </div> <!-- End Pic -->
            <div class="mgTable-list"> <!-- List -->
                <p class="mgTable-title">Basketball</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Goal scoring game</li>
                    <li><u>Goal:</u> Maximize basketballs scored in 60 seconds</li>
                    <li><u>Scoring:</u> Goals scored</li>
                    <li><u>Controls:</u> Shot zone system and Kinect movement</li>
                </ul>
            </div> <!-- End List -->
        </div> <!-- End Table Cell -->
        <!-- End Basketball -->
        <!-- Slingshot -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-listLeft"> <!-- List -->
                <p class="mgTable-title">Slingshot</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Balloon popping game</li>
                    <li><u>Goal:</u> Maximize balloons popped in 60 seconds</li>
                    <li><u>Scoring:</u> Sum of balloon values</li>
                    <li><u>Controls:</u> Kinect grabbing gesture and movement</li>
                </ul>
            </div> <!-- End List -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vfbA_slingshot.png"
                    alt="A virtual person holding a slingshot pouch with a dog and balloons."
                    title="VFB-A Slingshot Minigame">
            </div> <!-- End Pic -->
        </div> <!-- End Table Cell -->
        <!-- End Slingshot -->
        <!-- Soccer -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vfbA_soccer.png"
                    alt="A virtual person kicking a soccerball towards the goal with a dog."
                    title="VFB-A Soccer Minigame">
            </div> <!-- End Pic -->
            <div class="mgTable-list"> <!-- List -->
                <p class="mgTable-title">Soccer</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Goal scoring game</li>
                    <li><u>Goal:</u> Maximize soccer balls scored in 60 seconds </li>
                    <li><u>Scoring:</u> Goals scored</li>
                    <li><u>Controls:</u> Virtual paddle attached to foot for kicking</li>
                </ul>
            </div> <!-- End List -->
        </div> <!-- End Table Cell -->
        <!-- End Soccer -->
        <!-- Volleyball -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-listLeft"> <!-- List -->
                <p class="mgTable-title">Volleyball</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Serve streak game</li>
                    <li><u>Goal:</u> Perform longest serve streak in 60 seconds</li>
                    <li><u>Scoring:</u> Length of streak</li>
                    <li><u>Controls:</u> Virtual paddle attached to hand to return serve</li>
                </ul>
            </div> <!-- End List -->
            <div class="mgTable-pic"> <!-- Pic -->
                <img src="vfbA_volleyball.png"
                    alt="A virtual person hitting a beach ball over a volleyball net with dog."
                    title="VFB-A Volleyball Minigame">
            </div> <!-- End Pic -->
        </div> <!-- End Table Cell -->
        <!-- End Volleyball -->
    </details> <!-- End VFB-A Minigame Table -->
    <p>In addition to designing and implementing these minigames, I was also responsible for the following:</p>
    <ul> <!-- VFB-A responsibilities list -->
        <li>Lead designer and software engineer</li>
        <li>Lead a small team of artists and programmers</li>
        <li>Designed and implemented:</li>
        <ul> <!-- VFB-A design and implement list -->
            <li>Avatar</li>
            <li>Touchscreen selection system</li>
            <li>Two different throwing and trick gesture systems</li>
            <li>Leaderboards</li>
            <li>Data logging and data structures</li>
        </ul> <!-- End VFB-A design and implement list -->
        <li>Setting up and maintaining both control and treatment kiosks</li>
        <li>Tech support and troubleshooting for both kiosks and physical activity trackers</li>
        <li>Data engineer</li>
        <ul> <!-- Data Engineer list -->
            <li>Creating notes on what each data point meant</li>
            <li>Converting this data into a format our statisticians could use to process the data easily</li>
        </ul> <!-- End Data Engineer list -->
        <li>TODO: my responsibilities list</li>
    </ul> <!-- End VFB-A responsibilities list -->
</details> <!-- End VFB-A -->

## Virtual Fitness Buddy Summer Camp

<details open> <!-- VFB-C -->
    <summary>VFB-C Info TODO: keep title?</summary>
    <p><!-- TODO: done? -->The Virtual Fitness Buddy Summer Camp (VFB-C) project was designed to encourage children to engage in healthier physical activity (PA) habits through the use of a virtual dog buddy. As a child completed PA goals, tracked using a Fitbit PA tracker, they would earn points to use to unlock new tricks and their VFB's health would increase, meaning that they were slimmer and faster. Unlike the other VFB projects, children could only interact with their VFB by playing fetch and completing tricks without any minigames. VFB-C was built as a mobile kiosk station to be used in a week-long summer camp consisting of a large screen display and Microsoft Kinect. Lastly, the control group for this study also had their own VFB, but they did not earn points to spend.</p>
    <figure class=img-fig> <!-- TODO: right size? -->
        <img class=scale-w100 
            src="vfbC_kiosk-pet-skele.png"
            alt="Compilation of TV, virtual dog, and spheres in the shape of a human."
            title="VFB-C kiosk, buddy, and Kinect skeleton">
        <figcaption>The VFB-C kiosk, buddy, and Kinect skeleton.</figcaption>
    </figure>
    <details open> <!-- VFB-C Stats -->
        <summary>VFB-C Stats</summary>
        <div class="table-container"> <!-- VFB-C Stats Table -->
            <table>
                <tbody>
                    <tr>
                        <td>Name</td>
                        <td>Virtual Fitness Buddy Camp (VFB-C)</td>
                    </tr>
                    <tr>
                        <td>Dates</td>
                        <td>Summer 2015</td>
                    </tr>
                    <tr>
                        <td>Location</td>
                        <td>Summer Camp</td>
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
                        <td>3 Days</td>
                    </tr>
                    <tr>
                        <td>Participants</td>
                        <td>39 Treatment (67 Total)</td>
                    </tr>
                    <tr>
                        <td>Focus</td>
                        <td>Physical Activity</td>
                    </tr>
                    <tr>
                        <td>Controls</td>
                        <td>Motion and Voice </td>
                    </tr>
                    <tr>
                        <td>Hardware</td>
                        <td>TV, PC, Kinect</td>
                    </tr>
                    <tr>
                        <td>Publications</td>
                        <td>
                            <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC6566098/">Paper</a>
                            <a href="https://www.proquest.com/dissertations-theses/design-field-implementation-virtual-buddy-based/docview/2917424271/se-2?accountid=14537">Dissertation Ch. 2.2</a>
                        </td>
                    </tr>
                </tbody>
            </table>
        </div> <!-- End VFB-C Stats Table -->
    </details> <!-- End VFB-C Stats -->
    <p>TODO: second blurb - what about?? there's no minigames</p>
    <p>TODO: pic?</p>
    <p>TODO: I was responsible for the following:</p>
    <ul> <!-- VFB-C Responsibilities List -->
        <li>Designing and implementing</li>
        <ul> <!-- VFB-C design and implement list -->
            <li>Updated user interface (UI)</li>
            <li>Hover selection technique for menu selection</li>
            <li>Trick shop</li>
            <li>Trick and Fitbit selection systems</li>
        </ul> <!-- End VFB-C design and implement list -->
        <li>Observing and troubleshooting VFB-C system throughout the study</li>
        <li>Fitbit setup and troubleshooting</li>
        <li>Administering post-treatment questionnaires</li>
    </ul> <!-- End VFB-C responsibilities list -->
</details> <!-- End VFB-C -->

TODO: 
## Virtual Buddy Fruit and Vegetable Summer Camp

<details open> <!-- VB-F&V -->
    <summary>VB-F&V Info TODO: keep title?</summary>
    <p>The Virtual Buddy Fruit and Vegetable (VB-F&V) project was designed to encourage children to engage in healthier fruit and vegetable (F&V) habits through the use of a virtual dog buddy. As a child ate more fruits and vegetables, tracked by camp counselors, their VB's health would increase, which meant that their heart would be easier to pump, their major artery would be more elastic, and they could complete fetching and tricks faster. As that child met their F&V goals, they would earn credits to spend on performing tricks. VB-F&V was built as a station to be used in a week-long summer camp consisting of a Mac and Novint Falcon (haptic joystick).</p>
    <figure class=img-fig> <!-- TODO: right size? -->
        <img class=scale-w75 
            src="vbFV_interface_modified4.png"
            alt="Virtual dog on a screen with a haptic joystick controller."
            title="Virtual Buddy Fruit and Vegetable (VB-F&V) Station">
        <figcaption>The VB-F&V Novint Falcon station.</figcaption>
    </figure>
    <details open> <!-- VB-F&V Stats -->
        <summary>VB-F&V Stats</summary>
        <div class="table-container"> <!-- VB-F&V Stats Table -->
            <table>
                <tbody>
                    <tr>
                        <td>Name</td>
                        <td>Virtual Buddy Fruit and Vegetable (VB-F&V)</td>
                    </tr>
                    <tr>
                        <td>Dates</td>
                        <td>Summer 2014</td>
                    </tr>
                    <tr>
                        <td>Location</td>
                        <td>Summer Camp</td>
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
                        <td>3 Days</td>
                    </tr>
                    <tr>
                        <td>Participants</td>
                        <td>25 Treatment (68 Total)</td>
                    </tr>
                    <tr>
                        <td>Focus</td>
                        <td>Fruit and Vegetable Consumption</td>
                    </tr>
                    <tr>
                        <td>Controls</td>
                        <td>Haptic Joystick</td>
                    </tr>
                    <tr>
                        <td>Hardware</td>
                        <td>Mac, Novint Falcon</td>
                    </tr>
                    <tr>
                        <td>Publications</td>
                        <td>
                            <a href="https://www.researchgate.net/profile/Sun-Joo-Grace-Ahn/publication/281627304_Using_Virtual_Pets_to_Increase_Fruit_and_Vegetable_Consumption_in_Children_A_Technology-Assisted_Social_Cognitive_Theory_Approach/links/55f092ca08aef559dc46d679/Using-Virtual-Pets-to-Increase-Fruit-and-Vegetable-Consumption-in-Children-A-Technology-Assisted-Social-Cognitive-Theory-Approach.pdf">Paper</a>
                            <a href="https://www.proquest.com/dissertations-theses/design-field-implementation-virtual-buddy-based/docview/2917424271/se-2?accountid=14537">Dissertation Ch. 2.1</a>
                        </td>
                    </tr>
                </tbody>
            </table>
        </div> <!-- End VB-F&V Stats Table -->
    </details> <!-- End VB-F&V Stats -->
    <p>As part of this app, I implemented two different VB health checks: arterial elasticity and heart pumping. They were designed to represent different aspects of a child's VB. See below for more details on these health checks. In addition to these health checks, children were able to get their VFB to perform tricks and/or play fetch by spending trick credits earned through meeting their F&V goals.</p>
    <details open> <!-- VB-F&V Health Check Table -->
        <summary>VB-F&V Health Checks</summary>
        <!-- Arterial Elasticity -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-pic"> <!-- TODO: Pic -->
                <img src="vbFV_arterial_elasticity.png"
                    alt="A major artery of a heart inside a lab."
                    title="VB-F&V Arterial Elasticity Heath Check">
            </div> <!-- End Pic -->
            <div class="mgTable-list"> <!-- List -->
                <p class="mgTable-title">Arterial Elasticity</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Arterial elasticity check TODO:</li>
                    <li><u>Goal:</u> Determine the rigidity of a major artery TODO: </li>
                    <li><u>Controls:</u> Use haptic joystick to press on artery to see how much it depresses TODO:</li>
                </ul>
            </div> <!-- End List -->
        </div> <!-- End Table Cell -->
        <!-- End Arterial Elasticity -->
        <!-- Heart Pumping -->
        <div class="mgTable"> <!-- Table Cell -->
            <div class="mgTable-listLeft"> <!-- List -->
                <p class="mgTable-title">Heart Pumping</p>
                <ul class="mgTable">
                    <li><u>Type:</u> Heart pumping check TODO: </li>
                    <li><u>Goal:</u> Determine how difficult is it to pump the heart TODO:</li>
                    <li><u>Controls:</u> Use haptic joystick to pump heart and feel resistanceTODO:</li>
                </ul>
            </div> <!-- End List -->
            <div class="mgTable-pic"> <!-- TODO: Pic -->
                <img src="vbFV_heart_pumping.png"
                    alt="An anatomical heart in a lab."
                    title="VB-F&V Heart Pumping Health Check">
            </div> <!-- End Pic -->
        </div> <!-- End Table Cell -->
        <!-- End Heart Pumping -->
    </details> <!-- End VB-F&V Health Check Table -->
    <p>TODO: In addition to implementing these health checks, I was responsible for the following:</p>
    <ul> <!-- VB-F&V responsibilities list -->
        <li>Designing and implementing:</li>
        <ul> <!-- VB-F&V design and implement list -->
            <li>Haptic joystick input system</li>
            <li>Reward system based on fruit and vegetable consumption</li>
            <li>RFID login system</li>
            <li>Heart and artery testing minigames</li>
            <li>Updating gesture system to use the haptic joystick</li>
        </ul> <!-- End VB-F&V design and implement list -->
        <li>Observing and troubleshooting VB-F&V system throughout the study</li>
        <li>Administering post-treatment questionnaires</li>
    </ul> <!-- End VB-F&V responsibilities list -->
</details> <!-- End VB-F&V -->
