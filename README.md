# HawkularAPMTracer

[![CI Status](http://img.shields.io/travis/pat2man/HawkularAPMTracer.svg?style=flat)](https://travis-ci.org/pat2man/HawkularAPMTracer)
[![Version](https://img.shields.io/cocoapods/v/HawkularAPMTracer.svg?style=flat)](http://cocoapods.org/pods/HawkularAPMTracer)
[![License](https://img.shields.io/cocoapods/l/HawkularAPMTracer.svg?style=flat)](http://cocoapods.org/pods/HawkularAPMTracer)
[![Platform](https://img.shields.io/cocoapods/p/HawkularAPMTracer.svg?style=flat)](http://cocoapods.org/pods/HawkularAPMTracer)

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

## Installation

HawkularAPMTracer is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod "HawkularAPMTracer"
```

## Usage

Initialize the shared tracer. It will register itself with OTGlobal:

```swift
APMTracer.setup(AppDelegate.appEnviroment.tracingURL, credential: AppDelegate.appEnviroment.tracingURLCredential, flushInterval: 10)
```

Normal OpenTracing commands should work. If you want track NSURLSession tasks you can set the delegate to an instance of `APMURLSessionDelegate`.

## Author

pat2man, pat2man@gmail.com

## License

HawkularAPMTracer is available under the MIT license. See the LICENSE file for more info.
