# Http - NOP UI Page
## Configuration
ID:  64hrke1krq

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
 


## Custom HTML
```html
[
  {
    "children": [
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
|  | [2vij7q7i5j](./2vij7q7i5j.md) |