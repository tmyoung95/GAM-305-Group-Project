**Project Log Assignments**\
**4-2 Project Log**

**What parts of the testing process did the team perceive to go well?**

The team felt that early functional testing during the alpha stage went especially well. Because we focused on testing core mechanics inside simple test maps before worrying about level design, we were able to catch a lot of issues with core elements like pickups, widgets, and enemy behavior early. Systems like health restoration, armor chunk logic, and damage application were easier to fine tune since we isolated them first. The checklist approach also helped keep everyone aligned, since we always knew exactly what behavior we were intently verifying instead of just testing casually. Multiple team member's input allowed for layers of testing to yield maximal bug identification.

**How were bugs identified and corrected?**

Most bugs were identified through individual playtesting sessions where team members would test newly implemented mechanics catagorized on our Needs Testing Trello card catagory. When something did not behave as expected, it was logged in Trello as Tested (failed) with notes describing what happened and under what conditions. The person responsible for that system would then adjust the blueprint logic or settings, after which another team member retested it to make sure the issue was actually resolved. This back and forth helped reduce repeat problems, especially with things like collision on traps, enemy damage registration, and UI updates for armor and health.

**In terms of the QA and testing process, what would you do differently to improve the process?**

Our team did not have many problems with testing processes admittedly. Functionality was tested thoroughly by each team member as new features were developed in tandem with existing features. For example, heallth restoration mechanics were tested again after developing the player UI widget that displays how many health items the player was holding just to make sure nothing was breaking under the hood. If anything, one change we would make as a team would be better dividing the feature deadlines a bit better, as we front loaded alpha phase with some of the most critical and complex elements of our game. While things have gone smooth despite this, we understand that we made Alpha phase perhaps a bit harder than it needed to be.  

**What tools (chosen in Module Two) did you find successful in the development of your Alpha project? Why?**

Trello was very successful because it gave us a shared view of what was being worked on, what passed testing, and what still had problems. It helped prevent confusion about task ownership and kept testing tied directly to features. Discord was also effective for quick communication, especially during live troubleshooting when someone could share their screen and walk through blueprint logic. Frequent meetings helped align the team on prioriites, feature development sequence, and general support check ins. The discord chat helped streamline topics and gave us a history of any development challenges and their solutions. The internal development document helped remind the team of our objectives and required elements, and all team members were notified as the document was updated. 

**Were there any tools or techniques that you did not find helpful in the success of your project development? Why?**

The team feels that none of the tools utilized had any negative drawbacks. While minimalistic, each tool provided a clear purpose and a means to easily and clearly communicate project needs on a regular basis.  

**How did the team approach to the initial analysis of the game design document contribute to the decision to use these tools and techniques?**

Because we broke down the design document into specific systems early, like health, armor chunks, weapon pickups, enemies, and traps, it made sense to use tools that supported tracking individual features. Trello matched this system by system structure well, and our checklist came directly from the mechanics defined in the design. The design document also made it clear that progression and survival systems were core to the experience, which is why we focused testing around core mechanics rather than just visuals or environment details during Alpha phase.

All content was collaboratively developed by all members of the development team:

- Ziqura Thomas
- Amya Overton
- Anthony Munson
- Tyler Young





**3-2 Project Log: QA and Testing Plan**

**How will you test objects, levels, and games during the development cycle? Develop a schedule and include Play Test, Demo, and Code Release.**

Play Test will occur during preproduction and early development, primarily in Weeks 3 and 4. The goal is to verify that the core mechanics work inside designated test maps before the team commits to beta goals (level building, star/end progression, refinement, etc.). During this stage the team will test basic health and respawn functionailty,  object prototypes for power up pickups, player equipment pickups, moving enemies, and stationary obstacles, along with basic player combat and enemy AI behavior. This includes verifying that the health item restores health correctly, ammo pickups add ammunition properly, the battery restores flashlight power, and the adrenaline shot increases speed temporarily and then returns to normal. It also includes verifying that armor plates work as a four chunk system and that small plates restore one chunk, medium plates restore two chunks, and large plates restore all four. Weapon pickups will also be tested in this stage so the knife, pistol, and shotgun can be equipped and used reliably.

