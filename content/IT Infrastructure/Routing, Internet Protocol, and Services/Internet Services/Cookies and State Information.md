---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Cookies and State Information

- A **cookie** is data created by a web server and stored on a user's hard drive, used to track user activity and predict future needs.
  - Cookies provide convenience in business transactions by remembering user preferences and previous activities.
  - Information stored in cookies can also be used by other websites to deliver customized content.
- Many consider cookies an invasion of privacy due to their tracking capabilities.

### Cookie Interaction Example

1. **Client-Server Communication**: 
   - Upon accessing a website, the server sends a usual HTTP response message along with a cookie (e.g., `set-cookie: 1678`).
   - The client stores the cookie on the local hard drive.
  
2. **Subsequent Requests**:
   - When the user returns to the site, their browser sends the cookie back to the server (e.g., `cookie: 1678`), enabling access to user-specific actions and content.