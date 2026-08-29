# Cricket Scoreboard Pro

# CRICKETX — FIX CURRENT UI + BUILD REAL TOURNAMENT SCORING SYSTEM

You are working on my existing React + Vite + TypeScript cricket project called **CricketX**.

IMPORTANT: Do NOT create a completely separate project.

First inspect the existing project and fix the current implementation.

## CURRENT PROBLEM

The application is currently rendering like unstyled HTML.

The browser shows text such as:

CricketX

Scoreboard

Home Matches Live Teams Players Points Table Statistics Schedule About

CricketX — Every Ball. Every Run. Every Moment.

There are no proper cards, spacing, colors, buttons, layouts, icons, responsive design, or professional styling.

This means the CSS/Tailwind/styling setup is not being applied correctly.

### FIRST TASK — FIX THE UI

Inspect:

- App.tsx

- App.css

- index.css

- main.tsx

- package.json

- Tailwind configuration

- Vite configuration

- all component files

Find why the styling is not being loaded.

Do NOT simply hide the problem.

Fix the actual CSS configuration/import issue.

Make sure:

main.tsx imports the global CSS correctly.

App.tsx imports required styles correctly.

If Tailwind is configured incorrectly, fix the configuration.

If Tailwind is unnecessary or broken, use reliable CSS modules/global CSS instead.

After fixing it, verify that:

- Background colors work

- Cards work

- Buttons work

- Flex/grid layouts work

- Responsive design works

- Typography works

- Hover effects work

- Navigation works

Do not leave the application looking like raw HTML.

---

# SECOND TASK — TRANSFORM THIS INTO A REAL CRICKET TOURNAMENT MANAGEMENT SYSTEM

The primary purpose of this project is:

**I want to create a cricket tournament and manually enter scores for every match so the complete tournament can be maintained automatically.**

This is NOT just a website displaying static IPL data.

It should work like a real tournament scoring application.

Project name:

# CricketX

### Cricket Tournament & Live Scoring Management System

---

# 1. PROFESSIONAL UI

Create a premium modern cricket dashboard.

Design inspiration:

- Professional cricket score apps

- Sports analytics dashboards

- Modern IPL-style presentation

- ESPN/Cricbuzz-like information density

But create an ORIGINAL design.

Do NOT copy IPL branding, logos, copyrighted images, or exact layouts.

### Visual style

Use:

- Dark navy / black background

- Cricket green

- White cards

- Red/orange live indicators

- Subtle gradients

- Glass effects

- Stadium-inspired visuals

- Large score typography

- Professional tables

- Smooth animations

Use Lucide icons.

Use proper spacing.

Use responsive CSS.

---

# 2. TOURNAMENT CREATION

Add an Admin Dashboard.

Admin should be able to create a tournament.

Example:

Tournament Name:

CricketX Premier League 2026

Season:

2026

Number of Teams:

10

Format:

- T20

- ODI

- Test

Overs:

20

Start Date:

End Date:

Venue:

Tournament logo/banner:

Save Tournament.

---

# 3. TEAM MANAGEMENT

Admin can create teams.

Team fields:

- Team Name

- Short Code

- City

- Captain

- Vice Captain

- Coach

- Team Logo

- Team Color

Example:

Royal Challengers Bengaluru

RCB

Bengaluru

Chennai Super Kings

CSK

Chennai

Mumbai Indians

MI

Mumbai

etc.

Do not depend on copyrighted team logos.

Allow custom logo upload or generated placeholders.

---

# 4. PLAYER MANAGEMENT

Admin can add players.

Fields:

Player Name

Role:

- Batsman

- Bowler

- All Rounder

- Wicket Keeper

Batting Style

Bowling Style

Team

Jersey Number

Player Image

Create player profiles.

---

# 5. TOURNAMENT MATCH CREATION

Admin should be able to create matches.

Form:

Tournament

Match Number

Date

Time

Venue

Team A

Team B

Match Type

Overs

Umpires

Status

Status options:

- Scheduled

- Live

- Completed

- Abandoned

Example:

Match 1

RCB vs CSK

27 August 2026

7:30 PM