Demo testing will occur at the end of beta phase in Week 5 before the beta branch is finalized. The goal is ensuring all previous alpha functionality works in the newly dveloped beta environment. At this point the team will run full playthroughs through the current level progression route in the implemented rooms. Demo testing will focus on making sure the player can progress without being blocked by barriers, keys, or triggers, and that barriers correctly prevent progression until the intended requirement is met. Primary goals here would ensure that level designs are cohesive and placement of traps, pickups, and enemies are appropriate and to the benefit of the project. The team will also ensure that asset placement within the level does not contribute to any hindrance of player movement or game progression.  

Code Release testing will occur after beta phase in Week 5, during polishing in Weeks 6 and 7. The goal is to check the code release demo against the test plan and ensure the final build matches the selected scenario document requirements. The team would be focused on identifying remaining issues with combat responsiveness and refining the gameplay loop to enhance the player experience. Any bugs found in this pahse will be reported, reworked, and retested until all sytems on the task checklist have been completed, especially in the event of regression as final tweaks to the game are being made.  

**What items will be tested? Include a checklist of items to be tested (pass/fail).**

The following checklist will be used during testing. Each item is recorded as pass or fail during each milestone test session:

- Player movement and camera controls
- Health system decreases correctly when damaged
- Health pickup restores health correctly
- Armor system displays four chunks correctly
- Armor plates restore the correct amount of armor for small, medium, and large plates
- Damage is applied to armor first, then health when armor is empty
- Knife pickup equips and can be used reliably
- Pistol pickup equips, fires, and deals damage reliably
- Shotgun pickup equips, fires, and deals damage reliably
- Grenade functions correctly if implemented as the stretch goal
- Ammo pickups increase ammo for the correct weapon type
- Battery pickup restores flashlight power correctly
- Adrenaline shot increases speed temporarily and returns to normal afterward
- Quicker enemy moves faster than tank enemy and deals lower damage
- Tank enemy moves slower than quicker enemy and deals higher damage
- Enemy melee attacks register damage correctly without double hits or missed hits
- Bear trap triggers on contact, immobilizes the player, and deals damage
- Saw trap triggers correctly, deals damage, and applies bleeding
- Pitfalls trigger instant kill consistently
- Barriers block progression until the correct condition is met
- Level progression from start to end location is clear and functional
- Player cannot get stuck in geometry or fall out of the level
- UI displays health, armor, ammo, and key survival info correctly
- No crashes during a normal playthrough
- No soft locks where the player cannot continue
- Animations, if implmented as the stretch goal, behave normally and do not contribute to issues with player movement/physics

**How will you update the test plan to reflect changes to the game and design document?**

The test plan will be updated any time the design document or implemented gameplay changes. If a feature is added, such as the grenade stretch goal, a new test item is added with clear expected behavior. If a mechanic is modified, such as adjusting how long bear traps immobilize the player or changing adrenaline duration, the existing test criteria is revised to match the new intended behavior. If content is cut, the related test items are removed so the checklist stays accurate and does not waste time testing features that no longer exist. All tracking of test items are tracked using Trello.

**How will bugs be reported?**

Bugs will be reported through Trello so the team has one centralized place for issues. Currently, catgories for the Trello cards include a Tested (passed) and a Tested (failed) category. If a bug is found for any specific feature, the card name is amended to reflect the bug details, and is consequently moved to the Tested (failed) category. Then the team can troubleshoot nd make any neessary changes before testing until the card can be moved to Tested (passed).

**How will the bugs and their changes be tracked over time?**
Bug progress and changes will be tracked in Trello using a consistent status workflow. Bugs will move from new to in progress to fixed to needs retesting to closed. When a bug is marked fixed, another team member retests it using aformentioned testing protocols. If it fails again, it is moved back to Tested (failed) with notes on what still occurs. This makes it easy to track what has been resolved, what is still active, and whether any fixes caused regressions in systems like pickups, traps, enemies, or progression. Additionally, the team maintains and updates an internal project document, where specific reports on feature changes can be logged and reviewed at anytime to ensure a history of bugs is present through the development lifecycle. 

