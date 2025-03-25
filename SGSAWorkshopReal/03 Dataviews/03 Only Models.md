Displays all papers with non-null `Model`  field

```dataview
TABLE
title as Title, 
FirstAuthor as "First Author", 
Year as Year,
itemType as Item, 
Citekey as Citekey, 
Contribution_General as Contribution,
Contribution_Mine as "My Importance"
FROM "meta/Papers"
WHERE Model != null
```