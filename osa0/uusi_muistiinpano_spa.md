```mermaid
sequenceDiagram
    participant user
    participant browser
    participant server

    user->>browser: Type note content and click save

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa, JSON data
    activate server
    Note right of server: Server does stuff
    server-->>browser: 201 created
    deactivate server
```
