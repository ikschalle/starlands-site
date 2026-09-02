# ALL ABOUT CHARACTER PAGES!!

This will detail the character system and how to make character pages.

This is a 2 step process: info entry + assigning images.

### CHARACTER INFO

A page is created for each `.md` file in `/_characters/` based on the content within, so naturally make a new file if you want a new character.

This information may also be used across pages and for other automations (read the liquid template lang docs for details).
The properties can be in any order as long as theyre formatted correctly but this prescribed order is preferred.

!!File name should be hyphenated and should only have a first and last name for brevity. SHOULD NOT HAVE ACCENTS OR SPECIAL CHARACTERS!!

!!!INDENTATION IS IMPORTANT AND IMPROPER INDENTATION WILL EXPLODE EVERYTHING; YOU MUST ALSO HAVE A SPACE AFTER THE COLON!!!

The following is the Front Matter for all `.md` files located at `/_characters/`

```Markdown
--- 
title: # (string, set only if you want to override the title generated from the file name, e.g. if you have nicknames or middle names or accents) 
gender: # (string)
pronouns: # (string)
profession: # (string)
artfight-id: # (int)

affiliation: # currently doesn't do anything and might become obsolete depending on future implementation lol
	org-slug: # (rank/position/title if applicable, string) 

tags:
  - thing 1 # (string)

skills:
  thing1: # (int, 0-5)

relationships:
  slug-kebab:
	  type: # (string)
    description: # (string)
---

MARKDOWN, HTML, AND LIQUID HERE
```

Refer to other character files if you are stuck, dont worry about making mistakes they can always be amended!

### CHARACTER IMGS

> `slug` is a variable derived from the name of the page/`.md` file and is used as the unique reference/id for the character.
e.g. `ace-nightwing.md` has the slug `ace-nightwing`

Character images should be stored at `{{site.baseurl}}/assets/img/{{character.slug}}/`. Make a new folder when you make a new character page, matching the name of the page.

Portraits:
- Should be named `portrait.png` with a `.png` extension duh
- These are rendered at a 9:16 aspect ratio (quite tall), cropping very wide images may be more aesthetic

Thumbnails:
- Should be named `thumb.png` with a `.png` extension duh
- These are rendered at a 1:1 aspect ratio (perfect square), we insist cropping be mandatory for this as they are supposed to be bust shots anyway
	
And yeah you're done!
