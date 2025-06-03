# CGM to Pump and watch Diagram Example

## Flowcharts

```mermaid
graph LR
  A[Start] --> B{Xdrip+};
  B -->|Yes| C[Investigate...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Success!];
```



```mermaid
graph LR
  A[CGM] --> B{xDrip+};
  A[CGM] <--> I{Dexcom G6 APP};
  H[PDM] <--> I{Dexcom G6 APP};
  A[CGM] --> H{PDM};
  A[CGM] --> C[Nightscout];
  A[CGM] --> D[AAPS];
  B <-->|to| C[Nightscout];
  C <--> D[AAPS];
  F --> D[AAPS];
  D --> g[Watch];
  B <--> g[Watch];
  F <--> g[Watch];
  D <--> B;
  B ---->|will| E[Succeed !];
  F[Pump - Pod] ---->|will| E[Succeed !];
  F[Pump - Pod] ---->H[PDM];
  
```


## Sequence Diagrams

```mermaid
sequenceDiagram
  autonumber
  Server->>Terminal: Send request
  loop Health
      Terminal->>Terminal: Check for health
  end
  Note right of Terminal: System online
  Terminal-->>Server: Everything is OK
  Terminal->>Database: Request customer data
  Database-->>Terminal: Customer data
```


=== "🔄 AAPS in Action"
``` mermaid
graph LR
  A[CGM] --> |Bluetooth| B[AAPS App];
  B -->|Commands| C[Insulin Pump];
  C --> D[Adjust Insulin];
  B --> E[Nightscout Cloud];
  E --> F[Caregiver/Monitor];
```
=== "mermaid"
```js title="code-examples.md" linenums="1" hl_lines="2-4"
graph LR
  A[CGM] --> |Bluetooth| B[AAPS App];
  B -->|Commands| C[Insulin Pump];
  C --> D[Adjust Insulin];
  B --> E[Nightscout Cloud];
  E --> F[Caregiver/Monitor];
```


=== "mermaid"
```js title="code" 
graph LR
  A[CGM] --> |Bluetooth| B[AAPS App];
  B -->|Commands| C[Insulin Pump];
  C --> D[Adjust Insulin];
  B --> E[Nightscout Cloud];
  E --> F[Caregiver/Monitor];
```

=== "Sensor Applicator"

    <img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/c1ba943f-9cfc-4fdf-bbc1-c20955823984" title="Sensor Applicator"/></a>

=== "Sensor"

    <img width="Auto" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/e1682efa-b4e4-4874-93fe-1caa106f24b9" title="Sensor"/></a>
    

=== "Transmitter "

    <img width="300" height="Auto" border="0" align="left"  src="https://github.com/user-attachments/assets/be60b7f9-58bb-4a4f-8775-2dd0c851a6fb" title="Transmitter"/><center></a><img width="260" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/f331bf48-3ad1-456b-8484-503c37d780a1" title="Transmitter Serial "/></center></a>

    ### Code Blocks in Content Tabs

=== "Display"

    <img width="300" height="Auto" border="0" align="center"  src="https://github.com/user-attachments/assets/962a2daf-fb71-4133-b434-b97f0ce77cc0" title="Displays"/></a>

=== "mermaid"
```js title="code" linenums="1" hl_lines="2-4"
graph LR
  A[CGM] --> |Bluetooth| B[AAPS App];
  B -->|Commands| C[Insulin Pump];
  C --> D[Adjust Insulin];
  B --> E[Nightscout Cloud];
  E --> F[Caregiver/Monitor];
```