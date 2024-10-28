# Http - string 
Show Expiration Error
## Configuration
ID:  utjcbphp35

Type: CONNECTION 

CapabilityName: customHTMLTemplate



## Custom HTML
```html 
<div class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
   <div style="max-width: 400px; min-width: 400px; width: 100%">
        <div class="card shadow mb-5">
            <div class="card-body p-5 d-flex flex-column">
                {{global.parameters.ciam_companyLogo}}
                <h1 class="text-center mb-4">Error</h1>
                <p class="text-muted text-center">Magic Link has expired.</p>
            </div>
        </div>
    </div>
</div>
```



