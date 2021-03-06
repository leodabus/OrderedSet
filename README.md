# OrderedSetAlgebra

[![CI Status](https://img.shields.io/travis/leodabus/OrderedSetAlgebra.svg?style=flat)](https://travis-ci.org/leodabus/OrderedSetAlgebra)
[![Version](https://img.shields.io/cocoapods/v/OrderedSetAlgebra.svg?style=flat)](https://cocoapods.org/pods/OrderedSetAlgebra)
[![License](https://img.shields.io/cocoapods/l/OrderedSetAlgebra.svg?style=flat)](https://cocoapods.org/pods/OrderedSetAlgebra)
[![Platform](https://img.shields.io/cocoapods/p/OrderedSetAlgebra.svg?style=flat)](https://cocoapods.org/pods/OrderedSetAlgebra)

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

## Installation

OrderedSetAlgebra is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'OrderedSetAlgebra'
```

## Usage

```
var ordereSet1: OrderedSet = [1,2,3,4,5,6,1,2,3]  // [1, 2, 3, 4, 5, 6]
var ordereSet2: OrderedSet = [4,5,6,7,8,9,7,8,9]  // [4, 5, 6, 7, 8, 9]

ordereSet1 == ordereSet2                     // false
ordereSet1.union(ordereSet2)                 // [1, 2, 3, 4, 5, 6, 7, 8, 9]

ordereSet1.intersection(ordereSet2)          // [4, 5, 6]
ordereSet1.symmetricDifference(ordereSet2)   // [1, 2, 3, 7, 8, 9]

ordereSet1.subtract(ordereSet2)              // [1, 2, 3]
ordereSet2.popLast()                         // 9
```

## Author

Leonardo Dabus, leodabus@gmail.com

## License

OrderedSetAlgebra is available under the MIT license. See the LICENSE file for more info.
