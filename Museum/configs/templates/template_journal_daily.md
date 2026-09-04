---
date: <% tp.date.now("YYYY-MM-DD") %>
type: journal
ls-mood: 5
ls-focus: 5
ls-stress: 5
ls-deep-work: 0
ls-bath: false
ls-brushed-2x: false
ls-sleep-time: 00:00
ls-wake-time: 00:00
ls-gratitude: ""
ls-sleep-hours: 0
ls-sleep-quality: ""
ls-water-glasses: 0
ls-breakfast-done: false
ls-breakfast: ""
ls-lunch-done: false
ls-lunch: ""
ls-dinner-done: false
ls-dinner: ""
ls-fasting: false
ls-workout: ""
ls-workout-duration: 0
ls-workout-intensity: ""
ls-workout-log: ""
ls-steps: 0
ls-drinking-log: ""
ls-media-log: ""
ls-reflections: ""
ls-health-reflections: ""
sp-fajr-dua: ""
sp-fajr-sunnah: false
sp-fajr-fardh: false
sp-fajr-quran: false
sp-dhuhr-dua: ""
sp-dhuhr-sunnah-b: false
sp-dhuhr-fardh: false
sp-dhuhr-quran: false
sp-asr-dua: ""
sp-asr-fardh: false
sp-asr-quran: false
sp-maghrib-dua: ""
sp-maghrib-sunnah: false
sp-maghrib-fardh: false
sp-maghrib-quran: false
sp-isha-dua: ""
sp-isha-sunnah-a: false
sp-isha-fardh: false
sp-isha-quran: false
sp-tahajjud-nafl: false
sp-ishraq-nafl: false
sp-isha-witr: false
sp-read-nuh: false
sp-read-ambiya: false
sp-say-astaghfirullah: false
sp-done-for-allah: ""
ac-study-topics: ""
ac-study-hours: 0
ac-reflections: ""
cr-write-blogs: false
cr-post-blog: false
cr-cmnt-blog: false
cr-record-vlog: false
cr-post-vlog: false
cr-work-achievements: ""
cr-cold-connect: false
cr-cold-email: false
cr-cold-email-target: ""
cr-reflections: ""
kn-learned-today: ""
kn-articles-read: 0
kn-gfg: false
kn-gnews: false
kn-feedly: false
kn-ted: false
kn-devtools: false
kn-krebs: false
kn-indiehackers: false
kn-quranedu: false
kn-techblogs: false
kn-assimalhakeem: false
kn-noumanali: false
kn-zakirnaik: false
kn-muftimenk: false
kn-mercifulservant: false
fn-money-spent: 0
fn-purchases: ""
fn-income: 0
fn-income-source: ""
fn-reflections: ""
rel-family-interaction: ""
rel-jannatul: false
rel-ammu: false
rel-abbu: false
rel-vaiya: false
rel-vabi: false
rel-ilhan: false
rel-teach-islam: false
rel-discuss-islam: false
rel-extended-updates: ""
rel-social-reflections: ""
et-movie: ""
et-movie-rate: 0
et-series: ""
et-series-rate: 0
et-anime: ""
et-anime-rate: 0
et-book: ""
et-book-rate: 0
et-game: ""
et-game-rate: 0
Calendar Title: "[[Museum/configs/templates/template_journal_daily|template_journal_daily]]"
---
# <% tp.date.now("dddd, Do MMM YYYY") %>

> [!example] **Navigation**
>
> [[<% tp.date.now("YYYY-MM-DD", -1) %>|Yesterday]] | [[<% tp.date.now("YYYY-MM-DD", 1) %>|Tomorrow]]

---
# Journals

## Lifestyle
## Academic
## Health
## Entertainment
## Knowledge
## Careers
## Finance
## Relationship
## Social
## Spirituality

---

# Inbox

## Notes Created Today

```dataview
LIST 
WHERE file.cday = date("<% tp.date.now("YYYY-MM-DD") %>") AND file.name != this.file.name
```

## Tasks Completed Today

> [!NOTE] Tasks Completed Today
>
> ```tasks
>  (status.type is TODO) OR (status.type is IN_PROGRESS)
> (((starts on or before <% tp.date.now("YYYY-MM-DD") %>) AND (due on or after <% tp.date.now("YYYY-MM-DD") %>)) OR (scheduled on <% tp.date.now("YYYY-MM-DD") %>) ) OR (((starts before <% tp.date.now("YYYY-MM-DD") %>) AND (due before <% tp.date.now("YYYY-MM-DD") %>)) OR (scheduled before <% tp.date.now("YYYY-MM-DD") %>) )
> sort by scheduled
> sort by due
> sort by priority
> group by filename
> short mode
> ```
