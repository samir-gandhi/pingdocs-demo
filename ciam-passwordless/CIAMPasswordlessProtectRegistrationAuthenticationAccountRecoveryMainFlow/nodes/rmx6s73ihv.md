# Http - string 
Passwordless Sign On Page
## Configuration
ID:  rmx6s73ihv

Type: CONNECTION 

CapabilityName: customHTMLTemplate


## Custom CSS
```css
json 
.social-buttons {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  justify-content: center;
}

.social-buttons > div {
  width: auto !important;
  margin-bottom: 10px;
}
```

## Custom HTML
```html 
[{"children":[{"text":"<div    class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">    <div style="max-width: 400px; min-width: 400px; width: 100%">        <div class="card shadow mb-5">            <div class="card-body p-5 d-flex flex-column">                "},{"text":""},{"type":"link","src":"url:4rjs3llu20","url":"flowCompanyLogo","data":"{{local.4rjs3llu20.payload.output.flowCompanyLogo}}","tooltip":"{{local.4rjs3llu20.payload.output.flowCompanyLogo}}","children":[{"text":"{{local.4rjs3llu20.payload.output.flowCompanyLogo}}"}]},{"text":""},{"text":"                <h1 class="text-center mb-4">Sign On</h1>                "},{"text":""},{"type":"link","src":"url:4rjs3llu20","url":"flowCompanyGreeting","data":"{{local.4rjs3llu20.payload.output.flowCompanyGreeting}}","tooltip":"{{local.4rjs3llu20.payload.output.flowCompanyGreeting}}","children":[{"text":"{{local.4rjs3llu20.payload.output.flowCompanyGreeting}}"}]},{"text":""},{"text":"                <div style="height:20px">                    <p class="text-danger mdi mdi-alert-circle" data-id="feedback" data-skcomponent="skerror"></p>                    <p class="text-danger mdi mdi-alert-circle" data-skerrorid="email" data-skcomponent="skerrormessage"></p>                </div>                <form id="form" data-id="form">                    <div class="mb-4 form-floating">                        <input class="form-control" type="text" id="email" name="email" placeholder="email"                            autocomplete="off" value="" data-id="email-input" value"},{"text":"="},{"text":""},{"type":"link","src":"http.svg","url":"email","data":"{{local.q6r80e7ep2.payload.output.email}}","tooltip":"{{local.q6r80e7ep2.payload.output.email}}","children":[{"text":"email"}]},{"text":""},{"text":">                        <label class="form-label" for="email">Email Address</label>                    </div>                    <div class="d-flex flex-column">                        <div class="mb-4 form-check">                            <input                            class="form-check-input"                            type="checkbox"                            name="rememberMe"                            autocomplete="off"                            data-id="rememberMe-input"                            id="rememberMe"                            /><label class="form-check-label" for="rememberMe">Remember Me?</label>                        </div>                        <button data-id="button" type="submit" class="btn btn-primary" data-skcomponent="skbutton"                            data-skbuttontype="form-submit" data-skform="form" id="btnSignIn"                            data-skbuttonvalue="SIGNON">                            Sign On                        </button>                        {{#unless passwordlessRequired}}                        <button data-id="button" type="submit" class="btn btn-outline-secondary mt-3" data-skcomponent="skbutton"                            data-skbuttontype="next-event" data-skform="form" id="btnBack"                            data-skbuttonvalue="PASSWORD">                            Use Password                        </button>                        {{/unless}}                                           {{#if socialRegistrationEnabled}}                        <div class="d-flex flex-row align-items-center my-4">                            <hr class="flex-grow-1" />                            <span class="fs-5 fw-bold px-3">OR</span>                            <hr class="flex-grow-1" />                        </div>                                                {{/if}}                          <div class="social-buttons">                            {{#if googleEnabled}}                            "},{"text":""},{"type":"link","data":"[[[skcomponent###c2tjb21wb25lbnQgInNrSURQIiAgaWRwQ29ubmVjdG9yPSJjM2U2YTE2NGJkZTEwNzk1NGU5M2Y1YzA5ZjBjOGJjZSIgaWRlbnRpdHlQcm92aWRlcklkPSIxZTlmZjVmYi0zZjU3LTQ0ZDEtOWM1OS00YzVjM2Y0OWUwYzciIGlkZW50aXR5UHJvdmlkZXJJZEVudHJ5PSIiIGNyZWF0ZVAxVXNlcj0idHJ1ZSIgcG9wdWxhdGlvbklkPSJiOGYwMGQzNS02OTI4LTQ0ZDUtYjlhZC1hN2ZkYWY1NGY0OWQiIHBvcHVsYXRpb25JZEVudHJ5PSIiIHJldHVyblVybD0iIiBpZGVudGl0eVByb3ZpZGVyVHlwZT0iR09PR0xFIiBsYWJlbD0iIiBpZD0iIiBjbGFzcz0iIiBidXR0b25JbWFnZT0iIiBidXR0b25JbWFnZUNsYXNzPSIiIGJ1dHRvbkltYWdlUGxhY2VtZW50PSIi###eyJuYW1lIjoic2tJRFAiLCJvcHRpb25zIjp7ImlkcENvbm5lY3RvciI6ImMzZTZhMTY0YmRlMTA3OTU0ZTkzZjVjMDlmMGM4YmNlIiwiaWRlbnRpdHlQcm92aWRlcklkIjoiMWU5ZmY1ZmItM2Y1Ny00NGQxLTljNTktNGM1YzNmNDllMGM3IiwiaWRlbnRpdHlQcm92aWRlcklkRW50cnkiOiIiLCJjcmVhdGVQMVVzZXIiOnRydWUsInBvcHVsYXRpb25JZCI6ImI4ZjAwZDM1LTY5MjgtNDRkNS1iOWFkLWE3ZmRhZjU0ZjQ5ZCIsInBvcHVsYXRpb25JZEVudHJ5IjoiIiwicmV0dXJuVXJsIjoiIiwiaWRlbnRpdHlQcm92aWRlclR5cGUiOiJHT09HTEUiLCJsYWJlbCI6IiIsImlkIjoiIiwiY2xhc3MiOiIiLCJidXR0b25JbWFnZSI6IiIsImJ1dHRvbkltYWdlQ2xhc3MiOiIiLCJidXR0b25JbWFnZVBsYWNlbWVudCI6IiJ9LCJjb21wb25lbnRQcm9wcyI6eyJpZHBDb25uZWN0b3IiOnsibmFtZSI6ImlkcENvbm5lY3RvciIsImRpc3BsYXlOYW1lIjoiSWRlbnRpdHkgUHJvdmlkZXIgQ29ubmVjdG9yIiwidHlwZSI6ImlkcERyb3Bkb3duIiwiaW5mbyI6IlNlbGVjdCBhbiBpZGVudGl0eSBwcm92aWRlciBjb25uZWN0b3IuIn0sImlkZW50aXR5UHJvdmlkZXJJZCI6eyJuYW1lIjoiaWRlbnRpdHlQcm92aWRlcklkIiwiZGlzcGxheU5hbWUiOiJQaW5nT25lIEV4dGVybmFsIElkZW50aXR5IFByb3ZpZGVyIiwidHlwZSI6ImlkZW50aXR5UHJvdmlkZXJJZCIsImNhdGVnb3J5IjoiZXh0ZXJuYWxDb25uZWN0b3IiLCJpbmZvIjoiU2VsZWN0IGFuIGV4dGVybmFsIGlkZW50aXR5IHByb3ZpZGVyIGZyb20geW91ciBQaW5nT25lIGVudmlyb25tZW50LiJ9LCJpZGVudGl0eVByb3ZpZGVySWRFbnRyeSI6eyJuYW1lIjoiaWRlbnRpdHlQcm92aWRlcklkRW50cnkiLCJkaXNwbGF5TmFtZSI6IlBpbmdPbmUgRXh0ZXJuYWwgSWRlbnRpdHkgUHJvdmlkZXIgSUQiLCJ0eXBlIjoiaWRlbnRpdHlQcm92aWRlcklkRW50cnkiLCJjYXRlZ29yeSI6ImV4dGVybmFsQ29ubmVjdG9yIiwiaW5mbyI6IlRoZSBJRCBvZiBhbiBleHRlcm5hbCBpZGVudGl0eSBwcm92aWRlciBmcm9tIHlvdXIgUGluZ09uZSBlbnZpcm9ubWVudCwgc3VjaCBhcyAnZGY0MTczNTUtYWRjNC0yODQ2LTQxZjEtNmY0YjBiOWJkMTJjJy4ifSwiY3JlYXRlUDFVc2VyIjp7Im5hbWUiOiJjcmVhdGVQMVVzZXIiLCJkaXNwbGF5TmFtZSI6Ikxpbmsgd2l0aCBQaW5nT25lIFVzZXIiLCJ0eXBlIjoiY3JlYXRlUDFVc2VyIiwiY2F0ZWdvcnkiOiJleHRlcm5hbENvbm5lY3RvciIsImluZm8iOiJXaGVuIGVuYWJsZWQsIERhVmluY2kgY3JlYXRlcyBvciB1cGRhdGVzIGEgbGlua2VkIFBpbmdPbmUgdXNlciBhY2NvdW50IHVzaW5nIGF0dHJpYnV0ZXMgZnJvbSB0aGUgZXh0ZXJuYWwgSWRQLiJ9LCJwb3B1bGF0aW9uSWQiOnsibmFtZSI6InBvcHVsYXRpb25JZCIsImRpc3BsYXlOYW1lIjoiUGluZ09uZSBQb3B1bGF0aW9uIiwidHlwZSI6InBvcHVsYXRpb25JZCIsImNhdGVnb3J5IjoiZXh0ZXJuYWxDb25uZWN0b3IiLCJpbmZvIjoiVGhlIFBpbmdPbmUgcG9wdWxhdGlvbiB0byB1c2Ugd2hlbiBhdXRoZW50aWNhdGluZyB0aGUgdXNlci4ifSwicG9wdWxhdGlvbklkRW50cnkiOnsibmFtZSI6InBvcHVsYXRpb25JZEVudHJ5IiwiZGlzcGxheU5hbWUiOiJQb3B1bGF0aW9uIElEIiwidHlwZSI6InBvcHVsYXRpb25JZEVudHJ5IiwiY2F0ZWdvcnkiOiJleHRlcm5hbENvbm5lY3RvciIsImluZm8iOiJUaGUgSUQgb2YgdGhlIFBpbmdPbmUgcG9wdWxhdGlvbiB0byB1c2Ugd2hlbiBhdXRoZW50aWNhdGluZyB0aGUgdXNlciwgc3VjaCBhcyAnYWE0YjNlODEtY2Y3ZS04Njg1LTRiN2ItN2VjODljZmNmN2M4Jy4ifSwicmV0dXJuVXJsIjp7Im5hbWUiOiJyZXR1cm5VcmwiLCJkaXNwbGF5TmFtZSI6IlJldHVybiBVUkwiLCJ0eXBlIjoicmV0dXJuVXJsIiwiY2F0ZWdvcnkiOiJleHRlcm5hbENvbm5lY3RvciIsImluZm8iOiJVUkwgb2YgYW4gYXBwbGljYXRpb24gdG8gZ28gYmFjayB0byBjb250aW51ZSB3aXRoIHRoZSBmbG93LiJ9LCJpZGVudGl0eVByb3ZpZGVyVHlwZSI6eyJuYW1lIjoiaWRlbnRpdHlQcm92aWRlclR5cGUiLCJkaXNwbGF5TmFtZSI6IklkZW50aXR5IFByb3ZpZGVyIFR5cGUiLCJ0eXBlIjoiaWRlbnRpdHlQcm92aWRlclR5cGUiLCJjYXRlZ29yeSI6ImV4dGVybmFsQ29ubmVjdG9yIn0sImxhYmVsIjp7Im5hbWUiOiJsYWJlbCIsImRpc3BsYXlOYW1lIjoiQnV0dG9uIFRleHQiLCJpbmZvIjoiVGhlIHRleHQgdG8gc2hvdyBvbiB0aGUgYnV0dG9uLCBzdWNoIGFzICdTaWduIG9uIHdpdGggTWljcm9zb2Z0Jy4ifSwiaWQiOnsibmFtZSI6ImlkIiwiZGlzcGxheU5hbWUiOiJCdXR0b24gSUQiLCJpbmZvIjoiVGhlIHVuaXF1ZSBJRCB0byBpbmNsdWRlIGluIHRoZSBidXR0b24gSFRNTC4gVGhpcyBhbGxvd3MgeW91IHRvIHVzZSB0aGUgJ2RhdGEtc2tidXR0b25pZCcgdmFsdWUgdG8gaWRlbnRpZnkgdGhlIGJ1dHRvbiBpbiB5b3VyIGN1c3RvbSBDU1Mgb3IgSmF2YVNjcmlwdC4ifSwiY2xhc3MiOnsibmFtZSI6ImNsYXNzIiwiZGlzcGxheU5hbWUiOiJCdXR0b24gQ1NTIENsYXNzIiwiaW5mbyI6IlRoZSBDU1MgY2xhc3MgdG8gaW5jbHVkZSBpbiB0aGUgYnV0dG9uIEhUTUwuIFRoaXMgYWxsb3dzIHlvdSB0byBpZGVudGlmeSB0aGUgYnV0dG9uIGluIHlvdXIgY3VzdG9tIENTUyJ9LCJidXR0b25JbWFnZSI6eyJuYW1lIjoiYnV0dG9uSW1hZ2UiLCJkaXNwbGF5TmFtZSI6IkltYWdlIFVSTCIsImdyb3VwIjoiSW1hZ2UiLCJ0eXBlIjoiYnV0dG9uSW1hZ2UiLCJpbmZvIjoiVGhlIFVSTCBmb3IgdGhlIGltYWdlIHRoYXQgeW91IHdhbnQgdG8gdXNlIGZvciB0aGUgYnV0dG9uLCBzdWNoIGFzICdodHRwczovL2V4YW1wbGUuY29tL2ltZy9zaWdub24ucG5nJy4ifSwiYnV0dG9uSW1hZ2VDbGFzcyI6eyJuYW1lIjoiYnV0dG9uSW1hZ2VDbGFzcyIsImRpc3BsYXlOYW1lIjoiSW1hZ2UgQ1NTIENsYXNzIiwiZ3JvdXAiOiJJbWFnZSIsImluZm8iOiJUaGUgQ1NTIGNsYXNzIHRvIGluY2x1ZGUgaW4gdGhlIGJ1dHRvbiBpbWFnZSBIVE1MLiBUaGlzIGFsbG93cyB5b3UgdG8gaWRlbnRpZnkgdGhlIGltYWdlIGluIHlvdXIgY3VzdG9tIENTUy4ifSwiYnV0dG9uSW1hZ2VQbGFjZW1lbnQiOnsibmFtZSI6ImJ1dHRvbkltYWdlUGxhY2VtZW50IiwiZGlzcGxheU5hbWUiOiJJbWFnZSBQbGFjZW1lbnQiLCJ0eXBlIjoic2VsZWN0Iiwib3B0aW9ucyI6W3sibmFtZSI6IkxlZnQiLCJ2YWx1ZSI6ImxlZnQifSx7Im5hbWUiOiJSaWdodCIsInZhbHVlIjoicmlnaHQifV0sImdyb3VwIjoiSW1hZ2UiLCJpbmZvIjoiQWxpZ24gdGhlIGltYWdlIHRvIHRoZSBsZWZ0IG9yIHJpZ2h0IHNpZGUgb2YgdGhlIGJ1dHRvbi4ifX19]]]","src":"auth.svg","url":"skIDP","children":[{"text":"skIDP"}],"component":"skIDP","options":{"idpConnector":"c3e6a164bde107954e93f5c09f0c8bce","identityProviderId":"1e9ff5fb-3f57-44d1-9c59-4c5c3f49e0c7","identityProviderIdEntry":"","createP1User":true,"populationId":"b8f00d35-6928-44d5-b9ad-a7fdaf54f49d","populationIdEntry":"","returnUrl":"","identityProviderType":"GOOGLE","label":"","id":"","class":"","buttonImage":"","buttonImageClass":"","buttonImagePlacement":""},"componentProps":{"idpConnector":{"name":"idpConnector","displayName":"Identity Provider Connector","type":"idpDropdown","info":"Select an identity provider connector."},"identityProviderId":{"name":"identityProviderId","displayName":"PingOne External Identity Provider","type":"identityProviderId","category":"externalConnector","info":"Select an external identity provider from your PingOne environment."},"identityProviderIdEntry":{"name":"identityProviderIdEntry","displayName":"PingOne External Identity Provider ID","type":"identityProviderIdEntry","category":"externalConnector","info":"The ID of an external identity provider from your PingOne environment, such as &#39;df417355-adc4-2846-41f1-6f4b0b9bd12c&#39;."},"createP1User":{"name":"createP1User","displayName":"Link with PingOne User","type":"createP1User","category":"externalConnector","info":"When enabled, DaVinci creates or updates a linked PingOne user account using attributes from the external IdP."},"populationId":{"name":"populationId","displayName":"PingOne Population","type":"populationId","category":"externalConnector","info":"The PingOne population to use when authenticating the user."},"populationIdEntry":{"name":"populationIdEntry","displayName":"Population ID","type":"populationIdEntry","category":"externalConnector","info":"The ID of the PingOne population to use when authenticating the user, such as &#39;aa4b3e81-cf7e-8685-4b7b-7ec89cfcf7c8&#39;."},"returnUrl":{"name":"returnUrl","displayName":"Return URL","type":"returnUrl","category":"externalConnector","info":"URL of an application to go back to continue with the flow."},"identityProviderType":{"name":"identityProviderType","displayName":"Identity Provider Type","type":"identityProviderType","category":"externalConnector"},"label":{"name":"label","displayName":"Button Text","info":"The text to show on the button, such as &#39;Sign on with Microsoft&#39;."},"id":{"name":"id","displayName":"Button ID","info":"The unique ID to include in the button HTML. This allows you to use the &#39;data-skbuttonid&#39; value to identify the button in your custom CSS or JavaScript."},"class":{"name":"class","displayName":"Button CSS Class","info":"The CSS class to include in the button HTML. This allows you to identify the button in your custom CSS"},"buttonImage":{"name":"buttonImage","displayName":"Image URL","group":"Image","type":"buttonImage","info":"The URL for the image that you want to use for the button, such as &#39;https://example.com/img/signon.png&#39;."},"buttonImageClass":{"name":"buttonImageClass","displayName":"Image CSS Class","group":"Image","info":"The CSS class to include in the button image HTML. This allows you to identify the image in your custom CSS."},"buttonImagePlacement":{"name":"buttonImagePlacement","displayName":"Image Placement","type":"select","options":[{"name":"Left","value":"left"},{"name":"Right","value":"right"}],"group":"Image","info":"Align the image to the left or right side of the button."}},"tooltip":"{{component.skIDP}}"},{"text":""},{"text":"                            {{/if}}                            {{#if facebookEnabled}}                            "},{"text":""},{"type":"link","data":"[[[skcomponent###c2tjb21wb25lbnQgInNrSURQIiAgaWRwQ29ubmVjdG9yPSJjM2U2YTE2NGJkZTEwNzk1NGU5M2Y1YzA5ZjBjOGJjZSIgaWRlbnRpdHlQcm92aWRlcklkPSJhMWZhM2U0Ny03NmY5LTRkM2ItOTVlYy0yODhhMWQ0Njg3ZmQiIGlkZW50aXR5UHJvdmlkZXJJZEVudHJ5PSIiIGNyZWF0ZVAxVXNlcj0idHJ1ZSIgcG9wdWxhdGlvbklkPSJiOGYwMGQzNS02OTI4LTQ0ZDUtYjlhZC1hN2ZkYWY1NGY0OWQiIHBvcHVsYXRpb25JZEVudHJ5PSIiIHJldHVyblVybD0iIiBpZGVudGl0eVByb3ZpZGVyVHlwZT0iRkFDRUJPT0siIGxhYmVsPSIiIGlkPSIiIGNsYXNzPSIiIGJ1dHRvbkltYWdlPSIiIGJ1dHRvbkltYWdlQ2xhc3M9IiIgYnV0dG9uSW1hZ2VQbGFjZW1lbnQ9IiI=###eyJuYW1lIjoic2tJRFAiLCJvcHRpb25zIjp7ImlkcENvbm5lY3RvciI6ImMzZTZhMTY0YmRlMTA3OTU0ZTkzZjVjMDlmMGM4YmNlIiwiaWRlbnRpdHlQcm92aWRlcklkIjoiYTFmYTNlNDctNzZmOS00ZDNiLTk1ZWMtMjg4YTFkNDY4N2ZkIiwiaWRlbnRpdHlQcm92aWRlcklkRW50cnkiOiIiLCJjcmVhdGVQMVVzZXIiOnRydWUsInBvcHVsYXRpb25JZCI6ImI4ZjAwZDM1LTY5MjgtNDRkNS1iOWFkLWE3ZmRhZjU0ZjQ5ZCIsInBvcHVsYXRpb25JZEVudHJ5IjoiIiwicmV0dXJuVXJsIjoiIiwiaWRlbnRpdHlQcm92aWRlclR5cGUiOiJGQUNFQk9PSyIsImxhYmVsIjoiIiwiaWQiOiIiLCJjbGFzcyI6IiIsImJ1dHRvbkltYWdlIjoiIiwiYnV0dG9uSW1hZ2VDbGFzcyI6IiIsImJ1dHRvbkltYWdlUGxhY2VtZW50IjoiIn0sImNvbXBvbmVudFByb3BzIjp7ImlkcENvbm5lY3RvciI6eyJuYW1lIjoiaWRwQ29ubmVjdG9yIiwiZGlzcGxheU5hbWUiOiJJZGVudGl0eSBQcm92aWRlciBDb25uZWN0b3IiLCJ0eXBlIjoiaWRwRHJvcGRvd24iLCJpbmZvIjoiU2VsZWN0IGFuIGlkZW50aXR5IHByb3ZpZGVyIGNvbm5lY3Rvci4ifSwiaWRlbnRpdHlQcm92aWRlcklkIjp7Im5hbWUiOiJpZGVudGl0eVByb3ZpZGVySWQiLCJkaXNwbGF5TmFtZSI6IlBpbmdPbmUgRXh0ZXJuYWwgSWRlbnRpdHkgUHJvdmlkZXIiLCJ0eXBlIjoiaWRlbnRpdHlQcm92aWRlcklkIiwiY2F0ZWdvcnkiOiJleHRlcm5hbENvbm5lY3RvciIsImluZm8iOiJTZWxlY3QgYW4gZXh0ZXJuYWwgaWRlbnRpdHkgcHJvdmlkZXIgZnJvbSB5b3VyIFBpbmdPbmUgZW52aXJvbm1lbnQuIn0sImlkZW50aXR5UHJvdmlkZXJJZEVudHJ5Ijp7Im5hbWUiOiJpZGVudGl0eVByb3ZpZGVySWRFbnRyeSIsImRpc3BsYXlOYW1lIjoiUGluZ09uZSBFeHRlcm5hbCBJZGVudGl0eSBQcm92aWRlciBJRCIsInR5cGUiOiJpZGVudGl0eVByb3ZpZGVySWRFbnRyeSIsImNhdGVnb3J5IjoiZXh0ZXJuYWxDb25uZWN0b3IiLCJpbmZvIjoiVGhlIElEIG9mIGFuIGV4dGVybmFsIGlkZW50aXR5IHByb3ZpZGVyIGZyb20geW91ciBQaW5nT25lIGVudmlyb25tZW50LCBzdWNoIGFzICdkZjQxNzM1NS1hZGM0LTI4NDYtNDFmMS02ZjRiMGI5YmQxMmMnLiJ9LCJjcmVhdGVQMVVzZXIiOnsibmFtZSI6ImNyZWF0ZVAxVXNlciIsImRpc3BsYXlOYW1lIjoiTGluayB3aXRoIFBpbmdPbmUgVXNlciIsInR5cGUiOiJjcmVhdGVQMVVzZXIiLCJjYXRlZ29yeSI6ImV4dGVybmFsQ29ubmVjdG9yIiwiaW5mbyI6IldoZW4gZW5hYmxlZCwgRGFWaW5jaSBjcmVhdGVzIG9yIHVwZGF0ZXMgYSBsaW5rZWQgUGluZ09uZSB1c2VyIGFjY291bnQgdXNpbmcgYXR0cmlidXRlcyBmcm9tIHRoZSBleHRlcm5hbCBJZFAuIn0sInBvcHVsYXRpb25JZCI6eyJuYW1lIjoicG9wdWxhdGlvbklkIiwiZGlzcGxheU5hbWUiOiJQaW5nT25lIFBvcHVsYXRpb24iLCJ0eXBlIjoicG9wdWxhdGlvbklkIiwiY2F0ZWdvcnkiOiJleHRlcm5hbENvbm5lY3RvciIsImluZm8iOiJUaGUgUGluZ09uZSBwb3B1bGF0aW9uIHRvIHVzZSB3aGVuIGF1dGhlbnRpY2F0aW5nIHRoZSB1c2VyLiJ9LCJwb3B1bGF0aW9uSWRFbnRyeSI6eyJuYW1lIjoicG9wdWxhdGlvbklkRW50cnkiLCJkaXNwbGF5TmFtZSI6IlBvcHVsYXRpb24gSUQiLCJ0eXBlIjoicG9wdWxhdGlvbklkRW50cnkiLCJjYXRlZ29yeSI6ImV4dGVybmFsQ29ubmVjdG9yIiwiaW5mbyI6IlRoZSBJRCBvZiB0aGUgUGluZ09uZSBwb3B1bGF0aW9uIHRvIHVzZSB3aGVuIGF1dGhlbnRpY2F0aW5nIHRoZSB1c2VyLCBzdWNoIGFzICdhYTRiM2U4MS1jZjdlLTg2ODUtNGI3Yi03ZWM4OWNmY2Y3YzgnLiJ9LCJyZXR1cm5VcmwiOnsibmFtZSI6InJldHVyblVybCIsImRpc3BsYXlOYW1lIjoiUmV0dXJuIFVSTCIsInR5cGUiOiJyZXR1cm5VcmwiLCJjYXRlZ29yeSI6ImV4dGVybmFsQ29ubmVjdG9yIiwiaW5mbyI6IlVSTCBvZiBhbiBhcHBsaWNhdGlvbiB0byBnbyBiYWNrIHRvIGNvbnRpbnVlIHdpdGggdGhlIGZsb3cuIn0sImlkZW50aXR5UHJvdmlkZXJUeXBlIjp7Im5hbWUiOiJpZGVudGl0eVByb3ZpZGVyVHlwZSIsImRpc3BsYXlOYW1lIjoiSWRlbnRpdHkgUHJvdmlkZXIgVHlwZSIsInR5cGUiOiJpZGVudGl0eVByb3ZpZGVyVHlwZSIsImNhdGVnb3J5IjoiZXh0ZXJuYWxDb25uZWN0b3IifSwibGFiZWwiOnsibmFtZSI6ImxhYmVsIiwiZGlzcGxheU5hbWUiOiJCdXR0b24gVGV4dCIsImluZm8iOiJUaGUgdGV4dCB0byBzaG93IG9uIHRoZSBidXR0b24sIHN1Y2ggYXMgJ1NpZ24gb24gd2l0aCBNaWNyb3NvZnQnLiJ9LCJpZCI6eyJuYW1lIjoiaWQiLCJkaXNwbGF5TmFtZSI6IkJ1dHRvbiBJRCIsImluZm8iOiJUaGUgdW5pcXVlIElEIHRvIGluY2x1ZGUgaW4gdGhlIGJ1dHRvbiBIVE1MLiBUaGlzIGFsbG93cyB5b3UgdG8gdXNlIHRoZSAnZGF0YS1za2J1dHRvbmlkJyB2YWx1ZSB0byBpZGVudGlmeSB0aGUgYnV0dG9uIGluIHlvdXIgY3VzdG9tIENTUyBvciBKYXZhU2NyaXB0LiJ9LCJjbGFzcyI6eyJuYW1lIjoiY2xhc3MiLCJkaXNwbGF5TmFtZSI6IkJ1dHRvbiBDU1MgQ2xhc3MiLCJpbmZvIjoiVGhlIENTUyBjbGFzcyB0byBpbmNsdWRlIGluIHRoZSBidXR0b24gSFRNTC4gVGhpcyBhbGxvd3MgeW91IHRvIGlkZW50aWZ5IHRoZSBidXR0b24gaW4geW91ciBjdXN0b20gQ1NTIn0sImJ1dHRvbkltYWdlIjp7Im5hbWUiOiJidXR0b25JbWFnZSIsImRpc3BsYXlOYW1lIjoiSW1hZ2UgVVJMIiwiZ3JvdXAiOiJJbWFnZSIsInR5cGUiOiJidXR0b25JbWFnZSIsImluZm8iOiJUaGUgVVJMIGZvciB0aGUgaW1hZ2UgdGhhdCB5b3Ugd2FudCB0byB1c2UgZm9yIHRoZSBidXR0b24sIHN1Y2ggYXMgJ2h0dHBzOi8vZXhhbXBsZS5jb20vaW1nL3NpZ25vbi5wbmcnLiJ9LCJidXR0b25JbWFnZUNsYXNzIjp7Im5hbWUiOiJidXR0b25JbWFnZUNsYXNzIiwiZGlzcGxheU5hbWUiOiJJbWFnZSBDU1MgQ2xhc3MiLCJncm91cCI6IkltYWdlIiwiaW5mbyI6IlRoZSBDU1MgY2xhc3MgdG8gaW5jbHVkZSBpbiB0aGUgYnV0dG9uIGltYWdlIEhUTUwuIFRoaXMgYWxsb3dzIHlvdSB0byBpZGVudGlmeSB0aGUgaW1hZ2UgaW4geW91ciBjdXN0b20gQ1NTLiJ9LCJidXR0b25JbWFnZVBsYWNlbWVudCI6eyJuYW1lIjoiYnV0dG9uSW1hZ2VQbGFjZW1lbnQiLCJkaXNwbGF5TmFtZSI6IkltYWdlIFBsYWNlbWVudCIsInR5cGUiOiJzZWxlY3QiLCJvcHRpb25zIjpbeyJuYW1lIjoiTGVmdCIsInZhbHVlIjoibGVmdCJ9LHsibmFtZSI6IlJpZ2h0IiwidmFsdWUiOiJyaWdodCJ9XSwiZ3JvdXAiOiJJbWFnZSIsImluZm8iOiJBbGlnbiB0aGUgaW1hZ2UgdG8gdGhlIGxlZnQgb3IgcmlnaHQgc2lkZSBvZiB0aGUgYnV0dG9uLiJ9fX0=]]]","src":"auth.svg","url":"skIDP","children":[{"text":"skIDP"}],"component":"skIDP","options":{"idpConnector":"c3e6a164bde107954e93f5c09f0c8bce","identityProviderId":"a1fa3e47-76f9-4d3b-95ec-288a1d4687fd","identityProviderIdEntry":"","createP1User":true,"populationId":"b8f00d35-6928-44d5-b9ad-a7fdaf54f49d","populationIdEntry":"","returnUrl":"","identityProviderType":"FACEBOOK","label":"","id":"","class":"","buttonImage":"","buttonImageClass":"","buttonImagePlacement":""},"componentProps":{"idpConnector":{"name":"idpConnector","displayName":"Identity Provider Connector","type":"idpDropdown","info":"Select an identity provider connector."},"identityProviderId":{"name":"identityProviderId","displayName":"PingOne External Identity Provider","type":"identityProviderId","category":"externalConnector","info":"Select an external identity provider from your PingOne environment."},"identityProviderIdEntry":{"name":"identityProviderIdEntry","displayName":"PingOne External Identity Provider ID","type":"identityProviderIdEntry","category":"externalConnector","info":"The ID of an external identity provider from your PingOne environment, such as &#39;df417355-adc4-2846-41f1-6f4b0b9bd12c&#39;."},"createP1User":{"name":"createP1User","displayName":"Link with PingOne User","type":"createP1User","category":"externalConnector","info":"When enabled, DaVinci creates or updates a linked PingOne user account using attributes from the external IdP."},"populationId":{"name":"populationId","displayName":"PingOne Population","type":"populationId","category":"externalConnector","info":"The PingOne population to use when authenticating the user."},"populationIdEntry":{"name":"populationIdEntry","displayName":"Population ID","type":"populationIdEntry","category":"externalConnector","info":"The ID of the PingOne population to use when authenticating the user, such as &#39;aa4b3e81-cf7e-8685-4b7b-7ec89cfcf7c8&#39;."},"returnUrl":{"name":"returnUrl","displayName":"Return URL","type":"returnUrl","category":"externalConnector","info":"URL of an application to go back to continue with the flow."},"identityProviderType":{"name":"identityProviderType","displayName":"Identity Provider Type","type":"identityProviderType","category":"externalConnector"},"label":{"name":"label","displayName":"Button Text","info":"The text to show on the button, such as &#39;Sign on with Microsoft&#39;."},"id":{"name":"id","displayName":"Button ID","info":"The unique ID to include in the button HTML. This allows you to use the &#39;data-skbuttonid&#39; value to identify the button in your custom CSS or JavaScript."},"class":{"name":"class","displayName":"Button CSS Class","info":"The CSS class to include in the button HTML. This allows you to identify the button in your custom CSS"},"buttonImage":{"name":"buttonImage","displayName":"Image URL","group":"Image","type":"buttonImage","info":"The URL for the image that you want to use for the button, such as &#39;https://example.com/img/signon.png&#39;."},"buttonImageClass":{"name":"buttonImageClass","displayName":"Image CSS Class","group":"Image","info":"The CSS class to include in the button image HTML. This allows you to identify the image in your custom CSS."},"buttonImagePlacement":{"name":"buttonImagePlacement","displayName":"Image Placement","type":"select","options":[{"name":"Left","value":"left"},{"name":"Right","value":"right"}],"group":"Image","info":"Align the image to the left or right side of the button."}},"tooltip":"{{component.skIDP}}"},{"text":""},{"text":"                            {{/if}}                            {{#if appleEnabled}}                            "},{"text":""},{"type":"link","data":"[[[skcomponent###c2tjb21wb25lbnQgInNrSURQIiAgaWRwQ29ubmVjdG9yPSJjM2U2YTE2NGJkZTEwNzk1NGU5M2Y1YzA5ZjBjOGJjZSIgaWRlbnRpdHlQcm92aWRlcklkPSJmZmZlM2EyNS1lNTcyLTRlMWItYWJmNy0xMDY3Y2FkMTY4OGUiIGlkZW50aXR5UHJvdmlkZXJJZEVudHJ5PSIiIGNyZWF0ZVAxVXNlcj0idHJ1ZSIgcG9wdWxhdGlvbklkPSJiOGYwMGQzNS02OTI4LTQ0ZDUtYjlhZC1hN2ZkYWY1NGY0OWQiIHBvcHVsYXRpb25JZEVudHJ5PSIiIHJldHVyblVybD0iIiBpZGVudGl0eVByb3ZpZGVyVHlwZT0iQVBQTEUiIGxhYmVsPSIiIGlkPSIiIGNsYXNzPSIiIGJ1dHRvbkltYWdlPSIiIGJ1dHRvbkltYWdlQ2xhc3M9IiIgYnV0dG9uSW1hZ2VQbGFjZW1lbnQ9IiI=###eyJuYW1lIjoic2tJRFAiLCJvcHRpb25zIjp7ImlkcENvbm5lY3RvciI6ImMzZTZhMTY0YmRlMTA3OTU0ZTkzZjVjMDlmMGM4YmNlIiwiaWRlbnRpdHlQcm92aWRlcklkIjoiZmZmZTNhMjUtZTU3Mi00ZTFiLWFiZjctMTA2N2NhZDE2ODhlIiwiaWRlbnRpdHlQcm92aWRlcklkRW50cnkiOiIiLCJjcmVhdGVQMVVzZXIiOnRydWUsInBvcHVsYXRpb25JZCI6ImI4ZjAwZDM1LTY5MjgtNDRkNS1iOWFkLWE3ZmRhZjU0ZjQ5ZCIsInBvcHVsYXRpb25JZEVudHJ5IjoiIiwicmV0dXJuVXJsIjoiIiwiaWRlbnRpdHlQcm92aWRlclR5cGUiOiJBUFBMRSIsImxhYmVsIjoiIiwiaWQiOiIiLCJjbGFzcyI6IiIsImJ1dHRvbkltYWdlIjoiIiwiYnV0dG9uSW1hZ2VDbGFzcyI6IiIsImJ1dHRvbkltYWdlUGxhY2VtZW50IjoiIn0sImNvbXBvbmVudFByb3BzIjp7ImlkcENvbm5lY3RvciI6eyJuYW1lIjoiaWRwQ29ubmVjdG9yIiwiZGlzcGxheU5hbWUiOiJJZGVudGl0eSBQcm92aWRlciBDb25uZWN0b3IiLCJ0eXBlIjoiaWRwRHJvcGRvd24iLCJpbmZvIjoiU2VsZWN0IGFuIGlkZW50aXR5IHByb3ZpZGVyIGNvbm5lY3Rvci4ifSwiaWRlbnRpdHlQcm92aWRlcklkIjp7Im5hbWUiOiJpZGVudGl0eVByb3ZpZGVySWQiLCJkaXNwbGF5TmFtZSI6IlBpbmdPbmUgRXh0ZXJuYWwgSWRlbnRpdHkgUHJvdmlkZXIiLCJ0eXBlIjoiaWRlbnRpdHlQcm92aWRlcklkIiwiY2F0ZWdvcnkiOiJleHRlcm5hbENvbm5lY3RvciIsImluZm8iOiJTZWxlY3QgYW4gZXh0ZXJuYWwgaWRlbnRpdHkgcHJvdmlkZXIgZnJvbSB5b3VyIFBpbmdPbmUgZW52aXJvbm1lbnQuIn0sImlkZW50aXR5UHJvdmlkZXJJZEVudHJ5Ijp7Im5hbWUiOiJpZGVudGl0eVByb3ZpZGVySWRFbnRyeSIsImRpc3BsYXlOYW1lIjoiUGluZ09uZSBFeHRlcm5hbCBJZGVudGl0eSBQcm92aWRlciBJRCIsInR5cGUiOiJpZGVudGl0eVByb3ZpZGVySWRFbnRyeSIsImNhdGVnb3J5IjoiZXh0ZXJuYWxDb25uZWN0b3IiLCJpbmZvIjoiVGhlIElEIG9mIGFuIGV4dGVybmFsIGlkZW50aXR5IHByb3ZpZGVyIGZyb20geW91ciBQaW5nT25lIGVudmlyb25tZW50LCBzdWNoIGFzICdkZjQxNzM1NS1hZGM0LTI4NDYtNDFmMS02ZjRiMGI5YmQxMmMnLiJ9LCJjcmVhdGVQMVVzZXIiOnsibmFtZSI6ImNyZWF0ZVAxVXNlciIsImRpc3BsYXlOYW1lIjoiTGluayB3aXRoIFBpbmdPbmUgVXNlciIsInR5cGUiOiJjcmVhdGVQMVVzZXIiLCJjYXRlZ29yeSI6ImV4dGVybmFsQ29ubmVjdG9yIiwiaW5mbyI6IldoZW4gZW5hYmxlZCwgRGFWaW5jaSBjcmVhdGVzIG9yIHVwZGF0ZXMgYSBsaW5rZWQgUGluZ09uZSB1c2VyIGFjY291bnQgdXNpbmcgYXR0cmlidXRlcyBmcm9tIHRoZSBleHRlcm5hbCBJZFAuIn0sInBvcHVsYXRpb25JZCI6eyJuYW1lIjoicG9wdWxhdGlvbklkIiwiZGlzcGxheU5hbWUiOiJQaW5nT25lIFBvcHVsYXRpb24iLCJ0eXBlIjoicG9wdWxhdGlvbklkIiwiY2F0ZWdvcnkiOiJleHRlcm5hbENvbm5lY3RvciIsImluZm8iOiJUaGUgUGluZ09uZSBwb3B1bGF0aW9uIHRvIHVzZSB3aGVuIGF1dGhlbnRpY2F0aW5nIHRoZSB1c2VyLiJ9LCJwb3B1bGF0aW9uSWRFbnRyeSI6eyJuYW1lIjoicG9wdWxhdGlvbklkRW50cnkiLCJkaXNwbGF5TmFtZSI6IlBvcHVsYXRpb24gSUQiLCJ0eXBlIjoicG9wdWxhdGlvbklkRW50cnkiLCJjYXRlZ29yeSI6ImV4dGVybmFsQ29ubmVjdG9yIiwiaW5mbyI6IlRoZSBJRCBvZiB0aGUgUGluZ09uZSBwb3B1bGF0aW9uIHRvIHVzZSB3aGVuIGF1dGhlbnRpY2F0aW5nIHRoZSB1c2VyLCBzdWNoIGFzICdhYTRiM2U4MS1jZjdlLTg2ODUtNGI3Yi03ZWM4OWNmY2Y3YzgnLiJ9LCJyZXR1cm5VcmwiOnsibmFtZSI6InJldHVyblVybCIsImRpc3BsYXlOYW1lIjoiUmV0dXJuIFVSTCIsInR5cGUiOiJyZXR1cm5VcmwiLCJjYXRlZ29yeSI6ImV4dGVybmFsQ29ubmVjdG9yIiwiaW5mbyI6IlVSTCBvZiBhbiBhcHBsaWNhdGlvbiB0byBnbyBiYWNrIHRvIGNvbnRpbnVlIHdpdGggdGhlIGZsb3cuIn0sImlkZW50aXR5UHJvdmlkZXJUeXBlIjp7Im5hbWUiOiJpZGVudGl0eVByb3ZpZGVyVHlwZSIsImRpc3BsYXlOYW1lIjoiSWRlbnRpdHkgUHJvdmlkZXIgVHlwZSIsInR5cGUiOiJpZGVudGl0eVByb3ZpZGVyVHlwZSIsImNhdGVnb3J5IjoiZXh0ZXJuYWxDb25uZWN0b3IifSwibGFiZWwiOnsibmFtZSI6ImxhYmVsIiwiZGlzcGxheU5hbWUiOiJCdXR0b24gVGV4dCIsImluZm8iOiJUaGUgdGV4dCB0byBzaG93IG9uIHRoZSBidXR0b24sIHN1Y2ggYXMgJ1NpZ24gb24gd2l0aCBNaWNyb3NvZnQnLiJ9LCJpZCI6eyJuYW1lIjoiaWQiLCJkaXNwbGF5TmFtZSI6IkJ1dHRvbiBJRCIsImluZm8iOiJUaGUgdW5pcXVlIElEIHRvIGluY2x1ZGUgaW4gdGhlIGJ1dHRvbiBIVE1MLiBUaGlzIGFsbG93cyB5b3UgdG8gdXNlIHRoZSAnZGF0YS1za2J1dHRvbmlkJyB2YWx1ZSB0byBpZGVudGlmeSB0aGUgYnV0dG9uIGluIHlvdXIgY3VzdG9tIENTUyBvciBKYXZhU2NyaXB0LiJ9LCJjbGFzcyI6eyJuYW1lIjoiY2xhc3MiLCJkaXNwbGF5TmFtZSI6IkJ1dHRvbiBDU1MgQ2xhc3MiLCJpbmZvIjoiVGhlIENTUyBjbGFzcyB0byBpbmNsdWRlIGluIHRoZSBidXR0b24gSFRNTC4gVGhpcyBhbGxvd3MgeW91IHRvIGlkZW50aWZ5IHRoZSBidXR0b24gaW4geW91ciBjdXN0b20gQ1NTIn0sImJ1dHRvbkltYWdlIjp7Im5hbWUiOiJidXR0b25JbWFnZSIsImRpc3BsYXlOYW1lIjoiSW1hZ2UgVVJMIiwiZ3JvdXAiOiJJbWFnZSIsInR5cGUiOiJidXR0b25JbWFnZSIsImluZm8iOiJUaGUgVVJMIGZvciB0aGUgaW1hZ2UgdGhhdCB5b3Ugd2FudCB0byB1c2UgZm9yIHRoZSBidXR0b24sIHN1Y2ggYXMgJ2h0dHBzOi8vZXhhbXBsZS5jb20vaW1nL3NpZ25vbi5wbmcnLiJ9LCJidXR0b25JbWFnZUNsYXNzIjp7Im5hbWUiOiJidXR0b25JbWFnZUNsYXNzIiwiZGlzcGxheU5hbWUiOiJJbWFnZSBDU1MgQ2xhc3MiLCJncm91cCI6IkltYWdlIiwiaW5mbyI6IlRoZSBDU1MgY2xhc3MgdG8gaW5jbHVkZSBpbiB0aGUgYnV0dG9uIGltYWdlIEhUTUwuIFRoaXMgYWxsb3dzIHlvdSB0byBpZGVudGlmeSB0aGUgaW1hZ2UgaW4geW91ciBjdXN0b20gQ1NTLiJ9LCJidXR0b25JbWFnZVBsYWNlbWVudCI6eyJuYW1lIjoiYnV0dG9uSW1hZ2VQbGFjZW1lbnQiLCJkaXNwbGF5TmFtZSI6IkltYWdlIFBsYWNlbWVudCIsInR5cGUiOiJzZWxlY3QiLCJvcHRpb25zIjpbeyJuYW1lIjoiTGVmdCIsInZhbHVlIjoibGVmdCJ9LHsibmFtZSI6IlJpZ2h0IiwidmFsdWUiOiJyaWdodCJ9XSwiZ3JvdXAiOiJJbWFnZSIsImluZm8iOiJBbGlnbiB0aGUgaW1hZ2UgdG8gdGhlIGxlZnQgb3IgcmlnaHQgc2lkZSBvZiB0aGUgYnV0dG9uLiJ9fX0=]]]","src":"auth.svg","url":"skIDP","children":[{"text":"skIDP"}],"component":"skIDP","options":{"idpConnector":"c3e6a164bde107954e93f5c09f0c8bce","identityProviderId":"fffe3a25-e572-4e1b-abf7-1067cad1688e","identityProviderIdEntry":"","createP1User":true,"populationId":"b8f00d35-6928-44d5-b9ad-a7fdaf54f49d","populationIdEntry":"","returnUrl":"","identityProviderType":"APPLE","label":"","id":"","class":"","buttonImage":"","buttonImageClass":"","buttonImagePlacement":""},"componentProps":{"idpConnector":{"name":"idpConnector","displayName":"Identity Provider Connector","type":"idpDropdown","info":"Select an identity provider connector."},"identityProviderId":{"name":"identityProviderId","displayName":"PingOne External Identity Provider","type":"identityProviderId","category":"externalConnector","info":"Select an external identity provider from your PingOne environment."},"identityProviderIdEntry":{"name":"identityProviderIdEntry","displayName":"PingOne External Identity Provider ID","type":"identityProviderIdEntry","category":"externalConnector","info":"The ID of an external identity provider from your PingOne environment, such as &#39;df417355-adc4-2846-41f1-6f4b0b9bd12c&#39;."},"createP1User":{"name":"createP1User","displayName":"Link with PingOne User","type":"createP1User","category":"externalConnector","info":"When enabled, DaVinci creates or updates a linked PingOne user account using attributes from the external IdP."},"populationId":{"name":"populationId","displayName":"PingOne Population","type":"populationId","category":"externalConnector","info":"The PingOne population to use when authenticating the user."},"populationIdEntry":{"name":"populationIdEntry","displayName":"Population ID","type":"populationIdEntry","category":"externalConnector","info":"The ID of the PingOne population to use when authenticating the user, such as &#39;aa4b3e81-cf7e-8685-4b7b-7ec89cfcf7c8&#39;."},"returnUrl":{"name":"returnUrl","displayName":"Return URL","type":"returnUrl","category":"externalConnector","info":"URL of an application to go back to continue with the flow."},"identityProviderType":{"name":"identityProviderType","displayName":"Identity Provider Type","type":"identityProviderType","category":"externalConnector"},"label":{"name":"label","displayName":"Button Text","info":"The text to show on the button, such as &#39;Sign on with Microsoft&#39;."},"id":{"name":"id","displayName":"Button ID","info":"The unique ID to include in the button HTML. This allows you to use the &#39;data-skbuttonid&#39; value to identify the button in your custom CSS or JavaScript."},"class":{"name":"class","displayName":"Button CSS Class","info":"The CSS class to include in the button HTML. This allows you to identify the button in your custom CSS"},"buttonImage":{"name":"buttonImage","displayName":"Image URL","group":"Image","type":"buttonImage","info":"The URL for the image that you want to use for the button, such as &#39;https://example.com/img/signon.png&#39;."},"buttonImageClass":{"name":"buttonImageClass","displayName":"Image CSS Class","group":"Image","info":"The CSS class to include in the button image HTML. This allows you to identify the image in your custom CSS."},"buttonImagePlacement":{"name":"buttonImagePlacement","displayName":"Image Placement","type":"select","options":[{"name":"Left","value":"left"},{"name":"Right","value":"right"}],"group":"Image","info":"Align the image to the left or right side of the button."}},"tooltip":"{{component.skIDP}}"},{"text":""},{"text":"                            {{/if}}                        </div>                        <div class="d-flex flex-column">                            {{#if accountRecoveryEnabled}}                            <button type="submit" class="btn btn-link" data-skcomponent="skbutton"                                data-skbuttontype="next-event" data-skform="form" id="btnForget"                                data-skbuttonvalue="FORGET">                                Having trouble signing on?                            </button>                            {{/if}}                            <button type="submit" class="btn btn-link" data-skcomponent="skbutton"                                data-skbuttontype="next-event" data-skform="form" id="btnRegister"                                data-skbuttonvalue="REGISTER">                                No account? Register now!                            </button>                        </div>                    </div>                </form>            </div>        </div>    </div></div>"}]}]
```

