---
title: Element Testing Page
draft: true
---

<style>
.stats-container2 {
    width: flex;
    justify-content: center;
}

details {
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

details[open] + div.stats-table-content {
    max-height: 800px; /* Set a max-height value enough to show all the content */
    transition: max-height 400ms ease-out, border 0ms linear;
}

details[open] summary::before {
    rotate: 90deg;
    transition: rotate 200ms ease-out;
}
</style>

A page for constructing and testing various elements on a clean space

Testing new elements here for now <3

TODO: last things left: get the arrow back and rotating and centering table

<div class=stats-container2>
    <details open>
        <summary class="stats-table-summary" role="term" aria-details="pure-css">
           VFB-H Stats
        </summary>
    </details>
    <div role="definition" id="pure-css" class="stats-table-content"> <!-- VFB-H Stats Table -->
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
</div>