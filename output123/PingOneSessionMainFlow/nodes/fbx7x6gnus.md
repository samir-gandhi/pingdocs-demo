# PingOne Authentication - Return success
## Configuration
ID:  fbx7x6gnus

Type: action 

CapabilityName: returnSuccessResponseRedirect

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- || Valid Authentication Method | pwd
| User ID | ```json[
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
        "src": "teleport.svg",
        "url": "userId",
        "data": "{{local.ofk8hitz8r.payload.output.userId}}",
        "tooltip": "{{local.ofk8hitz8r.payload.output.userId}}",
        "children": [
          {
            "text": "userId"
          }
        ]
      },
      {
        "text": ""
      }
    ]
  }
]``` |
| Expire Authentication Token | pwd |
| Node Background Color | #9dc967ff | 

| Node Description | Returns successful flow completion back to the PingOne application connection | }
 



