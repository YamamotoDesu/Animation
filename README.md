# Basic Animation 

## Repeating   
<img src="https://github.com/YamamotoDesu/Animation/blob/main/BahamaAirLoginScreen/repeat.gif" width="200">   

```swift
        UIView.animate(withDuration: 0.5, delay: 0.4,
          options: .repeat,
          animations: {
            self.password.center.x += self.view.bounds.width
          },
          completion: nil
        )
``` 

## Repeating  && Autoreverse
<img src="https://github.com/YamamotoDesu/Animation/blob/main/BahamaAirLoginScreen/autoreverse.gif" width="200">   

```swift
        UIView.animate(withDuration: 0.5, delay: 0.4,
          options: [.repeat, .autoreverse],
          animations: {
            self.password.center.x += self.view.bounds.width
          },
          completion: nil
        )
```
