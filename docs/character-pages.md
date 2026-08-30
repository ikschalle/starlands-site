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
name: # (string) 
gender: # (string)
pronouns: # (string)
profession: # (string)
artfight-id: # (int)

affiliation: # currently doesn't do anything and might become obsolete depending on future implementation lol
	org-uid: # (rank/position/title if applicable, string) 

tags:
  - thing 1 # (string)

skills:
  thing1: # (int, 0-5)

relationships:
  uid-kebab:
	  type: # (string)
    description: # (string)
--- END OF FRONT MATTER

MARKDOWN, HTML, AND LIQUID HERE
```

Refer to other character files if you are stuck, dont worry about making mistakes they can always be amended!
