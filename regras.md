##Numero de jogadores:
    2 a 6 
##Objetivo do jogo:
Podem existir diversos modos de jogo.
O padrao eh ser o jogador com o maior tesouro no fim de X turnos.

##Entidades do jogo:

* Cartas
    * Personagem
    * Aventura
    * Inimigo
    * Item
    * Rumor
* Dado (d10)
* Tabuleiro
    * Area central
    * Area do jogador
* Mao do jogador

##Organizacao do Tabuleiro:

### Area central
Onde a acao de fato ocorre.
A organizacao da area central depende da `fase do jogo`.(Ler secao *jogo*)
### Area do jogador
Tudo que estiver nesta area eh visivel a todos os jogadores.
    * contador de tesouro 
    * items nao equipados 
    * personagens e seus respectivos itens equipados
### Mao do jogador
O jogador pode revelar a mao (ou uma carta apenas)quando quiser, mas ela eh por default escondida.
    * rumores

## Jogo:

### Tesouro inicial:
    * 1 personagem ao acaso, nao importando requisitos
    * 1 item inicial ao acaso

O jogo se da em diversos turnos.
Cada turno tem 2 fases:
    * Cidade
    * Aventura

### Cidade

It begins with the spoils of the quests being given.
If it is the first turn, the initial items are given.
For each quest done:
If the players have not decided how to divide the spoils, a fair division is made: all items are sold to the market, for half of their value. And all the money is distributed based on the number of the alive characters assigned by each player to the mission. So if your character died during the mission, he lost his part.
If the division is not exact, the highest divisible number, smaller than the spoil is chosen and the rest is lost.
The players, in order of who has the most valuable treasure, receives each one his part of the spoils.
    treasure = money + sum of values of all items
Whenever there is a draw in treasure value, choose the order by agreement or dice roll.

After that:
N quests are revealled into the table, from the quest deck.
    N = number of players
M items are anounced as selling in the store.
    M = number of players + 2
V rumors are spread, face down.
    V = number of players
C new characters visit the town.
    C = number of players - 1


The players, in order of who has the most valuable treasure, can do one buy action each.
    buy action = trade money for a item or rumor or show a character that you meet his pre-requisites
This cycle is repeated until all cards are bought or everyone is not willing to buy more things.

Buy:

Item:
    When a item is bought, it is guarded in the clan's treasure room

Rumor:
    Rumors have a fixed price equals to half of the greatest treasure, round up.
Character:
    If a character does not have pre requisites a simple buy action can recruit him.

in all these cases, when a card is not picked, it is not thrown away.
It remains in the table until is consumed. So, less cards are drawn from the correspondent deck in the next city turn.

The exception for this is the character pile.
Each city phase the unpicked characters are putted back in the deck and the deck is shuffled.

Sell:
    A player can sell a item, a character or a rumor too.
    When selling an item or a rumor, the card is putted in the bottom of the item deck and it is shuffled.
    The item and the rumor are sold for half the price they would be bought.
    When a character is sold, all his equipped items are sold as consequence.
    You can just equip items before going to a mission, so you must plan ahead.

With the buys finished, the players assign their characters to the avaiable missions.
A quest can be assigned to as many characters as a player want.
And he may assign his characters to multiple quests.
But a character should not be assigned to more than one quest.

The spoils are going to be divided based on the number of characters each player assigned to the quest. It is like a pie chart.

In this part, items can be assigned to character's inventories.
A item cannot belong to more than one character inventory.
Remembering that just characters that fulfill the pre-requisites can equip the card.
    
When everyone is happy with their quests assignments and item placing, the quest phase begins.

### Aventura

For each assigned quest, in no particular order, the table is set:
    each player put in his front the assigned characters and their respective items.
    based on the level of the match, the monsters are drawn in the table:
    
    to place a monster:
        calculate the monster level:
            roll a d10
            divide by 2 de value rolled and round up
            get the integer part
                so 1 and 2 are 1, 3 and 4 are 2 ... 9 and 0 are 5
        then, a card of the corresponding monster level is drawn and putted on table, face up
        the enemy level is substracted from the quest level
    this is repeated until the the quest level is equals or below 0
    
    after the preparation is over, the revealed effects of the enemies are triggered, in the same order as the enemies were placed.
    each character, based on the character value order, from bigger to lower, can do an action.
    the value of a character is the sum of values of it's items.
    the monster's value is written in his card.
    If there is a draw between values, it should be resolved based on clans treasure.
Consider the enemies’ monsters treasure as infinite. 
    an action is using an item, attacking or using the character effect.
    to attack is to roll nd10 where n is the character attack power.
    An item can have type "equip" or "use". If it is a "use" type, it may be used just once per battle, turn it to indicate it has been used.
    When is a monster turn, he will activate any effect that has its conditions fulfilled and then he will attack his target, as described in his card.
for less life/most life target policy:
life = lesser value of total life - damage counters.

    The attack is just like the player's. the targeted player rolls the dices.
    If a character dies in combat, turn his card.
    
A quest is over when the objective is fulfilled or all the characters alive belongs to one player (or are all monsters).
    
When a quest is over, the dead characters remain dead and they will be for the rest of the game. They cannot be assigned for quests.
    Their items go to the clan's treasure.
    
    Spawned monsters:
They act as normal monsters but they attack the enemy monsters, based on their rules and their effects should be applied normally, but should change “other monsters” for “controller’s clan” and “character” for “enemy monster”. Remember: The player does not control the will of the monster. 
    
Quest types:

Kill all monsters:
    This includes the monsters spawned by the player.
Kill the strongest monster:
    The strongest monster may be one spawned by a player.
Survive:

Protect:    
    Spawn a character to be protected. At the end of the quest he will appear in town.


During any moment in the game, even if it is not his time to do an action, a player can activate a rumor.
    To do that, he puts the rumor on the table and roll a d10.
    




Cards:

Quest card:
    Objective.
    Level. int 1-10 (10 is higher)
    Spoils. set of items
Money:
    1, 5, 10, 50, 100
Item card:
    Value (50% to sell).
    Effect.
    Pre-requisite (character).
Rumor card:
    Rumor.
    Chance. set of different 0-10 indicating the dice that will activate the effect.
Character card:
    life.
    attack.
    Effect.
    Pre requisite (clan).
Monster:
    attack.
    life.
    value.
    target.
    reveal effects.
    condition effects.

