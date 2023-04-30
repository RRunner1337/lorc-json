
# sets.json

Sets is an unordered JSON array of sets released for Disney's Lorcana TCG game. Sets file contains array of set objects.

##  set object

The following attributes are available for a set object:

| atribute | type | optional | description |
|--|--|--|--|
| id | string || UUID (v4) - Unique identifier(s) of the set |
| name | string || Name of the set |
| release | date || Set release date |
| code | string || Set code |
| noOfCards | number || Number of cards released in a set |
| cards | setCard[] || Array of set card objects released in set |

## setCard object

The following attributes are available for card objects that are described in a set:

| atribute | type | optional | description |
|--|--|--|--|
| number | number || Consecurive number identifier of a card in the set. |
| cardId | string || UUID (v4) - Unique identifier(s) of the card that is represented in the set - relates to a card object in [cards.json](../cards/cards.json)|
| cardName | string || Name of the card |
| printingId | string || Printing identifier of the card |
| rarity | enum || Rarity of the card, one of: "promo", "common", "uncommon", "rare", "super-rare", "legendary" |
| finish | enum || Finish of the card, one of: "normal", "special-foil", "rainbow-foil" |
