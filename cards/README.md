
# cards.json

Cards is an unordered JSON array of cards released for Disney's Lorcana TCG game. Cards file contains array of card objects.

##  card object

The following attributes are available for a card object:

| atribute | type | optional | description |
|--|--|--|--|
| id | string || UUID (v4) - Unique identifier(s) of the card |
| cardName | string | | Name of the card - concated name and version of the card delimited by '-' character |
| name | string || Name of the card |
| version | string | yes | Version of the card |
| ink | enum | | Ink color of the card: "amber", "amethyst", "emerald", "ruby", "sapphire", "steel"  |
| type | enum | | Type of the card: "character", "item", "action" |
| subTypes | string[] | yes | Sub-types of the card |
| text | string | yes | Abilities and effects on the card (unformatted) |
| mdText | string | yes | Abilities and effects on the cards (markdown formatted) |
| flavour | string | yes | Flavour text |
| cost | string | | Cost of the card |
| inkwell | boolean | | Can the card be used in inkwell |
| strength | string | yes | Strength of the card |
| willpower | string | yes | Willpower of the card |
| lore | string | yes | Lore the card can generate |
| artist | string | | Artist identifier (usually name and surname) |
