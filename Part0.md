```mermaid
sequenceDiagram
 participant browser
 participant server
 browser->>server: POST request to the server address new_note
 activate server
 server-->>browser:  Server asks to do a GET request to the address notes
 deactivate server
 browser->>browser: Reloads the Notes page
 browser->>server: GET style sheet
 activate server
 server-->>browser: Sends a CSS file
 deactivate server
 browser->>server: GET JavaScript code
 activate server
 server-->>browser: Sends a JavaScript file
 deactivate server
 browser->>server: GET raw data of the notes
 server-->>browser: 
```