M. Chinnaswamy Stadium

---

# 6. PLAYING XI SELECTION

Before starting a match:

Select Playing XI for Team A.

Select Playing XI for Team B.

Allow:

- 11 players

- Substitute players

Select:

Captain

Wicketkeeper

---

# 7. TOSS

Before starting the match:

Team A won toss.

Options:

- Bat

- Bowl

Save toss result.

---

# 8. LIVE SCORING PANEL

THIS IS THE MOST IMPORTANT PART.

Create a dedicated scorer interface.

The scorer should be able to maintain the entire match ball-by-ball.

Layout:

LEFT:

Current batsmen

RIGHT:

Bowler

CENTER:

Large score

BOTTOM:

Scoring buttons

---

# 9. SCORING BUTTONS

Create large easy-to-click buttons:

0

1

2

3

4

5

6

WIDE

NO BALL

BYE

LEG BYE

WICKET

Buttons must be designed for fast scoring.

The scorer should be able to operate the system during a real match.

---

# 10. SCORE AUTOMATICALLY

When scorer clicks:

FOUR

Automatically update:

Team Score +4

Batsman Runs +4

Ball +1

Boundary +1

Strike Rate

Current Run Rate

Over

Scorecard

Commentary

When scorer clicks:

SIX

Update all relevant statistics.

When scorer clicks:

WIDE

Update:

Team Score +1

Extras +1

Bowler Runs +1

DO NOT count it as a legal delivery.

When scorer clicks:

NO BALL

Update:

Team Score +1

Extras +1

Bowler Runs +1

DO NOT count it as a legal delivery.

If no-ball + bat runs are entered, calculate correctly.

---

# 11. WICKET SYSTEM

When WICKET is clicked, open a modal.

Ask:

Dismissed Batsman

Wicket Type:

- Bowled

- Caught

- LBW

- Run Out

- Stumped

- Hit Wicket

- Retired Hurt

If Caught:

Select Catcher.

If Run Out:

Select fielder.

After wicket:

Ask for new batsman.

Update:

Wickets

Batting scorecard

Fall of wickets

Current batsman

Partnership

Commentary

---

# 12. STRIKE ROTATION

Implement proper cricket strike logic.

Automatically rotate strike when required.

Handle:

- Odd runs

- End of over

- Boundaries

- Extras

- Wickets

Do not use simplistic decimal-over calculations.

Internally track:

legalBalls

Example:

19 overs + 5 balls

Display:

19.5

But internally:

233 legal balls

---

# 13. CURRENT SCORE DISPLAY

Create a premium live scoreboard:

LIVE

RCB

187 / 5

19.2 Overs

Current Run Rate:

9.67

Required:

42 runs

from 10 balls

Required Run Rate:

25.20

Target:

230

---

# 14. CURRENT BATTERS

Display:

Virat Kohli

72 (48)

4s: 6

6s: 2

SR: 150.00

Rajat Patidar

41 (25)

4s: 3

6s: 2

SR: 164.00

Show a ⭐ or strike icon beside the striker.

---

# 15. CURRENT BOWLER

Example:

Jasprit Bumrah

3.2 overs

28 runs

2 wickets

Economy:

8.40

Maidens:

0

---

# 16. BALL-BY-BALL COMMENTARY

Automatically generate commentary.

Examples:

19.1 — 1 run

19.2 — FOUR!

19.3 — SIX!

19.4 — WICKET!

19.5 — Wide

19.5 — 2 runs

19.6 — Dot ball

Store every delivery in the database.

---

# 17. OVER SUMMARY

After each over show:

Over 19

1 4 0 W 6 1

Over Runs:

12

Total:

187/5

Create a visual ball timeline.

---

# 18. INNINGS BREAK

When innings ends:

Show:

INNINGS BREAK

RCB

187/5

20 Overs

Top Scorer:

Virat Kohli — 82

Best Bowler:

Bumrah — 3/28

Target:

188

Then provide:

START 2ND INNINGS

button.

---

# 19. SECOND INNINGS

Repeat the scoring system for Team B.

Automatically calculate:

Target

Required Runs

