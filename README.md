# Basic Animation 

## Animation options    

### Repeating   
>  repeat: Include this option to makes your animation loop forever. 
```swift
        UIView.animate(withDuration: 0.5, delay: 0.4,
          options: .repeat,
          animations: {
            self.password.center.x += self.view.bounds.width
          },
          completion: nil
        )
``` 
<img src="https://github.com/YamamotoDesu/Animation/blob/main/BahamaAirLoginScreen/repeat.gif" width="200"> 

___


### Repeating  && Autoreverse   
> .autoreverse: Include this option only in conjunction with .repeat; this option repeatedly plays your animation forward, then in reverse. 
```swift
        UIView.animate(withDuration: 0.5, delay: 0.4,
          options: [.repeat, .autoreverse],
          animations: {
            self.password.center.x += self.view.bounds.width
          },
          completion: nil
        )
```
<img src="https://github.com/YamamotoDesu/Animation/blob/main/BahamaAirLoginScreen/autoreverse.gif" width="200">  

___



