# Http - Magic Link Polling
## Configuration
ID:  fhoue68esb

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Magic Link polling screen | 
 


## Custom HTML
```html
<div class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
    <div style="max-width: 400px; min-width: 400px; width: 100%">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
                {{global.parameters.ciam_companyLogo}}              
                <p class="text-muted text-center">A verification link is being sent to your email address.</p>
                <div class="align-self-center">
                [[[skcomponent###c2tjb21wb25lbnQgInNrcG9sbGluZyIgIGNsYXNzPSIiIHBvbGxJbnRlcnZhbD0iMzAwMCIgcG9sbFJldHJpZXM9IjM1IiBwb2xsQ2hhbGxlbmdlU3RhdHVzPSJ0cnVlIg==###eyJuYW1lIjoic2twb2xsaW5nIiwib3B0aW9ucyI6eyJjbGFzcyI6IiIsInBvbGxJbnRlcnZhbCI6IjMwMDAiLCJwb2xsUmV0cmllcyI6IjM1IiwicG9sbENoYWxsZW5nZVN0YXR1cyI6InRydWUifSwiY29tcG9uZW50UHJvcHMiOnsiY2xhc3MiOnsibmFtZSI6ImNsYXNzIiwiZGlzcGxheU5hbWUiOiJDU1MgQ2xhc3MifSwicG9sbEludGVydmFsIjp7Im5hbWUiOiJwb2xsSW50ZXJ2YWwiLCJkaXNwbGF5TmFtZSI6IlBvbGwgSW50ZXJ2YWwiLCJ2YWx1ZSI6MjAwMH0sInBvbGxSZXRyaWVzIjp7Im5hbWUiOiJwb2xsUmV0cmllcyIsImRpc3BsYXlOYW1lIjoiUG9sbCBSZXRyaWVzIiwidmFsdWUiOjYwfSwicG9sbENoYWxsZW5nZVN0YXR1cyI6eyJuYW1lIjoicG9sbENoYWxsZW5nZVN0YXR1cyIsImRpc3BsYXlOYW1lIjoiUG9sbCBDaGFsbGVuZ2UgU3RhdHVzIiwidHlwZSI6InNlbGVjdCIsInZhbHVlIjoidHJ1ZSIsIm9wdGlvbnMiOlt7Im5hbWUiOiJUcnVlIiwidmFsdWUiOiJ0cnVlIn0seyJuYW1lIjoiRmFsc2UiLCJ2YWx1ZSI6ImZhbHNlIn1dfX19]]]
                </div>
            </div>
        </div>
    </div>
</div>
```


### Additional Properties
challenge
 ```json 
[
  {
    "children": [
      {
        "text": ""
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "src": "flow-connector.svg",
        "url": "challenge",
        "data": "{{local.zsk0ny89ud.payload.output.challenge}}",
        "tooltip": "{{local.zsk0ny89ud.payload.output.challenge}}",
        "children": [
          {
            "text": "challenge"
          }
        ]
      },
      {
        "text": ""
      }
    ]
  }
]
```


formFieldsList
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
| [ali9zum89s](./ali9zum89s.md) | [2ynekjzhbj](./2ynekjzhbj.md) |