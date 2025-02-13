### Cold Steps

### Overview
Cold Steps is a puzzle level of the video game _Baba is You_ , created with the game level editor uploaded
on [Itch.io](https://hempuli.itch.io/baba-is-you-level-editor-beta). The following sections explain the process of creating the level from the first initial
concept to its latest version.

#### First Approach
After playing several levels of Baba is You, there were two mechanics that stood out to me.
The first was the fact that in some levels, the player could take control of the walls of the
level, which provided a feeling of power by suddenly gaining agency over a large area of the
level. The other mechanic was based on the **MAKE** property, which allowed the player to
generate an element every time they took a step.  
This mechanic reminded me of the puzzles of the video game The Legend Of Zelda: Tears
of the Kingdom, in which the puzzles provide you with different pieces and materials
separately and it is the player who must put them together to create himself the tools that will
allow him to solve the puzzle.
  
So I decided that in my level the player had to create different elements with the **MAKE**
property and then use them to solve the puzzle.
  
#### Initial Concept
The first idea of the level that I thought of, taking advantage of the **MAKE** property, was that
the player had to create a large version of Baba and then take control of it and with it solve
the puzzle.
  
_Original_ _concept_
There were three materials that worked well when creating large masses of elements, not
only because when different pieces were put together they formed a single piece, but it also
made logical sense taking into account the material used.
The materials were:

**CLOUD**,

![Cloud](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_cloud.png)

**ICE**,

![Ice](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_ice.png)

and **BLOB**.

![Blob](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_blob.png)
  
The material that worked best was **BLOB**, as it created an interesting result and it made
more sense that Baba could leave a trail of slime than clouds. However, the final material
was **ICE** as I thought it would be more fun if the player could create ice by walking on water
and it was a good hook that differentiated my level from the rest.

The idea was to use the large body created to move blocks of **TEXT** at the same time, or
adopt different shapes to fit into gaps and move text in ways that could not be done with
Baba.  
But this idea was discarded due to its complexity and I established that the way to beat the
level would not be to control the mass of ice created, but to use it to overcome the puzzle.
  
#### First Attempt

![First Attempt](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_first_attempt.png)

In the first attempt to make the level I had two rules clear that would remain intact throughout
development. The first was that the way to win was to touch the flag (**FLAG IS WIN**), since it
was a clear and easy to see objective. The second was the mechanic of Baba creating ice
when stepping on water (**BABA ON WATER MAKE ICE**), since this was the hook of the
level.
  
However, I couldn't use these mechanics in a way that they were not too easy to solve or
didn't break the level and then I realized that I was building the level before establishing the
puzzle to resolve.

#### Second Attempt

![Second Attempt](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_second_attempt.png)

On the second attempt at making the level I focused not only on using the mechanics of
using the **FLAG** to win and **BABA ON WATER MAKE ICE**, but also on playing with these
rules so that the player altered them to solve the puzzle, since the fact that changing the
rules was what made Baba is You special, and I wasn't taking advantage of it.
I started messing around with the **TEXT**s of the game to create the puzzle, however I ran
into three problems during the development.
  
The first was that it was creating the level in chunks, so the player had to solve several
mini-puzzles to reach the flag. This mechanic was not bad itself as long as the mini-puzzles
served to solve a larger puzzle, but I realized that I was doing them separately and
disconnected from each other, so I did not like this approach.
  
The second problem was that again, altering some rules made creating the puzzle very
complicated, since it completely broke the level.
And the last problem came as a result of the second, since I realized that some mechanics
should not be altered (such as the case of the level hook, **BABA ON WATER MAKE ICE**).
So for the next attempt I focused on finding first all the mechanics that the level would use
and then separating them into alterable and unalterable to make the puzzle.
  
#### First Iteration of the Level

![First Iteration](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_first_iteration.png)

The first version required the player to remove the **SINK** property of **WATER** and **ICE** in
order to freeze the water and use the ice to push the **FLAG** off the **SKULL** group and win.
However, I found at least five problems in the level, two due to design errors and three
through the playtesting done in class.
  
The first two design errors had to do with the word **WATER**, because, one, I realized that
having **WATER AND ICE IS SINK** as the first rule directly avoided the use of the main hook
of the level **BABA ON WATER MAKE ICE**, and two, the level could be solved by pushing
water instead of ice and the player would never see the hook mechanic.
On the other hand, thanks to playtesting I discovered three other problems.
  
The first problem was that with the **FLAG SINKS IN THE WATER** rule, the flag eliminated
the player when he touched it. This was because I wanted the players to create an ice
platform to save the flag from the lake, due to the **FLAG ON ICE IS SAFE** rule, as I wanted
the player to use the ice created to solve the puzzle no matter what, however, the **FLAG** that
had the **SINK** property eliminated the player on contact unless the flag was moved off the
surface of the water.
The second problem was due to players modifying the **FLAG IS PUSH** rule to create more
flags since there were no repercussions for altering this rule.
And the last problem, which I discovered thanks to the feedback of a classmate, was that the
rules to be modified were very easy to access, and it was very easy to change them.
  
#### Second Iteration of the Level

![Second Iteration](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_second_iteration.png)

For the second version I focused on correcting the problems from the previous version.
First I shrunk the size of the level vertically and enlarged the lake so that the player would
cross over it and try the **BABA ON WATER MAKE ICE** mechanic no matter what.
  
Second, I got rid of the **WATER AND ICE IS SINK** rule and the WATER AND ICE IS SAFE
rule, which prevented ice and water from eliminating each other, but without **WATER AND
ICE IS SINK** it was no longer necessary.
  
Third, I changed the **FLAG ON WATER IS SINK** rule to **WATER EAT FLAG**, which kept the
flag safe as long as it was on ice, but no longer eliminated the player on touch.
Also, I changed the **FLAG IS PUSH** rule, since I didn't like giving away part of the solution,
and replaced it with the **FLAG ON ICE IS SAFE** rule, which solved the problem of people
altering the **FLAG IS PUSH** rule without repercussions.
  
Finally I put the rules inside the lake, not only to encourage the player to step into the water,
but also to complicate access, since now the ice prevented the player from retracing their
steps with the **ICE IS STOP** rule.
Besides I added a new material called **CRYSTAL** as an excuse to add AND and allow the
player to create the **ICE AND FLAG IS PUSH** rule, which would allow them to win. I chose
**CRYSTAL** specifically because it looked like ice fragments, especially when its color is
changed to light blue.
  
Now the catch of the level is that the player had to use the words **ICE**, **AND**, **IS** and **PUSH** to
create the **ICE AND FLAG IS PUSH** rule or similars but it can not mess the **FLAG ON ICE IS SAFE** rule.
  
#### Modifications
I wanted the player to think first about using ice instead of crystals, so I tried adding the
**CRYSTAL IS DEFEAT** rule to draw the player's attention away from the crystals, which only
worked if the **CRYSTAL IS STOP AND PUSH** rule was modified.

![Modification 1](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_modification_1.png)

However, this did not greatly affect the gameplay and was more of an annoyance than a
feature. Therefore, I left the rules as they were, modified some colors to make the level more
aesthetic, and added clouds as decoration since they looked like snow.

![Modification 2](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_modification_2.png)

However, at this point I realized that **AND** was not really necessary if I placed the texts like a
crossword puzzle.

_Example:_

![Crossword](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_crossword.png)

So I changed the **CRYSTAL IS STOP AND PUSH** rule to **CRYSTAL IS PUSH**, and I put the
**ICE IS STOP** together with the **FLAG ON ICE IS SAFE** rule in the form of a crossword
puzzle to give the player a clue on how to solve the puzzle.

![Modification 3](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_modification_3.png)

With this change, the **ICE IS STOP** rule became more relevant, not only because it taught
the player that he could take advantage of texts from a column rule to create a row rule, but
now it was much further away from the player, which made it the mechanic of the player not
being able to retrace his steps inevitably lasted longer.
  
However, now the crystals took more leadership than the ice to move the flag, but I decided
not to interfere anymore since at this point the level design was more aimed at using the
crystals.
  
#### Final Iteration of the Level

![Final Iteration](https://github.com/MiguelRodriguezTorrente/Portfolio/main/assets/images/cold_steps/cold_steps_final_iteration.png)

Finally, I decided to recover the **AND** and add the **FLOAT** property so that the player would
have more options to choose from, and thus, make the level a little more difficult.
With this, not only did increase the possibility of using **ICE** to obtain the flag, but by not
having **CRYSTAL IS PUSH**, which I did not like since it gave part of the solution to the
puzzle, and changing it to **CRYSTAL IS FLOAT AND PUSH**, the player would have to make
the decision whether to use the **FLOAT** or not, which makes it a little more difficult to find the
solution to the puzzle.
  
I decided to use **FLOAT** instead of another **STOP** since **STOP** with a **PUSH** did not work
and with a **FLOAT** it gives the sensation that the crystals are floating in the lake.

Before finishing, there are several solutions to this puzzle, which are mainly divided into
three.
  
The first is to solve the puzzle as planned, which is to use the **PUSH** property and different
materials, such as **ICE**, **CRYSTAL** or **TEXT** itself to get the **FLAG** out of the **SKULL** group.
  
The second solution is to take one **CRYSTAL** out of the water and turn it into a **FLAG**. It
must be taken out of the water to prevent the destruction of the **FLAG** with the **WATER EAT
FLAG** rule.
  
The last solution is to modify the **FLAG ON ICE IS SAFE** rule, shortening it to **FLAG IS
SAFE**, causing the water to not destroy the **FLAG** in any case, and converting other
elements such as **ICE** or **CRYSTAL** into flags.
  
Last but not least, the level can be played with the code **8PRF-ZC2B**.
