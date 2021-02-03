# ReplayLatest

ReplayLatest simplifies sharing and receiving the most recent values immediately upon subscription.

## Usage

### Import

Import ReplayLatest into your files:

```swift
import ReplayLatest
````

### Implementation

Use the operator in your publisher chain declaration:

```swift
let subject = PassthroughSubject<Int, Never>()
let publisher = subject.replayLatest(capacity: 2)
````

## Debugging

ReplayLatest includes a built-in printSink() operator for easy debugging without additional subscribers:

```swift
Just("value").printSink()
```

# Installation

Add ReplayLatest to your dependencies:

```swift
dependencies: [
	.package(url: "https://github.com/AbdAlAlii/ReplayLatest.git")
]
```

## License

**ReplayLatest** is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more information.