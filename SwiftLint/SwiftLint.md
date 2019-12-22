# SwiftLint

SwiftLint is a tool to enforce Swift style and conventions. For more information you can go to the [SwiftLint](https://github.com/realm/SwiftLint/) GitHub page.

## Installation

### Using Homebrew:

```
brew install swiftlint
```

### Using CocoaPods:
Simply add the following line to your Podfile:

```
pod 'SwiftLint' 
```

## Setup

Setting up SwiftLint is very easy. You just open xCode, navigate to the build settings and add a new run script phase. Then copy the following shell command and your project is ready (if SwiftLint is installed on your machine).

```
if which swiftlint >/dev/null; then
  swiftlint
elif [ -f /usr/local/bin/swiftlint ]; then
  /usr/local/bin/swiftlint
else
  echo "warning: SwiftLint not installed, download from https://github.com/realm/SwiftLint"
fi
```
