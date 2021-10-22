# Questions

1. At what age is the surgery done?

- Right before they are starting to play the game. From the first half year onwards.
Boundaries (in years): Starting at 5 - ?

2. Due to bad hearing problem, how were the children taught to pronounce letters?

- They know sign language (We can use it inside the game)

3. After the surgery, how long does it take the wound to heal so the process can start?

- For 1 Month they do nothing
- Then they switch it on for 1 or 2 frequency-ranges (more simple scope of the game)
- 6 Months the frequencies extend to ~16 frequency-ranges

4. How long does the battery of the implant last?

- Charing via induction
- 1 day should not be a problem
- You have to exchange the battery after 2 yrs.

5. Will the target group consist of 5 year-olds?

- Starting with 5 year-olds

6. How old can the kids be?

- **Mostly 5 year-olds**
- Mby in the future for adults too

7. Who should be able to provide content for the game?

- Teachers
- Parents

8. Are those people versed in IT?

- Not versed (Easy to use UI)

9. Is playing these games mandatory for the children?

- Its optional

10. Are we targeting any platforms besides desktop?

- Moodle (also an app for the smartphone)

11. How familiar are the kids with sounds and sign language (scale 1-10)?

- Sign-language (10)
- Sound (0)

12. by whom is the sign-language tought?

- By the parents
- By the family
- Teachers
- Has to be used accordingly

## Misc

Email: gerd.moeckel@srh-imd.de

## Status presentation content

- We want to present about the problem space (**Design Thinking**) and brainstorming
  - Matrix
  - Personas
  - PoV (Point of View)
- Provide idea in which direction well be developing the game scenario
- Mby use mascot (Team 4)
- Mby consolidate with team 1 and 2 (3)
  - What is possible
  - Briefly include into the presentation
- Mby other schools can participate within the system

## Feedback for the brainstorming

- Learning curve (Progression)
- Ranking System
- Rewards
- Skins (?)
- C/L-MS (Content/Learning-Management System) features
- Voice-chat (Sign-language Chat) (Be careful...What is the meaning?)
- Games should also train reflexes | dexterity (First start without time-concerns...mby after some time...advanced players) [In multiplayer u can have a time-based ranking]
- 2D - 3D ???
- 2D: Mby platformer -> procedurally generated world (enemies/bosses) with themes that can be customised with assets - (using imgs and sounds) [Singleplayer AND Multiplayer] (Style=Pixelart)
- 3D: Minigames like golf, airhockey -> mixed with quizzes [Multiplayer]
- Focus on Sign-language, symbols and Sound

## Brainstorming

- For example
  - **Throwing darts**, **golf**, **(table)tennis**, **football**, **parks with a slide**, **animals with sounds**, **dinosaurs sounds not as good**, **cartoons (mixed with animals) work with the mascot**, **traffic...cars, motorcycles**
  - Feedback as
    - Sound (Positive or negative feedback depending on the result)
    - Sign (from sign-language)
    - Symbol like icons or emojis

## Questions for team 7 (free game)

- What kind of game-ideas have you been able to come up with already?
- Be sure to not end up with the same idea

## Questions for team 5 and 6 (quiz and memory)

- How do you innovate your gamemodes further from your current prerequisites?

## Questions for team 4

- What are the restrictions for the UI/UX we have to use for our game?
- What does the mascot look like?

## Questions for team 3

- Written in php
- What are the given interfaces to extend moodle?
  - Plugin in the backend and frontend
- What database do you use?
  - Some SQL dialect
    - Hybrid with resources (Mby nfs storing the path in the db)
- Can you tell us something about your:
  - Motivation: Write a 25 page report
  - Challenges: Moodle supports rdbms...not sure how good the implementation works...iops might get reduced
  - Needs:
    - Get in touch for clear communication
  - Wants:
    - A game that is scalable
    - Easy game

1. There can be different type of data (Text to speech)
2. uploaded data will be verified by the school

## Questions for team 2 (Backend)

- What language do you use on the backend?
- What database do you use?
- Is it possible to implement a VR/AR game with that tech-stack?
- is there a list of exception of things we can not implement or not use?
- Can you tell us something about your:
  - Motivation:
  - Challenges:
  - Needs:
  - Wants:

## Questions for team 1 (Frontend)

- Do you use any frameworks on the frontend
- Can we use the html-canvas and WebGL to render our game?
- Any specific frontend-tech we cannot use?

## Considering persona

- Name:
- Age:
- Marital-status:
- Profession:
- Team-name:
- Motivation:
- Challenges:
- Needs:
- Wants:

## Personas

- Teacher [Mahima]
- Parent [Mahima]
- Dean? [Mahima]
- Student [Mahima]
- Doctor [Mahima]

- Team 1 (Frontend) [Niklas]
- Team 2 (Backend) [Niklas]
- Team 3 (Moodle) [Finished]
- Team 4 (UI/UX) [Niklas]
- Team 5 (Quiz game mode) [Vipul]
- Team 6 (Memory game mode) [Vipul]
- Team 7 (Free game mode) [Vipul]

## Questions to us from team 2

- Name of App.
  - Not available yet.
- Available in Platform.
  - Moodle
- What help you require from the backend team?
  - What language do you use on the backend?
  - What database do you use?
  - Is it possible to implement a VR/AR game with that tech-stack?
  - is there a list of exception of things we can not implement or not use?
  - Can you tell us something about your:
    - Motivation:
    - Challenges:
    - Needs:
    - Wants:
- In what format do you want the data?
  - We don't know :)
  - Why are you asking?
- What all data needs to be encrypted?
  - No data encryption please :)
  - Only encrypt the path
  - If you encrypt it you need to hash + encrypt so you can query which is n*2 size
- How will the integration work between frontend and backend?
  - Not our job :/
  - Use APL programming language mby
  - Multiplayer mby websockets...or webRTC for peer to peer
- What data needs to be saved?
  - Information about the user like
    - Progress
    - Rewards
- Will there be guest users?
  - No
- What all privileges admin would like to have?
  - Mutate state :)
- What all information would you acquire from the user? (If Biometrics are involved, what are they?)
  - Name
  - Age
  - Height
- Would this be plugin work as a web application / Mobile application / both?
  - I guess both thehe
- How many user modules(number of entities)?
  - As many as possible
- How many tabs does your dashboard have?
- What level of user accessibility each entity has(meaning: authorisation primarily)
  - Analytics page with a graph of progress
- Examples:
  - Parents can access their child’s profile
  - Children have limited access to details
  - Doctors have access to parents as well as child’s progress and involvement report.
- Who would be able to change master data, and what information are users/doctors/children/parents allowed to update?
  - Parents and teachers are able to upload content like images, sound and (videos)
  - Doctors can only read...analytics...metrics
- Do you use password management system? (if yes, for recovery, would their personal id’s be stored as well)?
  - We use moodle to authenticate
- Do you use SSO( Single sign on (FB/Google/Email) for creating profiles) and any tracking service for them if they are lost or need support?
  - No...We use moodle to authenticate
- Do you have a grievance section for continuous evolution of your game? (To report issues faced by certain kid)
  - Yes we ofc thought about that
- How often would you update the progress details for doctors to monitor?
  - Realtime
- Quiz examples: if you could give examples to help us decide the schema and decide on our databases.
  - Yeah not that far yet
- Brief Description and Features.
  - We are still trying to understand the problem :) Sowwy uwu ^.^
