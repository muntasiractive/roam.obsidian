---
type: monthly-journal
date: <% tp.date.now("YYYY-MM") %>
ls-deep-declutter-phone: false
ls-deep-declutter-pc: false
ls-review-passwords: false
ls-update-readme: false
ls-os-updates: false
ls-clear-cache: false
ls-delete-account: false
sec-pwned: false
sec-mfa: false
sec-sessions: false
sec-privacy: false
sec-permissions: false
sec-router: false
fn-review-budget-invest-debt: false
fn-audit-subs: false
fn-update-networth: false
fn-make-budget-plan: false
fn-make-invest-plan: false
fn-verify-emergency-fund: false
fn-review-credit-score: false
cr-update-profiles: false
cr-update-resume: false
cr-update-portfolio: false
ls-reflections: ""
ac-reflections: ""
cr-reflections: ""
sk-reflections: ""
kn-reflections: ""
fn-reflections: ""
ls-health-reflections: ""
et-reflections: ""
rel-shanta: false
rel-lisha: false
rel-niloy: false
rel-arafat: false
rel-rohan: false
rel-tanvir: false
rel-mridul-mehrab: false
rel-rafid: false
rel-lubna: false
rel-mohammed: false
rel-bappy: false
rel-misty: false
rel-moyna: false
rel-sarbik: false
rel-ritu: false
rel-happy: false
rel-opi: false
rel-sami: false
rel-ruponti: false
rel-trina: false
rel-toma: false
rel-tanin: false
rel-rohit: false
rel-samia: false
rel-abdullah: false
rel-reflections: ""
rel-social-reflections: ""
sp-reflections: ""
---

# <% tp.date.now("MMMM YYYY") %>

## Performance Review

> [!abstract] **Monthly Performance Summary**
>
> ```dataview
> TABLE 
>     round(average(rows.ls-focus), 1) AS "Avg Focus", 
>     round(average(rows.ls-stress), 1) AS "Avg Stress", 
>     sum(rows.ls-deep-work) AS "Total Focus Sessions"
> FROM "Museum/Journals"
> WHERE type = "journal" AND file.day.month = this.file.day.month AND file.day.year = this.file.day.year
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