Required Balls

Required Run Rate

Current Run Rate

Wickets Remaining

---

# 20. MATCH RESULT

Automatically determine result.

Example:

RCB won by 22 runs.

Or:

CSK won by 5 wickets.

Or:

Match tied.

Or:

No Result.

Store result permanently.

---

# 21. COMPLETE SCORECARD

After match completion display:

## Batting

Player

Dismissal

Runs

Balls

4s

6s

Strike Rate

## Bowling

Bowler

Overs

Maidens

Runs

Wickets

Economy

## Extras

Wides

No Balls

Byes

Leg Byes

Penalty

## Fall of Wickets

1-42

2-87

3-121

etc.

---

# 22. TOURNAMENT POINTS TABLE

THIS MUST UPDATE AUTOMATICALLY.

Columns:

POS

TEAM

P

W

L

NR

PTS

NRR

After every completed match:

Automatically update:

Matches Played

Wins

Losses

No Results

Points

Net Run Rate

Do NOT manually enter the points table.

Calculate it from match results.

---

# 23. NET RUN RATE

Implement proper tournament NRR calculation.

NRR:

Total runs scored / total overs faced

minus

Total runs conceded / total overs bowled

Handle all-out innings correctly according to the tournament rules.

Create reusable utility:

calculateNetRunRate()

---

# 24. TOURNAMENT DASHBOARD

Create:

## Tournament Overview

Tournament name

Matches Played

Matches Remaining

Teams

Top Run Scorer

Top Wicket Taker

Current Leader

Upcoming Match

Latest Result

---

# 25. TOURNAMENT STANDINGS

Create a dedicated Points Table page.

Show:

Position

Team

Played

Won

Lost

NR

Points

NRR

Highlight:

Playoff qualification positions.

---

# 26. TOURNAMENT SCHEDULE

Display:

Completed matches

Live matches

Upcoming matches

Allow filtering by:

Date

Team

Status

---

# 27. MATCH HISTORY

Admin should be able to view all completed matches.

Each match should show:

Teams

Score

Winner

Date

Venue

Player of Match

View Scorecard

---

# 28. PLAYER TOURNAMENT STATISTICS

Automatically calculate tournament statistics from match data.

### Batting

- Total Runs

- Matches

- Innings

- Average

- Strike Rate

- Highest Score

- 50s

- 100s

- Fours

- Sixes

### Bowling

- Matches

- Overs

- Runs

- Wickets

- Economy

- Average

- Best Bowling

- Maidens

Do NOT manually duplicate statistics.

Calculate from deliveries and scorecards.

---

# 29. PLAYER OF THE MATCH

After completing a match:

Admin can select:

Player of the Match.

Save it.

Display it on:

Match result

Player profile

Tournament statistics

---

# 30. DATABASE

Use Supabase PostgreSQL.

Create a proper relational database.

Tables:

profiles

tournaments

teams

players

venues

matches

playing_xi

tosses

innings

deliveries

batting_scorecards

bowling_scorecards

wickets

partnerships

match_results

points_table

player_tournament_stats

player_of_match

---

# 31. DELIVERY TABLE

This table is extremely important.

Each delivery should store:

id

match_id

innings_id

over_number

ball_number

striker_id

non_striker_id

bowler_id

runs_batter

runs_extras

total_runs

extra_type

is_legal_delivery

is_wicket

wicket_type

dismissed_player_id

fielder_id

created_at

Every scoring action creates one delivery record.

---

# 32. REAL-TIME SCORE

Use Supabase Realtime.

When scorer enters a ball:

Database updates immediately.

Live viewers see the new score without refreshing.

---

# 33. ADMIN ROUTES

Create:

/admin

/admin/tournaments

/admin/teams

/admin/players

/admin/matches

/admin/matches/:id/scoring

/admin/matches/:id/edit

---

# 34. USER ROUTES

Create:

/

/matches

/live

/matches/:id

/teams

/teams/:id

/players

/players/:id

/points-table

/statistics

/schedule

/about

---

# 35. SECURITY

Use Supabase Authentication.

Roles:

Admin

Scorer

Viewer

