---
type: daily
aliases: ["<% moment(tp.file.title,'YYYY-MM-DD').format("dddd MMMM DD YYYY") %>"]
tags: [daily]
siblings:
  - "[[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').subtract(1, 'd').format('YYYY-MM-DD-dddd') %>]]"
  - "[[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').add(1, 'd').format('YYYY-MM-DD-dddd') %>]]"
  - "[[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').format('YYYY-[W]ww') %>#<%tp.file.title%>|<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').format('YYYY-[W]ww') %>]]"
  - "[[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').format('YYYY-MM-MMMM') %>]]"
---
# 📅 <% moment(tp.file.title,'YYYY-MM-DD').format("dddd, MMMM DD, YYYY") %>

***Notes last touched***
```dataview
LIST
FROM -"__Z"
WHERE file.mday = date("<%moment(tp.file.title,'YYYY-MM-DD').format("YYYY-MM-DD")%>") OR file.cday = date("<%moment(tp.file.title,'YYYY-MM-DD').format("YYYY-MM-DD")%>") SORT file.mtime desc
```


 ✅ 🍊 📊 ❇️  🍱 📝 🕹 👁🧽🏹👩‍🌾🚶🏻‍♂️✏️📝🔍📊🏃🏻‍♂️📃📄🧾📊📈📉🗓📆📅🗄📋📎🔖📖📏📐📚✏️🔓🔎🖋✒️📁📂〰️❌
