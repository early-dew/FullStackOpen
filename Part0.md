```mermaid
sequenceDiagram
 participant browser
 participant server
 browser->>server: POST request to the server address new_note
 activate server
 server-->>browser:  server asks to do a GET request to the address notes
 deactivate server
 browser->>browser: reloads the Notes page
 browser->>server: GET style sheet
 activate server
 server-->>browser: sends a CSS file
 deactivate server
 browser->>server: GET JavaScript code
 activate server
 server-->>browser: sends a JavaScript file
 deactivate server
 browser->>server: GET raw data of the notes
 server-->>browser: 
```
