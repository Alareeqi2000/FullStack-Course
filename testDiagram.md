```mermaid
sequenceDiagram
  browser->>server:GET https://studies.cs.helsinki.fi/exampleapp 
  Activate server
server-->browser:HTML document
deactivate server
 browser->>server:GET https://studies.cs.helsinki.fi/exampleapp/kuva.png
 Activate server
 server-->browser:the png pic
 deactivate server
note right of browser:Page with a pic will be rendered
```