---
type: weekly-journal
date: <% tp.date.now("YYYY-[W]ww") %>
sp-read-kahf: false
sp-salawat-friday: false
sp-friday-ghusl: false
sp-friday-sunnah: false
sp-friday-early: false
sp-friday-charity: false
rel-boro-kakku: false
rel-sejo-kakku: false
rel-nowa-kakku: false
rel-boro-mama: false
rel-soto-mama: false
rel-boro-khala: false
rel-mejho-khala: false
rel-sejo-khala: false
rel-soto-khala: false
rel-bappy: false
rel-moyna: false
rel-misty: false
rel-trina: false
rel-toma: false
rel-tanin: false
rel-happy: false
rel-opi: false
rel-sarbik: false
rel-ritu: false
rel-samo: false
rel-ruponti: false
rel-ahmed: false
rel-rohit: false
rel-samia: false
rel-mohammed-1: false
rel-lisha: false
rel-santa: false
rel-niloy: false
rel-arafat: false
rel-rohan: false
rel-tanvir: false
rel-lubna: false
rel-mohammed-2: false
rel-mridul: false
rel-mehrab: false
ls-flaw-quit: false
ls-implement-char: false
ls-declutter-home: false
ls-upload-roam: false
ls-declutter-roam: false
ls-clean-phone: false
ls-clean-pc: false
ls-verify-backup: false
ls-fast-monday: false
cr-codeberg: false
ls-reflections: ""
ac-reflections: ""
cr-reflections: ""
sk-reflections: ""
kn-reflections: ""
fn-reflections: ""
ls-health-reflections: ""
et-reflections: ""
rel-reflections: ""
rel-social-reflections: ""
sp-reflections: ""
---

# <% tp.date.now("[W]ww") %>

## Performance Review

> [!abstract] **Focus & Stress Summary**
>
> ```dataview
> TABLE 
>     round(average(rows.ls-focus), 1) AS "Avg Focus", 
>     round(average(rows.ls-stress), 1) AS "Avg Stress", 
>     sum(rows.ls-deep-work) AS "Total Focus Sessions"
> FROM "Museum/Journals"
> WHERE type = "journal" AND date >= date(<% tp.date.now("YYYY-MM-DD", -7) %>)
> GROUP BY true
> ```

## Lifestyle
## Academic
## Careers
## Skill

## Knowledge
## Finance
## Health
## Entertainment
## Relationship
## Social
## Spirituality

## Prayer