## Custom Script
```js 
const focusOnFirstInputElement = () => {
  document.getElementById("email").focus();
};

function start() {
  focusOnFirstInputElement();
}

if (document.readyState === "loading") {
  // Loading hasn&#39;t finished yet
  document.addEventListener("DOMContentLoaded", start);
} else {
  // `DOMContentLoaded` has already fired
  start();
}
```


### Additional Properties
accountRecoveryEnabled
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
        "src": "teleport.svg",
        "url": "flowAccountRecoveryEnabled",
        "data": "{{local.el9cmscetd.payload.output.flowAccountRecoveryEnabled}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowAccountRecoveryEnabled}}",
        "children": [
          {
            "text": "flowAccountRecoveryEnabled"
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


appleEnabled
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
        "src": "teleport.svg",
        "url": "flowAppleEnabled",
        "data": "{{local.el9cmscetd.payload.output.flowAppleEnabled}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowAppleEnabled}}",
        "children": [
          {
            "text": "flowAppleEnabled"
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


externalIdentityProvider
```
```


facebookEnabled
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
        "src": "teleport.svg",
        "url": "flowFacebookEnabled",
        "data": "{{local.el9cmscetd.payload.output.flowFacebookEnabled}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowFacebookEnabled}}",
        "children": [
          {
            "text": "flowFacebookEnabled"
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
```
```


googleEnabled
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
        "src": "teleport.svg",
        "url": "flowGoogleEnabled",
        "data": "{{local.el9cmscetd.payload.output.flowGoogleEnabled}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowGoogleEnabled}}",
        "children": [
          {
            "text": "flowGoogleEnabled"
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


idpList
```string 
skConnectorList
```


inputSchema
```json 
{
	"type": "object",
	"properties": {
		"googleEnabled":{
			"type":"boolean"
		},
		"facebookEnabled":{
			"type":"boolean"
		},
		"appleEnabled":{
			"type":"boolean"
		},
		"socialRegistrationEnabled":{
			"type":"boolean"
		},
		"passwordlessRequired":{
			"type":"boolean"
		},
		"accountRecoveryEnabled":{
			"type":"boolean"
		}
	}
}
```


passwordlessRequired
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
        "src": "teleport.svg",
        "url": "flowPasswordlessRequired",
        "data": "{{local.el9cmscetd.payload.output.flowPasswordlessRequired}}",
        "tooltip": "{{local.el9cmscetd.payload.output.flowPasswordlessRequired}}",
        "children": [
          {
            "text": "flowPasswordlessRequired"
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


socialRegistrationEnabled
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
        "src": "functions.svg",
        "url": "flowSocialRegistrationEnabled",
        "data": "{{local.byomx9u9ci.payload.output.flowSocialRegistrationEnabled}}",
        "tooltip": "{{local.byomx9u9ci.payload.output.flowSocialRegistrationEnabled}}",
        "children": [
          {
            "text": "flowSocialRegistrationEnabled"
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


undefined
```
```


validationRules
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [8epxzybfo](./8epxzybfo.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[59qszmzgg5](./59qszmzgg5.md) | 