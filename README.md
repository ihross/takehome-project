# jello
**J**ob tr**ELLO**

Students have trouble keeping track of work that needs to get done. We believe that giving them somewhere to track this will help them. We are going to start by replicating the trello workflow!

To get an introduction into what Trello is like, look here: https://www.youtube.com/watch?v=xky48zyL9iA

Our trello has humble beginnings we just want to keep track of the following tracks:
* Saved
* Applied
* Interviewing
* Offer

# Entities
For now, the two objects we want to keep track of are:
* Cards - hold information on what the user is keeping track of
* Lists - organizes a list of cards

# APIs
Our APIs are backed by a json-server db: https://github.com/typicode/json-server

The data which can be found in db.json

Cards has an API at:
/cards
/lists

The way to have this work is to run
`npm install`
and then
`npm run json-server`
You will then be greated by the following message.
![image](https://user-images.githubusercontent.com/607097/68042884-632c5380-fcaa-11e9-84a8-89d2742e48f4.png)

# Features to support
## Loading cards and lists and displaying them in columns like the following
![image](https://user-images.githubusercontent.com/607097/68040972-dd0e0e00-fca5-11e9-8b5d-3106d22847fe.png)

## Creating new cards under a list
When selecting "+ Add another card" at the bottom of a List, a text field appears that allows the user to type in a new entry.
* Pressing enter saves the card to the list or
* Clicking "Add Card" saves it
![image](https://user-images.githubusercontent.com/607097/68041130-43932c00-fca6-11e9-8a49-ea4812b0af8b.png)

The act of saving a card, opens another Textfield for continue adding of cards.

## Editing/Deleting card
When hovering over a card, there should be an option to edit it denoted with a pencil icon (or any icon):
![image](https://user-images.githubusercontent.com/607097/68041308-ad133a80-fca6-11e9-93b5-f7890f4c6fdf.png)

Clicking the icon changes the style by dimming everything and allowing a textfield with the content to be editted
![image](https://user-images.githubusercontent.com/607097/68041526-23b03800-fca7-11e9-9e9c-3b8e461a528e.png)

Clicking "Save"
* saves it
* archiving it, deletes it

## Moving cards between lists
When selecting a card "not on the edit button", the card is able to be dragged to another list. When being dragged there are a few states

**Recently grabbed, but not over any list**
There is a "ghost" placeholder on where the item was there before
![image](https://user-images.githubusercontent.com/607097/68041927-121b6000-fca8-11e9-9ffe-43a72eef9439.png)

**Recently grabbed, and over another list**
There is a "ghost" placeholder on where the item will be going
![image](https://user-images.githubusercontent.com/607097/68041996-35dea600-fca8-11e9-8fd6-78cf37c06427.png)

**Dropped onto the list**
![image](https://user-images.githubusercontent.com/607097/68042082-645c8100-fca8-11e9-8a3c-565fa951b33f.png)

# Extra things if you get to it
## Any way to move lists
Look at the trello demo if you are curious.

## Supporting images in the entry
Ditto.
