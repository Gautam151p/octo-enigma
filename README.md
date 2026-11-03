# SQL Quest: The Data Dungeon

A self-contained, browser-based adventure for learning practical SQL. Open `index.html` in a modern browser to play; no installation, server, or external assets are required.

## How to play

1. Choose a hero: DB Brute, Query Ranger, Server Crusher, Schema Lich, SQL Mage, or Index Thief. These portraits are cosmetic for now; you can change your hero with **Change Hero**.
2. Read the lesson, guide tip, and SQL example at each chapter. Optionally edit the example and check it with the practice keyword checker.
3. Enter a regular encounter and answer two four-choice questions to defeat the guardian.
4. A correct answer damages the guardian; a wrong answer costs one of your three hearts. As you travel, the torchlit stone dungeon changes from a green grove to icy caverns, an ember-lit forge, a violet crypt, and the Overlord's red throne room.
5. After groups of lessons, face a skull-marked boss. Write a SQL query for each mixed-topic challenge; a matching query hits the boss, and an incorrect query costs a heart. Bosses ask more questions and award extra XP.
6. If you lose all your hearts, restart that topic or boss to begin its encounter again. Previously cleared chapters and XP are kept.
7. The enlarged torchlit arena features compact, detailed hero portraits inspired by the character blueprints: an armored DB Brute, elven Query Ranger, orc Server Crusher, hooded Schema Lich, blue-robed SQL Mage, and masked Index Thief. Each has a distinct silhouette, outfit, and signature weapon or magic; the selected class badge and accent remain visible. The bestiary includes the Syntax Bug, Null Phantom, Deadlock Ghoul, and Injection Demon, along with mythical bosses. Defeated enemies blur and fade from the arena; running out of hearts fades your hero.
8. Pick an attack from your spell arsenal. Defeating key guardians and bosses unlocks elemental attacks, including Fire Blast, Ice Shard, Lightning Shock, Earth Rupture, Shadow Pulse, and Starfall. Choose from your unlocked attacks on the victory screen or in the arsenal before a fight. Attacks launch across the arena with hit effects and a brief screen shake; reduced-motion settings disable the animations.

Progress, your hero, and your selected attack are saved in browser local storage on your device. Use **Reset Adventure** to clear them and choose a new hero. The SQL database-and-wand artwork appears as the game logo and browser-tab icon.

The six character portraits in the picker are read from `assets/character_portraits.png`, a 1920 × 450 horizontal sprite sheet with six 320 × 450 frames ordered DB Brute, Query Ranger, Server Crusher, SQL Mage, Schema Lich, and Index Thief. If the portrait asset is missing or has different dimensions, the picker reports that and displays the class icons.

Combat uses the corresponding full-body models from `assets/in_game_full_models.png`, normalized to the same six-frame, 1920 × 450 layout and class order. The selected character is saved with the adventure and determines the combat sprite; if the full-model sheet cannot load, the built-in SVG portrait is used instead.

## Curriculum

The 30 SQL lessons cover `SELECT` and `FROM`, `DISTINCT`, `WHERE`, boolean logic, `IN` and `BETWEEN`, `LIKE`, `NULL`, sorting, result limits, aggregate functions, `GROUP BY`, `HAVING`, aliases, `CASE`, text and dates, table DDL, `INSERT`, `UPDATE`, `DELETE`, constraints and keys, joins, set operations, subqueries, CTEs, window functions, views, indexes, transactions, normalization, and parameterized queries. Five stronger, red-and-skull-marked boss chapters follow lessons 7, 15, 21, and 29, then the final lesson. Their quizzes review the SQL topics covered so far.

The optional lesson practice checks for required keywords. Boss battles compare your normalized query against accepted reference solutions; neither feature executes SQL against a database. Syntax and feature support can vary among database systems, as noted in the relevant lessons.
