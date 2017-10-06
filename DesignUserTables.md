## Design the users tables ##

Assume that one user has one unique **UserID**, one **FamilyName** and more than one children. Therefore, we need to create a separate table for children.

**User_tbl** includes below attributes:

- UserID(**PK**)
- DateCreated
- FamilyName
- Email
- Address(Address will be in a separate table in the future as **State City Street**)
- Region

**Children_tbl** includes below attributes:

- ChildID (**PK**)
- UserID(**FK**)
- ChildFirstName
- ChildMiddleName
- ChildLastName
- Gender
- Age
- Birthday
- TopSize
- BottomSize
- Premium/Deluxe

**User_feedback_tbl** includes below attributes:

- FeedbackID(**PK**)
- ChildID(**FK**)
- ItemID(**FK**)
- FitRating
- StyleRating
- InWardrobePurchase(**Y/N**)
- AffilicatePurchase(**Y/N**)
- PurchasePrice

## Generate sample data in two tables for training ##





