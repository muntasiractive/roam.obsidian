---
status: not started
region:
due_date:
opr_id: <% tp.file.title.substring(4) %>
created: <% tp.date.now("Do MMM YYYY [at ]HH[hrs & ]mm[min]") %>
type: operation
---
> [!question] Properties
> `Status` `INPUT[inlineSelect(option(not started), option(started), option(end), option(paused)):status]` `Due Date` `INPUT[datePicker:due_date]` `Region` `INPUT[inlineSelect(option(academic), option(career), option(entertainment), option(finance), option(health), option(knowledge), option(lifestyle), option(relationship), option(skill), option(social), option(spirituality)):region]`
# Overview

> [!info] **Purpose**
> <% tp.file.cursor() %>

> [!danger] **Overdue Tasks**
>
> ```tasks
> not done
> no done date
> no cancelled date
>  (status.type is TODO) OR (status.type is IN_PROGRESS)
> ((starts before today) AND (due before today)) OR (scheduled before today) 
> path includes {{query.file.path}}
> sort by urgency
> sort by scheduled
> sort by due
> sort by status.type
> short mode
> ```

> [!todo] **Today's Tasks**
>
> ```tasks
> not done
> no done date
> no cancelled date
>  (status.type is IN_PROGRESS) OR (status.type is TODO)
> (scheduled on today) OR ((starts on or before today) AND (due on or after today))
> sort by scheduled
> sort by due
> sort by priority
> short mode
> path includes {{query.file.path}}
> ```

> [!calendar] **Upcoming Tasks**
>
> ```tasks
> not done
> no done date
> no cancelled date
> (status.type is TODO)
> (((has start date) AND (starts after today)) AND ((has due date) AND (due after today))) OR ((has scheduled date) AND (scheduled after today))
> path includes {{query.file.path}}
> sort by scheduled
> sort by due
> sort by priority
> limit 15
> short mode
> ```
# Task
## Others
- [ ] Set Goals for `<% tp.file.title.substring(4) %>`
# Wiki

```meta-bind-button
label: Create Linked Wiki
icon: "book-plus"
style: plain
class: wiki
actions:
  - type: command
    command: quickadd:choice:a0847609-be65-4fbd-95bc-5a50233dbd01
```

```dataview
TABLE WITHOUT ID
  file.link AS "Wiki",
  region AS "Region",
  due_at AS "Due At"
FROM "Reflections/Wikis"
WHERE opr_id = this.opr_id
```
