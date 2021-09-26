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

## Animation easing     
### Repeating  && Autoreverse  && CurveEaseOut
> .curveEaseOut: This option applies deceleration to the end of your animation. 
```swift
        UIView.animate(withDuration: 0.5, delay: 0.4,
          options: [.repeat, .autoreverse, .curveEaseOut],
          animations: {
            self.password.center.x += self.view.bounds.width
          },
          completion: nil
        )
```
<img src="https://github.com/YamamotoDesu/Animation/blob/main/BahamaAirLoginScreen/autoreverse.gif" width="200">  

___


### Repeating  && Autoreverse  && CurveEaseIn
> .curveEaseIn: This option applies acceleration to the start of your animation.        
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



## Spring animations    
### UsingSpringWithDamping && initialSpringVelocity
> usingSpringWithDamping: This controls the amount of damping, or reduction, applied to the animation as it approaches its final state. This parameter accepts values between 0.0 and 1.0. Values closer to 0.0 create a bouncier animation, while values closer to 1.0 create a stiff-looking effect. You can think of this value as the “stiffness” of the spring.    
> initialSpringVelocity: This controls the initial velocity of the animation. A value of 1.0 sets the initial velocity of the animation to cover the total distance in the span of one second. Bigger and smaller values will cause the animation to have more or less velocity, and will affect how the spring settles. Note however that the initial velocity is soon amended by the spring calculation, and the animation will always finish by the end of duration.     
```swift
        UIView.animate(withDuration: 3.5, delay: 0.5,
        usingSpringWithDamping: 0.5, initialSpringVelocity: 0.0, options: [], animations: {
          self.loginButton.center.y -= 30.0
          self.loginButton.alpha = 1.0
        }, completion: nil)
```
<img src="https://github.com/YamamotoDesu/Animation/blob/main/BahamaAirLoginScreen/autoreverse.gif" width="200">  

___


