# Basic Animation 

```swift
        UIView.animate(withDuration: 0.5, delay: 0.4,
          options: .repeat,
          animations: {
            self.password.center.x += self.view.bounds.width
          },
          completion: nil
        )
``` 

```swift
        UIView.animate(withDuration: 0.5, delay: 0.4,
          options: [.repeat, .autoreverse],
          animations: {
            self.password.center.x += self.view.bounds.width
          },
          completion: nil
        )
```
