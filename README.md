# SimpleLinesCoreGrapghics
SimpleLinesCoreGrapghics

``` swift
import UIKit

class SimpleView: UIView {
    override func draw(_ rect: CGRect) {
        // context es el lienzo de pintado.
        let context = UIGraphicsGetCurrentContext()
        context?.setLineWidth(2)
        context?.move(to: CGPoint(x: 0, y: 0))
        context?.addLine(to: CGPoint(x: 100, y: 100))
        context?.setStrokeColor(UIColor.black.cgColor)
    
        context?.addLine(to: CGPoint(x: 100, y: frame.height))
        context?.strokePath()
    }
}
```

<p align="center">
    <img src="https://github.com/carlos-santiago-2017/SimpleLinesCoreGrapghics/blob/master/1.png" width="375">
</p>
