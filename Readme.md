NBADrafts
=========
This service provides information on the NBA draft starting from its inception in 1947. NBA drafts occur once every year, and consist of multiple rounds where players are drafted by professional basketball teams. 
Each draft provides details on the number of selections in that round, and each selection provides details about the player picked. 
Data is organized by drafts and selections. Users will be able to search through drafts based on years or selections.

ID Attribute Values
-------------------
1. drafts - applied to a DIV tag, includes a list of all of the drafts present in the representation. May contain only one draft. 
2. selections - applied to a DIV tag, includes a list of all of the draft selections present in the presentation. May contain only one selection. 
3. search - applied to a DIV tag, includes a form for query links. May contain only one form.
4. create - applied to a DIV tag, includes a form for update links. May contain only one form. 
    
Class Attribute Values 
----------------------
1. all - applied to a UL,OL tag. A list of representations. When this tag is a descendant of a  DIV.id="drafts" it may have  one or more LI.class="year" descendant elements.  When this tag is a descendant of a  DID.id="selections" it MUST have one or more SPAN.class="year" descendant elements and it may have one or more LI.class="selection" elements. 
2. description - applied to a SPAN tag. Contains a summary description of a selection. 
3. details - applied to a SPAN tag. Contains a brief description of a selection.
4. draft-add - applied to a FORM tag. A template to add the next draft. The element MUST be set to FORM.method="post" and SHOULD contain the following descendant elements: INPUT[text].name="password".
5. draft-search - applied to a FORM tag. A template to search draft years and selections. The element MUST be set to FORM.method="get" and SHOULD contain the descendant element INPUT[text].name="year" or INPUT[text].name="selection".
6. multiple - applied to a UL tag. A list representation. When this tag is a descendant of a DIV.id="drafts" it may have one or more LI.class="year" descendant elements.
7. selection - applied to a LI, SPAN tag. Contains the selection of a draft. When this element is a descendant of DIV.id="selections" then it MUST contain the descendent element SPAN.class="description".
8. selections - applied to  a DIV tag, includes a list of all of the draft selections based on a query. May contain only one selection or all selections from a year.
9. selection-add - applied to a FORM tag. A template to add a draft selection. The element MUST be set to FORM.method="post" and SHOULD contain the descendant elements: INPUT[text].name="selection" and INPUT[text].name="details" and INPUT[text].name="description" and INPUT[text].name="password".
10. selection-remove - applied to a FORM tag. A template to remove a draft selection. The element MUST be set to FORM.method="post" and SHOULD contain the descendant elements: INPUT[text].name="selection" and INPUT[text].name="password".
11. selection-update - applied to a FORM tag. A template to update a draft selection. The element MUST be set to FORM.method="post" and SHOULD contain the descendant elements: INPUT[text].name="selection" and INPUT[text].name="details" and INPUT[text].name="description" and INPUT[text].name="password".
12. single - applied to a UL tag. A list representation. When this tag is a descendant of DIV.id="drafts" it MUST have one SPAN.class="year" descendant element and may	have one DIV.class="selections" descendant element. When this tag is a decendant of DIV.id="selections" it MUST contain a LI.class="selection" element. 
13. year - applied to a LI, SPAN tag. Contains the year of a draft. When this element is a descendant of Div.id="drafts" then it MUST contain the descendent element A.rel="draft". 

selection_search
round
pick
nav
team
name 
number
player
position
instructions
	
Name Attibute Values
--------------------
1. description - applied to an INPUT[text] element. The team name, player name, position, etc of a selection. 
2. details - applied to an INPUT[text] element. The team name and player name of a selection.
3. password - applied to an INPUT[text] element. The password to allow for creation, update and removal of selections.
4. selection - applied to an INPUT[text] element. The selection/position of the draft. The selection value to use when creating a draft position using FORM.class="selection-add". The selection value to use when removing a draft position using FORM.class="selection-remove".The selection value to use when updating a draft position using FORM.class="selection-update". The search value to use when searching draft selection using FORM.class="draft-search".
5. year-end - applied to an INPUT[text] element. The year of the last desired draft. A search value to use when searching draft values using FORM.class="draft-search".
6. year-start - applied to an INPUT[text] element. The year of the first desired draft. A search value to use when searching draft values using FORM.class="draft-search".

	
Rel Attribute Values
--------------------
1. draft - applied to an A tag, a reference to a draft year. 
2. selection - applied to an A tag, a reference to a draft selection.
