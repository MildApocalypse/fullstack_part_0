# fullstackopen_part_0_ex0.6

```mermaid
    sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: [{ "message": "note created" }]
    deactivate server

    Note left of server: The server sends HTTP code 201 to the browser
    Note right of browser: The browser pushes the note itself with the javascript code
    
```