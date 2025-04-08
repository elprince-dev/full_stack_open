``` mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: Status 201: Created
    deactivate server

    note right of browser: browser excultes the event handler and re-renders notes

```