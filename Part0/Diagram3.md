```mermaid
sequenceDiagram
    participant browser
    participant server

    browser -->> server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa   payload  {content: "new note", date: "2025-09-            27T20:23:13.118Z"
    activate server

    server -->> browser: Status 201 Created   {"message":"note created"}
    deactivate server    
```
