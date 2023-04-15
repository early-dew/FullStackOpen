```mermaid
sequenceDiagram
 participant browser
 participant server
 browser->>server: POST request to the server address new_note
 activate server
 server-->>browser:  Asks to do a GET request to the address notes
 deactivate server
 browser->>browser: Notes page reloads
 browser->>server: GET style sheet
 activate server
 server-->>browser: Sends a CSS file
 deactivate server
 browser->>server: GET JavaScript code
 activate server
 server-->>browser: Sends a JavaScript file
 deactivate server
 browser->>server: GET raw data of the notes
 activate server
 server-->>browser: 
 deactivate server
```
