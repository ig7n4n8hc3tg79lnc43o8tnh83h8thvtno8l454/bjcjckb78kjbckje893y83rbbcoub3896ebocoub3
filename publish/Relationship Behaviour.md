Configure what happens to its related records, when an action (delete or change of owner) is performed on the primary (parent) record

### Types
- **Referential** - no Cascading at all
- **Parental** - Cascading all
- **Custom** - specifically configure Delete, Share (with user/team) and Reparent operation

##### Custom options
**Cascade Active** - Perform the action on all active related entity records
**Cascade All** - Perform the action on all related entity records
**Cascade None** - Do nothing Like Referential
**Remove Link** - Remove the lookup value for all related records
**Restrict** - Prevent the primary entity record from being deleted when related entity records exist
**Cascade User Owned** - Perform the action on all related entity records owned by the same user as the primary entity record

### Example
- When you delete Expense Request record what should happen to all related Expense Item records
- When you assign (change of owner) Expense Request to your colleague, what should happen to all related Expense Item records

### Configuring Relationship Behaviour

```mermaid

graph TB

0["steps"] --> 1["<div class = 'scrollmenu'><img src='http://127.0.0.1:8000/b99c9b71-5d80-4ecf-904a-b1f64facb78a.png' width='478' height='73'/><br><br><img src='http://127.0.0.1:8000/86d88b6e-d4c3-422b-b85f-3171f5e32da5.png' width='477' height='72'/><br><br><img src='http://127.0.0.1:8000/4eda3865-fdde-4513-906f-ee3e2348ffc6.png' width='477' height='154'/><br><br><img src='http://127.0.0.1:8000/d8c06004-528b-4f4b-b957-529f05e94638.png' width='316' height='268'/><br><br><img src='http://127.0.0.1:8000/696762ed-1906-4468-8e73-33e37bc93002.png' width='334' height='267'/><br><br><b>whatever you do on expense request that<br>action will not be cascaded to expense<br>item</b><br><br></div>"]

style 0 fill:#ba271b
style 1 fill:#457eba

```
