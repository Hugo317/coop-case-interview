##### START #####
Please see attached excel for column names, example value, and short description.
A bit more details follows below:



##### REPLACED VALUES DUE TO GDPR #####
Columns:
- itemId
- customerId
- householdId
- receiptId
have been replaced with integer values 1 -> however many unique records exist in the dataset.



##### ITEM NAMES ARE NOT INCLUDED #####
Item EAN and Name cannot be displayed for GDPR reasons.
However, the categories and the segments that items belong to, can.
Below follows a hierarchical overview example:

ItemCategoryAreaID      11
ItemCategoryGroupID     423206
ItemCategoryTeamID      423330
ItemCategoryID          249
ItemSubCategoryID       12
ItemSegmentID           3
ItemSubSegmentID        2
ItemID                  7300156583413

ItemCategoryAreaName    Food
ItemCategoryGroupName   NEARFOOD
ItemCategoryTeamName    DRYCKER
ItemCategoryName        LÄSK&SAFT
ItemSubCategoryName     LÄSK DRICKA NU
ItemSegmentName         APELSIN
ItemSubSegmentName      MINDRE ÄN 45 CL
ItemName                FANTA  (NOTE: You do not have the ItemName in you dataset)

----- Tip -----
Use the following hierarchy to get a good overview on what Item you are working with:
ItemCategoryArea<Name/ID>
ItemCategoryGroup<Name/ID>
ItemCategoryTeam<Name/ID>
ItemCategory<Name/ID>
ItemSubCategory<Name/ID>

Result of tip as the above example would yield:
ItemCategoryAreaName    Food
ItemCategoryGroupName   NEARFOOD
ItemCategoryTeamName    DRYCKER
ItemCategoryName        LÄSK&SAFT
ItemSubCategoryName     LÄSK DRICKA NU

You can also create your own unique item names by concatenating one or more of the selected columns.
Since you do not have "Fanta" in you dataset, you could for example concatenate:
ItemCategoryName + _ + ItemSegmentName  -> LÄSK&SAFT_APELSIN

##### ./END #####
