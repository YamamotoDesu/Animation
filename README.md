# Basic Animation 

## Repeating   
<img src="https://github.com/YamamotoDesu/Animation/blob/main/BahamaAirLoginScreen/autoreverse.gif" width="200">   

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
<img src="https://user-images.githubusercontent.com/47273077/133958788-02d3da18-829d-4185-994b-9fd7d1eca382.png" width="200">   

```swift
        UIView.animate(withDuration: 0.5, delay: 0.4,
          options: [.repeat, .autoreverse],
          animations: {
            self.password.center.x += self.view.bounds.width
          },
          completion: nil
        )
```
