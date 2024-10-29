# Http - string 
Error Message
## Configuration
ID:  ue7utb27ym

Type: CONNECTION 

CapabilityName: customHTMLTemplate

### Settings
| Setting | Value  |
| :------------------------ | ---------------------------------------- |
| Node Background Color | html 
#ffc8c1ff | 

| Node Description | string 
Configuration value not set error | 

## Custom CSS
```css
string 

```

## Custom HTML
```html 
<div
  class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
  <div style="max-width: 400px; min-width: 400px; width: 100%">
    <div class="card shadow mb-5">
      <div class="card-body p-5 d-flex flex-column">
        <img class="companyLogo align-self-center mb-5" alt="{{global.variables.companyName}}" />
        <h1 class="text-center mb-4">Flow Configuration Error</h1>
        <p class="text-muted text-center">{{errorMessage}}</p>
      </div>
    </div>
  </div>
</div>
```

## Custom Script
```string 

```


### Additional Properties
errorMessage
```json 
[
  {
    "children": [
      {
        "text": "Unable to execute the flow due to missing parameter values."
      }
    ]
  }
]
```


formFieldsList
```
```


inputSchema
```json 
{
	"type": "object",
	"properties": {
		"errorMessage": {
			"type": "string",
			"displayName": "Error Message",
			"preferredControlType": "textField",
			"enableParameters": true,
			"propertyName": "errorMessage"
		}
	}
}
```


sktemplate
```string 
f3e47d945ae971a4b4142ec75012d155
```


validationRules
```
```