Only Admin and Scorer can modify scoring.

Viewers can only read data.

Implement Row Level Security.

Never expose Supabase service-role keys in frontend code.

---

# 36. UNDO LAST BALL

The scorer MUST have:

UNDO LAST BALL

button.

If accidentally entering a wrong score:

Click UNDO LAST BALL.

Restore:

Score

Batsman

Bowler

Over

Wickets

Extras

Strike

Partnership

Commentary

Database state

This is extremely important for real scoring.

---

# 37. EDIT PREVIOUS DELIVERY

Allow admin/scorer to edit a previous delivery.

After editing:

Recalculate the innings.

Recalculate:

Score

Batting

Bowling

Extras

Wickets

Overs

Run Rate

Tournament statistics

---

# 38. AUTO SAVE

Every scoring action should automatically save to Supabase.

Show:

✓ Saved

or

Saving...

Do not lose the score if the page refreshes.

---

# 39. MOBILE SCORER MODE

The scoring interface must work extremely well on mobile.

Buttons should be:

Large

Easy to tap

Clearly labeled

Example:

┌────┬────┬────┐

│ 0 │ 1 │ 2 │

├────┼────┼────┤

│ 3 │ 4 │ 6 │

├────┼────┼────┤

│ W │ WD │ NB │

└────┴────┴────┘

This should feel like a real cricket scorer application.

---

# 40. DEMO TOURNAMENT

Create a demo tournament:

CricketX Premier League 2026

Add:

10 teams

100+ players

Multiple venues

20+ scheduled matches

Some completed matches

One live demo match

Use clearly labeled demo data.

---

# 41. UI COMPONENTS

Create reusable components:

Navbar

Sidebar

TournamentCard

MatchCard

LiveMatchCard

ScoreHeader

BattingTable

BowlingTable

BallTimeline

ScoringPad

WicketModal

ExtrasModal

PartnershipCard

PointsTable

PlayerCard

TeamCard

TournamentStats

MatchResult

CommentaryPanel

AdminSidebar

LoadingState

ErrorState

---

# 42. IMPORTANT CODE ARCHITECTURE

Do NOT put all scoring logic inside React components.

Create:

src/

components/

pages/

layouts/

services/

hooks/

types/

utils/

lib/

data/

Create a dedicated:

src/utils/cricketEngine.ts

It should contain functions such as:

calculateScore()

calculateOvers()

calculateStrikeRate()

calculateEconomy()

calculateRunRate()

calculateRequiredRunRate()

calculateNRR()

calculatePoints()

processDelivery()

processWicket()

rotateStrike()

undoDelivery()

recalculateInnings()

---

# 43. FINAL TESTING

Before finishing:

Run:

npm install

npm run dev

Then test:

1. Create tournament

2. Add teams

3. Add players

4. Create match

5. Select playing XI

6. Record toss

7. Start innings

8. Score 1

9. Score 4

10. Score 6

11. Record wide

12. Record no-ball

13. Record wicket

14. Add new batsman

15. Complete over

16. Complete innings

17. Start second innings

18. Complete match

19. Generate result

20. Update points table

21. Update NRR

22. Update player statistics

23. Check match history

24. Refresh browser

25. Confirm data remains saved

26. Test mobile layout

Fix all errors before considering the project complete.

---

# MOST IMPORTANT REQUIREMENT

I am going to use this application to **actually maintain a cricket tournament by entering scores match-by-match**.

Therefore, prioritize:

1. Reliable scoring engine

2. Correct ball/over calculations

3. Correct wickets/extras

4. Automatic scorecard

5. Automatic match result

6. Automatic points table

7. Automatic NRR

8. Automatic player statistics

9. Supabase persistence

10. Real-time updates

11. Undo/edit scoring

12. Professional UI

Do not make this a static IPL clone.

Make it a **real tournament management and live cricket scoring platform**.

First fix the current unstyled/raw HTML problem, then implement the tournament management and scoring system in the existing project.

After every major change, verify the application compiles successfully and has no TypeScript/runtime errors.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/5a02e7a4-e266-442c-aa1b-bac146522dad).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
