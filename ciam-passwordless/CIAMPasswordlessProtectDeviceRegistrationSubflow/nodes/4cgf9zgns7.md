# Http - string 
Get Origin
## Configuration
ID:  4cgf9zgns7

Type: CONNECTION 

CapabilityName: customHTMLTemplate


## Custom CSS
```css
json 
.hidden-button {
  display: none;
}
```

## Custom HTML
```json 
[
  {
    "children": [
      {
        "text": "<form id="location" method="post">    <input type="hidden" name="origin" id=""
      },
      {
        "text": "origin"
      },
      {
        "text": "">"
      }
    ]
  },
  {
    "children": [
      {
        "text": "    <input type="hidden" name=""
      },
      {
        "text": "rpid"
      },
      {
        "text": "" id=""
      },
      {
        "text": "rpid"
      },
      {
        "text": "">"
      },
      {
        "text": "    <button type="hidden" data-skcomponent="skbutton" data-skbuttontype="form-submit" class="hidden-button"  data-skbuttonvalue="submit" data-skform=""
      },
      {
        "text": "location"
      },
      {
        "text": "" id="autoSubmit">Next</button></form>"
      }
    ]
  }
]
```

## Custom Script
```js 
setTimeout(function() {
    const origin = window.location.origin;
    document.getElementById("origin").value = origin;
    const index = origin.indexOf(":");
    const index2 = index &#43; 3;
    document.getElementById("rpid").value = origin.substr(index2);
    document.getElementById(&#39;autoSubmit&#39;).click();
}, 1000);
```


### Additional Properties
formFieldsList
```
```




