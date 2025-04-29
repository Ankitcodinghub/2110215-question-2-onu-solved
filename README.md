# 2110215-question-2-onu-solved
**TO GET THIS SOLUTION VISIT:** [2110215 Question 2-ONU Solved](https://www.ankitcodinghub.com/product/2110215-question-2-40-minutes-10-40-11-20-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;109260&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;2110215 Question 2-ONU Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
1. Instruction

1) Create Java Project named “2110215_Midterm_Q2”.

2) Copy all folders in “Q2.zip” to your project directory src folder.

3) You are to implement the following classes (detail for each class is given in section 3 and 4)

a) BaseCard (package logic.card)

b) NumberCard (package logic.card)

c) DrawTwoCard (package logic.card)

d) GameLogicUtility (package logic.utility)

4) Make UML class diagram for classes in package logic, using ObjectAid or another UML generator program. Save its picture file in your logic.card folder.

5) JUnit for testing is in package test.

6) To submit:

6.1. go to src folder that you actually do the coding for this question.

6.2. Zip this question’s src folder. Name it YOUR-ID_Q2.zip (for example, 6332112121_Q2.zip)

6.3. Submit the zipped file as an assignment on MyCourseville.

2. Problem Statement: ONU

Figure 1 ONU Game logo

We create UNO-liked puzzle game called ONU. The basic rule is very similar to UNO, but ONU is a single player game. ONU’s win condition is that player has to empty his/her hand before the deck is out.

In every turn, the player has to play 1 card from his/her hand by discarding it to the discard pile. However, each card type can only be played if certain condition(s) is satisfied. There are 2 types of cards in ONU.

• a “number” card which has a number and a color on it. A number card can be played when it has the same color or same number as the top card of the discard pile. There are number 1 to number 4 cards for each color, RED, BLUE, YELLOW, and GREEN (16 in totals) in the deck.

• The second type is a “draw-two” card which has a draw-symbol and color on them. A player who plays a draw-two card has to draw 2 cards from the deck (there is only one player in our game anyway). A draw-two card can only be played when it has the same color as the top card on the discard pile. There are 4 “draw-two” cards in the deck, one for each color.

The game will end when the player’s hand is out of cards or the deck is out of cards.

4. Implementation Detail

The class package is summarized below.

* In the following class description, only details of IMPORTANT fields and methods

are given. *

4.1 Package logic.card /* You must implement this package from scratch*/

4.1.1 class BaseCard /* You must implement this class from scratch*/

This class is a base class for all kind of Cards. It contains all common elements which a card should have.

Field

Name Description

– CardColor color Color of the card. CardColor is enum in the package logic.game.

– CardSymbol symbol Symbol of the card. CardSymbol is enum in the package logic.game.

Method

Name Description

+ BaseCard(CardColor color) This is the Constructor.

Set color as one given in the parameter.

+ void play() This method is called when the card is played. The results of actions are different for each type of Cards.

+ boolean ruleCheck() This method returns true if the card can be played according to the rule and returns false when the card is illegal to play. The rules are different for each type of Cards.

+ getter-setter for all fields.

4.1.2. class NumberCard /* You must implement this class from scratch*/

This class is a type of Card. The top card of the discard pile must have same color or the same symbol to make this card playable. Playing a number card will change the top card of the discard pile to this card but no special effect happens.

Method

Name Description

+ NumberCard(CardColor color, CardSymbol symbol) This is the Constructor.

Set the information of the super class.

Set symbol as one given in the parameter.

+ void play() Use method setTopCard in class GameLogic to set this card to the top of the discard pile.

You can call the method by using

GameLogic.getInstance().setTopCard(…..).

*You do not need to check for play legality.

+ boolean ruleCheck() return true if the top card of the discard pile has the same color or same symbol as this card. Otherwise, return false. You can use GameLogic.getInstance().getTopCard() to get the top card of the discard pile.

4.1.3. class DrawTwoCard/* You must implement this class from scratch */

This class is a type of Card. The top card of the discard pile must have same color to make this card playable. Playing draw-two card will change the top card of the discard pile to this card and the player has to draw 2 cards from the deck.

Method

Name Description

+ DrawTwoCard(CardColor color) This is the Constructor.

Set the information of the super class.

Set symbol as CardSymbol.DRAW.

+ void play() Use method setTopCard in class GameLogic to set this card to the top of the discard pile.

Then, use method draw in class GameLogic to draw 2 cards by setting the parameter of the method as 2.

You can call the methods by using

GameLogic.getInstance().setTopCard(…..). and

GameLogic.getInstance().draw(…..)

*You do not need to check for play legality.

+ boolean ruleCheck() return true if the top card of the discard pile has the same color as this card. Otherwise, return false.

You can use GameLogic.getInstance().getTopCard() to get the top card of the discard pile.

4.2 Package logic.game

4.2.1. class GameLogic /*ALREADY PROVIDED*/

This class is the main game system. This class provides cards in deck, hand and game rules.

The game will be run via this class.

4.2.2. enum CardColor /*ALREADY PROVIDED*/

This enum contains values of color in this game.

4.2.3. enum CardSymbol /*ALREADY PROVIDED*/

This enum contains values of symbol on the cards.

4.3 Package logic.utility /* You must implement this package from scratch*/

4.3.1 class GameLogicUtility /* You must implement this class from scratch */

This class contains a method which will be used in GameLogic. Note: This is not the proper design of classes structure but it is required for scoring.

Method

Name Description

+ boolean drawRule() This method checks all cards in ArrayList&lt;BaseCard&gt; hand from

GameLogic as follows

• Return false, if there is any legal card to play in hand.

• Return true, if there is no legal card in hand. You can get the hand of the player by using GameLogic.getInstance().getHand().

4.4 Package main

4.4.1 class Main /*ALREADY PROVIDED*/

This class is the main program. You don’t have to implement anything in this class. You can test the program by running this class.

4.5 Package test.grader /*ALREADY PROVIDED*/

This package provides JUnit test for each of your class.

5. Finished Code Run Example

5.1. Start the game

5.2. Game play

5.3. Play number card

5.4. Play draw-two card

5.5. Draw a card by rule

5.6. Play illegal card

5.7. Input index out of bounds

5.8. Win the game (empty the hand)

5.10. Lose the game (empty the deck)

6. Score Criteria

The maximum score for the problem is 15 and will be rounded down to 5.

6.1 Implement Class BaseCard, which does not have complete functions, correctly = 3 points

6.2 Class NumberCard: = 3.5 points

testConstructor = 1 points

testPlay = 1 points

testRuleCheck = 1.5 points

6.3 Class DrawTwoCard: = 3.5 points

testConstructor = 1 points

testPlay = 1.5 points

testRuleCheck = 1 points

6.4 Class GameLogicUtility: = 3 points

testRuleCheck = 3 points

6.5 UML = 2 points

All classes in package logic are present (correct variables and methods) = 1 points

Inheritance and Abstract structures are correct = 1 points
