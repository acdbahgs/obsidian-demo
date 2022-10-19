---
date: <% tp.date.now("YYYY-MM-DD") %>
type: meeting
company: LEM11
summary: "Trying to get Templater work"
tags: index
---

### Last modified date - dynamic cmd: <%+ tp.file.last_modified_date() %>

### Web Daily quote:  <% tp.web.daily_quote() %>

### Web Random picture: <% tp.web.random_picture() %>

### Web Random picture with size: <% tp.web.random_picture("200x200") %>

### Web random picture with size + query: <% tp.web.random_picture("200x200", "landscape,water") %>
 

### File title - not working: `<% tp.file.title %>`
### File creation date: <% tp.file.creation_date() %>
### File existence - Postgres: <% tp.file.exists("Postgres") %>
### File Last Modif Date: <% tp.file.last_modified_date() %> 
### File Last Modif Date with format: <% tp.file.last_modified_date("dddd Do MMMM YYYY HH:mm") %>

### File tags - not working: <% tp.file.tags %>

### Run_mode: <% tp.config.run_mode %>

Date now: <% tp.date.now() %>
Date now with format: <% tp.date.now("Do MMMM YYYY") %>

Last week: <% tp.date.now("dddd Do MMMM YYYY", -7) %>
Today: <% tp.date.now("dddd Do MMMM YYYY, ddd") %>
Next week: <% tp.date.now("dddd Do MMMM YYYY", 7) %>

Last month: <% tp.date.now("YYYY-MM-DD", "P-1M") %>
Next year: <% tp.date.now("YYYY-MM-DD", "P1Y") %>

### File's title date + 1 day (tomorrow): <% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>
### File's title date - 1 day (yesterday): <% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>

### Date tomorrow with format: <% tp.date.tomorrow("Do MMMM YYYY") %>    

### This week's monday: <% tp.date.weekday("YYYY-MM-DD", 0) %>
### Next monday: <% tp.date.weekday("YYYY-MM-DD", 7) %>
### File's title monday: <% tp.date.weekday("YYYY-MM-DD", 0, tp.file.title, "YYYY-MM-DD") %>
### File's title next monday: <% tp.date.weekday("YYYY-MM-DD", 7, tp.file.title, "YYYY-MM-DD") %>

### Date yesterday with format: <% tp.date.yesterday("Do MMMM YYYY") %>


## Attendees


## Agenda

## Log
