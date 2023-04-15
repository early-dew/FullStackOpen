```mermaid
sequenceDiagram
 participant browser
 participant server
 browser->>server: POST request to the server address new_note
 server-->>browser:  server asks to do a GET request to the address notes
 browser->>browser: reloads the Notes page
 browser->>server: GET style sheet
 browser->>server: GET the style sheet
 browser->>server: GET raw data of the notes
```
