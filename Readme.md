NBADrafts
=========
This service provides information on the NBA draft. 
NBA drafts occur once every year, and consist of multiple rounds where players are drafted by professional basketball teams. 
Each draft provides details on the number of selections in that round, and each selection provides details about the player picked. 
Data is organized by drafts and selections. Users will be able to search through drafts based on years or selections.
For the purposes of this assignment, in order to reduce the number of data to be entered only a small proportion of all drafts and selection were included; the functionality of the database is still maintained however. 

ID Attribute Values
-------------------
1. drafts - applied to a DIV tag, includes a list of all of the drafts present in the representation. May contain only one draft. 
1. selections - applied to a DIV tag, includes a list of all of the draft selections present in the presentation. May contain only one selection. 
1. search - applied to a DIV tag, includes a form for query links. May contain only one form.
1. create - applied to a DIV tag, includes a form for update links. May contain only one form.
1. delete - applied to a DIV tag, includes a form for delete links. May contain only one form. 
    
Class Attribute Values 
----------------------
1. all - applied to a UL,OL tag. A list of representations. When this tag is a descendant of a  DIV.id="drafts" it may have  one or more LI.class="year" descendant elements.  When this tag is a descendant of a  DID.id="selections" it MUST have one or more SPAN.class="year" descendant elements and it may have one or more LI.class="selection" elements. 
1. description - applied to a SPAN tag. Contains a summary description of a selection. 
1. draft-add - applied to a FORM tag. A template to add the next draft. The element MUST be set to FORM.method="post" and SHOULD contain the following descendant elements: INPUT[text].name="pass".
1. info - applied to a SPAN tag. Contains details on the data to be included in a form. 
1. instructions - applied to a DIV tag, includes information on how to use a form. 
1. multiple - applied to a UL tag. A list representation. When this tag is a descendant of a DIV.id="drafts" it may have one or more LI.class="year" descendant elements.
1. nav - applied to a DIV tag, includes links to different representations. 
1. player - applied to a SPAN, DT tag. Contains the name of the selection that was chosen.
1. pick - applied to a SPAN, DT tag. Contains the pick order in which a selection was chosen.
1. position - applied to a SPAN, DT tag. Contains the playing position of a selection.
1. round - applied to a SPAN, DT tag. Contains the round in which a selection was chosen.
1. selection - applied to a LI, SPAN tag. Contains the selection of a draft. When this element is a descendant of DIV.id="selections" then it MUST contain the descendent element SPAN.class="description".
1. selections - applied to  a DIV tag, includes a list of all of the draft selections based on a query. May contain only one selection or all selections from a year.
1. selection_add - applied to a FORM tag. A template to add a draft selection. The element MUST be set to FORM.method="post" and SHOULD contain the descendant elements: INPUT[text].name="draft" and INPUT[text].name="year" and INPUT[text].name="id" and INPUT[text].name="name" and INPUT[text].name="number" and INPUT[text].name="team" and INPUT[text].name="player" and INPUT[text].name="position".
1. selection_delete - applied to a FORM tag. A template to remove a draft selection. The element MUST be set to FORM.method="post" and SHOULD contain the descendant elements: INPUT[text].name="rev" and INPUT[text].name="id" and INPUT[text].name="password".
1. selection_search - applied to a FORM tag. A template to search amongst draft selections. The element MUST be set to FORM.method="get" and SHOULD contain the descendant elements: INPUT[text].name="name".
1. selection_update - applied to a FORM tag. A template to update a draft selection. The element MUST be set to FORM.method="post" and SHOULD contain the descendant elements: INPUT[text].name="draft" and INPUT[text].name="year" and INPUT[text].name="id" and INPUT[text].name="name" and INPUT[text].name="number" and INPUT[text].name="team" and INPUT[text].name="player" and INPUT[text].name="position".
1. single - applied to a DL,UL tag. A list representation. When this tag is a descendant of DIV.id="drafts" it MUST have one SPAN.class="year" descendant element and may have one DIV.class="selections" descendant element. When this tag is a decendant of DIV.id="selections" it may contain a LI.class="selection" element. 
1. team - applied to a SPAN, DT tag. Contains the team for which a selection was chosen.
1. year - applied to a LI, SPAN tag. Contains the year of a draft. When this element is a descendant of Div.id="drafts" then it MUST contain the descendent element A.rel="draft". 
    
Name Attibute Values
--------------------
1. description - applied to an INPUT[text] element. The team name, player name, position, etc of a selection. 
1. details - applied to an INPUT[text] element. The team name and player name of a selection.
1. name  - applied to an INPUT[text] element. The unique, overall identifier of a selection.
1. pass - applied to an INPUT[text] element. The password to allow for creation, update and removal of selections.
1. player  - applied to an INPUT[text] element. The name of a selection.
1. pick - applied to an INPUT[text] element. The pick number of a selection.
1. player  - applied to an INPUT[text] element. The selection's position.
1. number - applied to an INPUT[text] element. The round of a selection.
1. selection - applied to an INPUT[text] element. The selection/position of the draft. The selection value to use when creating a draft position using FORM.class="selection-add". The selection value to use when removing a draft position using FORM.class="selection-remove".The selection value to use when updating a draft position using FORM.class="selection-update". The search value to use when searching draft selection using FORM.class="draft-search".
1. team - applied to an INPUT[text] element. The team of a selection.
1. year-end - applied to an INPUT[text] element. The year of the last desired draft. A search value to use when searching draft values using FORM.class="draft-search".
1. year-start - applied to an INPUT[text] element. The year of the first desired draft. A search value to use when searching draft values using FORM.class="draft-search".

	
Rel Attribute Values
--------------------
1. all_drafts - applied to an A tag, a reference to all draft years.
1. all_selections - applied to an A tag, a reference to all selections.
1. draft_year - applied to an A tag, a reference to a single draft. 
1. home - applied to an A tag, a reference to the main database navigation page. 
1. selection_info - applied to an A tag, a reference to a single selection.

