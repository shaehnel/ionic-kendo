# Ionic with KendoUI example

Q: Can we use KendoUI widgets in an Ionic application?

A: Seems like (with obstacles)

## What happens here?

The application was created using Ionic's sidemenu example, see http://ionicframework.com/getting-started/

- `www/templates/browse.html`: using KendoUI Angular bindings
- `www/index.html`: including KendoUI style and js
- `www/lib/telerik/*`: checking in KendoUI Core code (KendoUI Core available in npm registry and as webjar)

### Result

- Ionic and KendoUI can be combined. 
- Need to use full JQuery. Need to have compatible AngularJS versions in Ionic and KendoUI bindings.
- KendoUI numeric textbox, combobox and color picker work out-of-the-box.
- KendoUI Calendar not showing. Not sure why and no desire to debug.
- Assumption: Other components might work instantly or need a bit of attention before they work. But no blockers.


## Building

Just use Ionic. Quick test:
  
    ionic serve
    
Run in iOS emulator:

    ionic platform add ios
    ionic build ios
    ionic emulate ios
    
