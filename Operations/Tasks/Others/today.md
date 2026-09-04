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
> ```