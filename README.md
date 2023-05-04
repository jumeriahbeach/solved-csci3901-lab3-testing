Download Link: https://assignmentchef.com/product/solved-csci3901-lab3-testing
<br>
In this lab, you will expand your skills in developing test cases.

You will create test cases for a program that creates a leader board for a sports league.

You are not required to develop code for the test cases or to develop test input data for your test cases.

<h1>Preparation</h1>

You are going to help manage the leader board for a local sports league. The teams play against one another and the leader board is created by ordering the teams from most winning to least winning. Specifically, the first team on the leader board has the most game wins. If a tie happens between teams then the order of tie-breaking, in order of precedence, is:

<ul>

 <li>most games won</li>

 <li>most games tied</li>

 <li>most points scored by the team</li>

 <li>highest difference of points scored to points lost</li>

 <li>most games played</li>

 <li>lexicographic order of the team names</li>

</ul>

You will be writing test cases for a class for this problem. The methods in the class are as follows:

public boolean addTeam(String teamName) Adds the given team name as one team in the league. Returns true if the team was added to the league. Returns false if the team is already in the league or if any problem arose with the addition.

public boolean recordGameOutcome(String team1, String team2, int scoreTeam1, int scoreTeam2) Record that team1 played team2 and that the ending score was scoreTeam1 for team 1 and scoreTeam2 for team 2. Return true if the game was recorded. Return false if the game was not recorded or if any problem arose with the recording.

public String createLeaderBoard() Create a string that is the leader board for the league. The leader board lists all of the teams in the league in the order of most-successful team to least-successful team, based on game outcomes, as described earlier. Each line of the leader board string is as follows:

<ul>

 <li>team name (use 15 columns)</li>

 <li>number of games won (use 2 columns)</li>

 <li>number of games lost (use 2 columns)</li>

 <li>number of games tied (use 2 columns)</li>

 <li>points scored by the team (use 4 columns)</li>

 <li>points scored against the team (use 4 columns)</li>

</ul>

Include one space between each column.

There will also be a header row, with titles Team, W, L, T, +, and -, all right justified except “Team”.

The league has space for a maximum of 24 teams.

Given the following data for recordGameOutcome (4 method invocations)

“Anchor”, “Salty”, 15, 12

“RC”, “Kitchen Party”, 9, 11

“Anchor”, “RC”, 12, 7

“Salty”, “Kitchen Party”, 6, 0

We get the following leader board

<table width="273">

 <tbody>

  <tr>

   <td width="134">Team</td>

   <td width="27">W</td>

   <td width="23">L</td>

   <td width="34">T</td>

   <td width="40">+</td>

   <td width="16">−</td>

  </tr>

  <tr>

   <td width="134">Anchor</td>

   <td width="27">2</td>

   <td width="23">0</td>

   <td width="34">0</td>

   <td width="40">27</td>

   <td width="16">19</td>

  </tr>

  <tr>

   <td width="134">Salty</td>

   <td width="27">1</td>

   <td width="23">1</td>

   <td width="34">0</td>

   <td width="40">18</td>

   <td width="16">15</td>

  </tr>

  <tr>

   <td width="134">Kitchen Party</td>

   <td width="27">1</td>

   <td width="23">1</td>

   <td width="34">0</td>

   <td width="40">11</td>

   <td width="16">15</td>

  </tr>

  <tr>

   <td width="134">RC</td>

   <td width="27">0</td>

   <td width="23">2</td>

   <td width="34">0</td>

   <td width="40">16</td>

   <td width="16">23</td>

  </tr>

 </tbody>

</table>

<strong>Resources</strong>

<ul>

 <li>None required</li>

</ul>

<h1>Procedure</h1>

<strong>Set-up</strong>

<ol>

 <li>Ensure that all in your group understand and agree upon the intention of the problem. Do not make assumptions on how someone will implement a program to solve this problem.</li>

</ol>

<strong>Lab steps</strong>

<strong>Part 1 – Understand the problem</strong>

<ol>

 <li>Clarify any ambiguities that your team may have about the problem. Record these clarifications.</li>

 <li>Identify the boundary conditions that exist in the problem statement. Record these boundaries.</li>

 <li>Outline the type of control flow that <em>any </em>implementation for the problem will need to follow, based on the problem statement. Record these flows.</li>

 <li>Define what would be perceived as the “normal” order in which methods would be invoked for the problem.</li>

</ol>

<strong>Part 2 – Create test cases</strong>

<ol>

 <li>Identify a set of input validation tests for each method as well as the expected outcome for each case.</li>

 <li>Identify a set of boundary tests for these boundary cases.</li>

 <li>Identify a set of control flow tests.</li>

 <li>Identify a set of data flow tests based on your “normal” order.</li>

</ol>

<h1>Questions</h1>

How, if at all, would input validation change if you were getting input from a user interface rather than as parameters to methods?

Explain whether or not boundary cases exist beyond checking the incoming input values.

How does the idea of “control flow” change between black box tests and white box tests?

Should all permutations of methods result in data flow tests? Explain.

<h1>Reporting</h1>

<ol>

 <li>In one file, list

  <ul>

   <li>The members of your team.</li>

   <li>The clarifications and reporting from part 1.</li>

   <li>The tests from part 2, divided by test type.</li>

   <li>How complete you think that your test cases are.</li>

   <li>The answers from the Questions section of the lab.</li>

  </ul></li>

 <li>Generate a PDF from the document.</li>

 <li>Submit the PDF in Brightspace in the Lab/Lab 3 section of the course page in Brightspace.</li>

</ol>