All content was collaboratively developed by all members of the development team:

- Ziqura Thomas
- Amya Overton
- Anthony Munson
- Tyler Young



















**2-2 Project Log: Team Formation and Project Design**

After reviewing the project scenarios outlined in the Final Project Guidelines and Rubric, the team selected the third person scenario set as a survival horror shooter within a cathedral environment. Based on this scenario, the following four additional gameplay elements were chosen for inclusion in the project:
- Power-up pickups
- Player equipment pickups
- Moving enemies
- Stationary obstacles

**Brainstormed Content Based on the Scenario**\
The game is designed as a third-person survival horror experience set in an archaic cathedral. The player begins in the catacombs and progresses through dangerous areas while attempting to escape the cathedral. The narrative centers on a time-travel mission where the player is sent from the future to stop a threat contained within the cathedral. Previous agents failed, leaving behind barriers and equipment for the player to use.

Gameplay content includes modern weapons and equipment (firearms & armor) contrasted against an ancient cathedral setting, enemy cultists guarding the area, and environmental traps. Armor plates, health items, ammunition, and temporary buffs such as adrenaline shots support the survival horror gameplay.

Power Pickups
- Consumable health item (quick use): Restores health upon use
- Ammo pickups: Ammunition for weapons
- Battery: Used for flashlight power
- Adrenaline shot: Temporarily increases player speed

Player Equipment
Armor Pickups
Armor plate system will be displayed as a bar above the health bar in 4 distinct chunks:
- Small armor plate: Restores 1 armor
- Medium armor plate: Restores 2 armor
- Large armor plate: Restores all 4 armor

Weapon Pickups
- Knife
- Pistol
- Shotgun
- Stretch Goal: Grenade

Enemy Types (Moving)
Enemies will comprise of the cathedrals cultists, being melee focused only.\
- Quicker: Fast movement, lower damage
- Tank: Slow movement, high damage

Obstacles (Stationary)
- Bear trap: Renders the player immobile and causes damage
- Saw trap: Deals damage and causes bleeding
- Pitfalls: Instant kill
- Barriers: Prevent progression and require key objects to continue

**Development Schedule and Timeline**\
The project development timeline follows the course structure and milestone deadlines:

- Weeks 1–4: Alpha development phase
- Week 5: Beta development phase
- Weeks 6–7: Polishing, bug fixing, and final submission preparation

This timeline ensures that core systems are implemented early and refined before final submission.

**Alpha and Beta Development Goals**\
Alpha Stage Goals (Completed by Week 4):
The Alpha stage focuses on establishing core gameplay systems and basic functionality. By the Alpha submission, the following elements should be in place:
- Basic player movement and combat functionality
- Enemy movement with simple AI behaviors (attacking)
- Functional stationary obstacles (traps)
- Player equipment pickups (weapons and armor)
- Power-up pickups with basic effects

Beta Stage Goals (Completed by Week 5):
The Beta stage focuses on refinement, content expansion, and level design. By the Beta submission, the following goals should be met:
- Fully designed level layout, with each team member contributing one room, with the fifth and final room being a larger collaborative effort
- Final enemy and obstacle placement
- Improved combat and interaction responsiveness
- Clear progression from start to end location

**Communication Methods & Communication Frequency**\
The team will use Discord as the primary communication platform. Discord voice channels will be used for meetings and live discussions, while text channels will serve as a persistent communication hub for updates, questions, and coordination between meetings. The team will hold a minimum of two check-ins per week. Tuesdays are designated as a consistent meeting day to ensure regular progress updates and alignment. Additional meetings may be scheduled as needed based on development requirements.

**Task Assignment and Reporting**\
All project tasks will be tracked using Trello. All team members are expected to report all in-progress and completed tasks using the dedicated card categories.  

All content was collaboratively developed by all members of the development team:

- Ziqura Thomas
- Amya Overton
- Anthony Munson
- Tyler Young
