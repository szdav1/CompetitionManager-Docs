# Competition Control Logic

## Control and Data flow in a competition

---

Contents:

- Poule
  
  - Poule, poule control
  
  - PouleCompeition, PouleCompetition control

- Table
  
  - Table, table control
  
  - TableCompetition, TableCompetition control

- Competition

---

## Made by

- Szabó Dávid

- Szürke Levente

- Szántó Dávid

---

# Poule

> A poule is a specially structured spreadsheet for storing competitors' scores.
> 
> It also serves as the main data source for the rest of a competition, as every necessary data is calculated inside the poule.

![](C:\Users\Dave\IdeaProjects\CompetitionManager\Docs\pics\PouleScoresheet.png)

The above image (Free to download from [USA Fencing](https://www.usafencing.org/scoresheets)) shows how a poule looks like.

Every poule has its own controller that takes care of validating input and controlling control elements.

---

## PouleCompetition

The PouleCompetition panel stores multiple poules, distributes the competitors among the poules and controls the competition.

---

# Table

> A table is a binary tree on its side. It looks like every other table in other sports.

![](C:\Users\Dave\IdeaProjects\CompetitionManager\Docs\pics\Table.png)

The above image (Free to download from [USA Fencing](https://www.usafencing.org/scoresheets)) shows how a tavle looks like.

Every table has its own controller that takes care of validating input and controlling control elements.

Our project excludes bout for the 3rd place.

---

## TableCompetition

The TableCompetition panel stores the table, distributes the competitors and controls the competition.

---

# Competition

> The competition is conducted using the PouleCompetition and the TableCompetition. This way less code is written and the control logic will be more consistent.

![](C:\Users\Dave\IdeaProjects\CompetitionManager\Docs\pics\CompetitionControlFlow.png)
