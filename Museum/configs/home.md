---
type: dashboard
last_update: 2026-07-14 21:17
---

$$ {\huge {\color{blue}R}.{\color{red}O}.{\color{green}A}.{\color{orange}M}.}$$  
$$ {\large Reflection.Operation.Asset.Museum }$$
$$ {\small {\color{olive}Hello}, \ Muntasir! \ Let's \ work \ on \ something \ great.} $$

> [!tip] At a Glance
> `BUTTON[button-today-journal]` `BUTTON[button-new-op]` `BUTTON[button-new-wiki]`
> 
> `BUTTON[quicktask]` `BUTTON[timeline]`

---

# 📥Inbox
## ❗**Overdue Task**

> [!danger] ###### Do these tasks before anything else
> ```tasks
> not done
> no done date
> no cancelled date
>  (status.type is TODO) OR (status.type is IN_PROGRESS)
> ((starts before today) AND (due before today)) OR (scheduled before today) 
> sort by scheduled
> sort by due
> sort by priority
> short mode
> group by priority
> group by filename
> ```
## 📅 **Today's Stream**

> [!todo] ###### Finish these first
> ```tasks
> not done
> no done date
> no cancelled date
>  (status.type is IN_PROGRESS) OR (status.type is TODO)
>  ((scheduled on today)) OR ((starts on or before today) AND (due on today)) 
> group by priority
> group by filename
> sort by scheduled
> sort by due
> sort by priority
> short mode
> ```

> [!todo] ###### Then work on these and touch upcoming 
> ```tasks
> not done
> no done date
> no cancelled date
>  (status.type is TODO) OR (status.type is IN_PROGRESS)
> ((starts on or before today) AND (due after today)) 
> group by priority
> group by filename
> sort by scheduled
> sort by due
> sort by priority
> short mode
> ```

---
# 🎯Operations
```dataview
TABLE WITHOUT ID
  link(file.link, opr_id) AS "Operation",
  due_date AS "Deadline",
  region AS "Region"
FROM "Operations"
WHERE type = "operation" AND status = "started"
SORT due_date ASC
```
