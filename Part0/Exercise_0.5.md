```mermaid

sequenceDiagram

Participant Browser
Participant Server


Browser->>Server:Get https://studies.cs.helsinki.fi/exampleapp/spa
Activate Browser
Activate Server
Server-->>Browser:HTML Document
Deactivate Browser
Deactivate Server

Browser->>Server:Get https://studies.cs.helsinki.fi/exampleapp/main.css
Activate Browser
Activate Server
Server-->>Browser:The CSS File
Deactivate Browser
Deactivate Server

Browser->>Server:Get https://studies.cs.helsinki.fi/exampleapp/spa.js
Activate Browser
Activate Server
Server-->>Browser:The JavaScript File
Deactivate Browser
Deactivate Server

Browser->>Server:Get https://studies.cs.helsinki.fi/exampleapp/data.json
Activate Browser
Activate Server
Server-->>Browser:The JSON File
Deactivate Browser
Deactivate Server

Browser->>Server:Get https://studies.cs.helsinki.fi/favicon.ico
Activate Browser
Deactivate Browser
Note Right of Browser:The Browser Waits for response but the Server Can't find the requested file
```