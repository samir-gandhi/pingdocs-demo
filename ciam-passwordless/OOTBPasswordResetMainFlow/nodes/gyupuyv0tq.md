# Http - string 
Error Screen
## Configuration
ID:  gyupuyv0tq

Type: CONNECTION 

CapabilityName: customHTMLTemplate



## Custom HTML
```html 
<div
	class="bg-light d-flex flex-column justify-content-center align-items-center position-absolute top-0 start-0 bottom-0 end-0 overflow-auto">
	<div class="mh-100" style="max-width: 400px; width: 100%;">
		<div class="card shadow mb-5">
			<div class="card-body p-5 d-flex flex-column">
				<div class="dialog-content-header dialog-content__header" style="height: 85px"><div class="dialog-content-header__logo"></div></div>
				<h1 class="text-center mb-4">Error</h1>
				<p class="text-muted text-center">
					{{local.qwwhmi6a6f.payload.output.errorMessage}}
				</p>
				<button data-id="button" type="submit" class="btn btn-primary mb-3" data-skcomponent="skbutton"
					data-skbuttontype="form-submit" data-skform="form" id="btnContinue"
					data-skbuttonvalue="CONTINUE">
					Continue
				</button>
			</div>
		</div>
	</div>
</div>
```



### Additional Properties
formFieldsList
```
```





### Position

#### Previous Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL | [ppo83pmk4y](./ppo83pmk4y.md) | 
 
 #### Future Nodes
| Node Title | Node ID |
| :------------- | ------------ |
| EVAL |[kydkhvfnus](./kydkhvfnus.md) | 