---
title: Element Testing Page
draft: true
---

<!-- //TODO: add sliding up/down animation for tables
// a solution: https://nerdy.dev/open-and-close-transitions-for-the-details-element -->

<style>
.stats-container2 {
    width: flex;
    justify-content: center;
}

details.stats-table {
    max-width: 500px;
    overflow: hidden; /* Keep this line to prevent an odd blue outline around the element in Safari. */
    background: light-dark(royalblue,#3e5d7b);
    box-shadow: 3px 3px 3px #797979;
    border-radius: 5px;
    flex-basis: 52%;
    position: relative;
    width: flex;
    justify-content: center;
}

.stats-table-summary {
    display: flex;
    color: light-dark(#efefef,lavender);
    justify-content: center;
}

.stats-table-summary::-webkit-details-marker {
    display: none;
}

.stats-table-summary:hover {
    cursor: pointer;
}

.stats-table-summary::before {
    content: "►";
    font-size: 1rem;
    display: flex;
    align-items: center;
    margin-right: 0.5rem;
    transition: rotate 200ms 400ms ease-out;
}

div.stats-table-content {
    box-sizing: border-box;
    max-width: 500px;
    max-height: 0;
    overflow: hidden;
    padding: 0 10px;
    transition: max-height 400ms ease-out, border 0ms 400ms linear;
    background-color: #797979;
    box-shadow: 3px 3px 4px #797979;
    border-radius: 5px;
    display: flex;
    width: flex;
    justify-content: center;
}

div.stats-table-content tr:nth-of-type(even) {
    background-color: light-dark(royalblue,#3e5d7b);
}

div.stats-table-content td {
    color: light-dark(#efefef,lavender);
}

div.stats-table-content a {
    color: light-dark(#efefef,lavender);
    text-decoration: underline;
    font-style: italic;
}

details.stats-table[open] + div.stats-table-content {
    max-height: 800px; /* Set a max-height value enough to show all the content */
    transition: max-height 400ms ease-out, border 0ms linear;
}

details.stats-table[open] summary.stats-table-summary::before {
    rotate: 90deg;
    transition: rotate 200ms ease-out;
}
</style>

A page for constructing and testing various elements on a clean space

Testing new elements here for now <3

TODO: last things left: 
- get the arrow back 
- get the arrow rotating 
- center table on page
- make the scroll bar not show up when closing/opening ONLY

<div class=stats-container2>
    <details open class="stats-table">
        <summary class="stats-table-summary" role="term" aria-details="pure-css">
           VFB-H Stats
        </summary>
    </details>
    <div role="definition" id="pure-css" class="stats-table-content"> <!-- VFB-H Stats Table -->
        <table>
            <tbody>
                <tr>
                    <td>Name</td>
                    <td>Virtual Fitness Buddy At-&NoBreak;Home (VFB-&NoBreak;H)</td>
                </tr>
                <tr>
                    <td>Dates</td>
                    <td>Fall&nbsp;2021 to Spring&nbsp;2022</td>
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
                    <td>25&nbsp;Treatment (44&nbsp;Total)</td>
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
                    <td><a href="https://esploro.libs.uga.edu/esploro/outputs/doctoral/Design-and-Field-Implementation-of-Virtual/9949618127102959">Dissertation Ch.&nbsp;5</a></td>
                </tr>
            </tbody>
        </table>
    </div> <!-- End VFB-H Stats Table -->
</div>