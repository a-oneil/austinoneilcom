---
id: <% tp.file.title.split(" ")[0] %>
created_date: <% tp.file.creation_date('YYYY.MM.DD') %>
updated_date: <% tp.file.last_modified_date('YYYY.MM.DD') %>
type: daily-note
---

# <% tp.file.title %>
- **🏷️Tags** : #<% tp.file.creation_date("YYYY-MM") %> #daily 
## Links
- [ ] 
## Thoughts




tags:: [[Daily Notes]]

# <% moment(tp.file.title,'YYYY.MM.DD-dddd').format("dddd, MMMM DD, YYYY") %>

## To-Do
- [ ] 

## Notes
- 

## TIL
- 

## For tomorrow
- 

---

## Notes created today
```dataview
LIST FROM -"Daily Notes" and -"_config" WHERE file.cday = date(this.file.frontmatter.date_created) SORT file.ctime ASC
```

## Notes last touched today
```dataview
LIST FROM -"Daily Notes" and -"_config" WHERE file.mday = date(this.file.frontmatter.date_created) SORT file.mtime ASC
```