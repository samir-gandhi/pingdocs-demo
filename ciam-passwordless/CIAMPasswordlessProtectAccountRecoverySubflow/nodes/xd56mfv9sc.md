# Http - NOP UI Page
## Configuration
ID:  xd56mfv9sc

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Description | Initiate SK Risk SDK with appropriate details to initiate PingOne Protect feature. | 
 


## Custom HTML
```html
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
        "data": "[[[skcomponent###c2tjb21wb25lbnQgInNrcmlzayIgIGVudmlyb25tZW50SWQ9IiIgY29sbGVjdEJlaGF2aW9yYWxEYXRhPSJ0cnVlIiBwcm9wZXJ0eW5hbWU9InJpc2tmcCI=###eyJuYW1lIjoic2tyaXNrIiwib3B0aW9ucyI6eyJlbnZpcm9ubWVudElkIjoiIiwiY29sbGVjdEJlaGF2aW9yYWxEYXRhIjoidHJ1ZSIsInByb3BlcnR5bmFtZSI6InJpc2tmcCJ9LCJjb21wb25lbnRQcm9wcyI6eyJlbnZpcm9ubWVudElkIjp7Im5hbWUiOiJlbnZpcm9ubWVudElkIiwiZGlzcGxheU5hbWUiOiJFbnZpcm9ubWVudCBJRCJ9LCJjb2xsZWN0QmVoYXZpb3JhbERhdGEiOnsibmFtZSI6ImNvbGxlY3RCZWhhdmlvcmFsRGF0YSIsImRpc3BsYXlOYW1lIjoiQ29sbGVjdCBiZWhhdmlvcmFsIGRhdGEiLCJ0eXBlIjoic2VsZWN0IiwidmFsdWUiOiJ0cnVlIiwiaW5mbyI6IkJlaGF2aW9yYWwgZGF0YSBpcyB1c2VkIHRvIGRldGVjdCBIdW1hbi9Ob24gSHVtYW4gdXNlcnMuIEl0IGlzIHJlY29tbWVuZGVkIHRvIHNldCB0aGUgc2FtZSB2YWx1ZSB0aHJvdWdob3V0IHRoZSBmbG93LiIsIm9wdGlvbnMiOlt7Im5hbWUiOiJUcnVlIiwidmFsdWUiOiJ0cnVlIn0seyJuYW1lIjoiRmFsc2UiLCJ2YWx1ZSI6ImZhbHNlIn1dfSwicHJvcGVydHluYW1lIjp7Im5hbWUiOiJwcm9wZXJ0eW5hbWUiLCJkaXNwbGF5TmFtZSI6IlJpc2sgUHJvcGVydHkgTmFtZSIsInZhbHVlIjoicmlza2ZwIiwiaW5mbyI6Ik5hbWUgZm9yIHJlZmVyZW5jaW5nIHRoaXMgcmlzayBjb21wb25lbnQifX19]]]",
        "src": "auth.svg",
        "url": "skrisk",
        "children": [
          {
            "text": "skrisk"
          }
        ],
        "component": "skrisk",
        "options": {
          "environmentId": "",
          "collectBehavioralData": "true",
          "propertyname": "riskfp"
        },
        "componentProps": {
          "environmentId": {
            "name": "environmentId",
            "displayName": "Environment ID"
          },
          "collectBehavioralData": {
            "name": "collectBehavioralData",
            "displayName": "Collect behavioral data",
            "type": "select",
            "value": "true",
            "info": "Behavioral data is used to detect Human/Non Human users. It is recommended to set the same value throughout the flow.",
            "options": [
              {
                "name": "True",
                "value": "true"
              },
              {
                "name": "False",
                "value": "false"
              }
            ]
          },
          "propertyname": {
            "name": "propertyname",
            "displayName": "Risk Property Name",
            "value": "riskfp",
            "info": "Name for referencing this risk component"
          }
        },
        "tooltip": "{{component.skrisk}}"
      },
      {
        "text": ""
      },
      {
        "text": "<div style="display: none">"
      },
      {
        "text": ""
      },
      {
        "type": "link",
        "data": "[[[skcomponent###c2tjb21wb25lbnQgInNrcG9sbGluZyIgIGNsYXNzPSIiIHBvbGxJbnRlcnZhbD0iMTAiIHBvbGxSZXRyaWVzPSIxIiBwb2xsQ2hhbGxlbmdlU3RhdHVzPSJmYWxzZSI=###eyJuYW1lIjoic2twb2xsaW5nIiwib3B0aW9ucyI6eyJjbGFzcyI6IiIsInBvbGxJbnRlcnZhbCI6IjEwIiwicG9sbFJldHJpZXMiOiIxIiwicG9sbENoYWxsZW5nZVN0YXR1cyI6ImZhbHNlIn0sImNvbXBvbmVudFByb3BzIjp7ImNsYXNzIjp7Im5hbWUiOiJjbGFzcyIsImRpc3BsYXlOYW1lIjoiQ1NTIENsYXNzIn0sInBvbGxJbnRlcnZhbCI6eyJuYW1lIjoicG9sbEludGVydmFsIiwiZGlzcGxheU5hbWUiOiJQb2xsIEludGVydmFsIiwidmFsdWUiOjIwMDB9LCJwb2xsUmV0cmllcyI6eyJuYW1lIjoicG9sbFJldHJpZXMiLCJkaXNwbGF5TmFtZSI6IlBvbGwgUmV0cmllcyIsInZhbHVlIjo2MH0sInBvbGxDaGFsbGVuZ2VTdGF0dXMiOnsibmFtZSI6InBvbGxDaGFsbGVuZ2VTdGF0dXMiLCJkaXNwbGF5TmFtZSI6IlBvbGwgQ2hhbGxlbmdlIFN0YXR1cyIsInR5cGUiOiJzZWxlY3QiLCJ2YWx1ZSI6InRydWUiLCJvcHRpb25zIjpbeyJuYW1lIjoiVHJ1ZSIsInZhbHVlIjoidHJ1ZSJ9LHsibmFtZSI6IkZhbHNlIiwidmFsdWUiOiJmYWxzZSJ9XX19fQ==]]]",
        "src": "auth.svg",
        "url": "skpolling",
        "children": [
          {
            "text": "skpolling"
          }
        ],
        "component": "skpolling",
        "options": {
          "class": "",
          "pollInterval": "10",
          "pollRetries": "1",
          "pollChallengeStatus": "false"
        },
        "componentProps": {
          "class": {
            "name": "class",
            "displayName": "CSS Class"
          },
          "pollInterval": {
            "name": "pollInterval",
            "displayName": "Poll Interval",
            "value": 2000
          },
          "pollRetries": {
            "name": "pollRetries",
            "displayName": "Poll Retries",
            "value": 60
          },
          "pollChallengeStatus": {
            "name": "pollChallengeStatus",
            "displayName": "Poll Challenge Status",
            "type": "select",
            "value": "true",
            "options": [
              {
                "name": "True",
                "value": "true"
              },
              {
                "name": "False",
                "value": "false"
              }
            ]
          }
        },
        "tooltip": "{{component.skpolling}}"
      },
      {
        "text": ""
      },
      {
        "text": "</div>"
      }
    ]
  }
]
```


### Additional Properties
formFieldsList
 ```json 

```




### Position
| Previous Nodes | Future Nodes |
| :------------- | ------------ |
|  | [n9k3edxufj](./n9k3edxufj.md) |