    sequenceDiagram
        participant browser
        participant server

    browser->>server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: Status Code 201 with Response{"message":"note created"}
    deactivate server

