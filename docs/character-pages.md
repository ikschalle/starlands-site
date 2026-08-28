# ALL ABOUT CHARACTER PAGES!!

This will detail the character system and how to make character pages

### CHARACTER IMGS

Character images should be stored at `/assets/img/characters` with the filename uid.png (see uid in front matter template)
	These are rendered at a 9:16 aspect ratio (quite tall), cropping very wide images may be more aesthetic
Character thumbnails should be stored at `/assets/img/characters/thumb` with the filename uid.png
	These are rendered at a 1:1 aspect ratio (perfect square), we insist cropping be mandatory for this as they are supposed to be bust shots anyway

### CHARACTER INFO

The following is the Front Matter for all character.md files located at `/_characters/`
A page is created for each .md file in this directory based on the content within, so naturally make a new file if you want a new character
This information may also be used across pages and for other automations (read the liquid template lang docs for details)
the properties can be in any order as long as theyre formatted correctly but this prescribed order is preferred.
!!!INDENTATION IS IMPORTANT AND IMPROPER INDENTATION WILL EXPLODE EVERYTHING, YOU MUST HAVE A SPACE AFTER THE COLON!!!
and ofc delete all the comments they are just here to provide info on usage

```Markdown
--- 
layout: character -- DO NOT CHANGE
uid: (REQUIRED, kebab-string, middle and last name with no accents, should match file name)
name: (string) 
gender: (string)
pronouns: (string)
profession: (string)
affiliation: 
	org-uid: rank/title (string) 
	org-uid:
artfight-id: (int)

skills:
  thing1: (int, 0-5)

relationships:
  uid-kebab:
	type: homos (string)
    description: "blahblah" (string)
--- END OF FRONT MATTER

MARKDOWN, HTML, AND LIQUID HERE
```

Refer to other character files if you are stuck, dont worry about making mistakes they can always be amended!

Heres Seb's at the moment of writing:

```Markdown
---
layout: character
uid: sebastian-grunhaut
name: Sebastian Grünhaut
gender: Male
pronouns: He/They
profession: Railway Engineer
affiliation: 
  wulpin-rail-company: CEO
  stardoods-consortium:
artfight-id: 6406415

skills:
  Tinkering: 5
  Being Cold: 5
  Glibness: 4
  Marketing: 3
  Open-mindedness: 2
  Child Rearing: 1
  Philanthropy: 0

relationships:
  ace-nightwing:
    type: Friend?
    description: "In the unlikely event there is a catastrophic and completely unintentional accident which casts the flames of the law upon me, I would want this paragon of a lawyer to extinguish them."

  elene-sauvageau:
    type: Friend, probably.
    description: "Dearest Elene, We've had our moments of abrasion but I much prefer she to her predecessor. I'd like to avoid slighting her but has become something of habit."

  dotor-drep: 
    type: Friend
    description: "Curious fellow. One of my greatest customers despite no true agreement between us, though I wish he'd stop looking at me like that."

  venessa-sunset: 
    type: Frenenemy
    description: "Pristine at the surface, she had class; that I respect. But she was rotten. Rotted through all the way to marrow under that shadowy brim. Her soul, her business, her prices. All foul and odoriferous."

  allyn-asubaki:
    type: Daughter-for-tax-purposes
    description: "Young ones are universally unlearned but that is not my responsibility to amend, I am far too busy with affairs of actual importance."
---
## About
> "I have never done anything bad in my life. Ever."

Long a presence in the Starlands and the Consortium, Sebastian seeks to build railways to connect the world and does so for the great love of it.<br> 
Trains are all he has known and trains is all he commit to. Build, build, build. Rob you of your money so he can build. Beneath that prim dress and polite manner there is no concern for anything but trains. Or so one might think. Sebastian loves flowers! Did you know that? He should like to build gardens and sniff bouquets. Alas, his olfactory senses are redundant and his hands are bitingly cold. Indeed, he gives no warmth whatsoever. A plume of frost with every exhale. He is getting better at "caring" to some degree but it will take some time yet to thaw the permafrost at his core. He has been known to accidentally and intentionally murder people but running people over with trains is 100% never his fault. Some speak of a blaze powder habit but pay it no mind, its all just rumour, yes?
```
