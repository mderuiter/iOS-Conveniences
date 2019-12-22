# Deeplinks

Applications can be started via tapping the app icon on the home screen, but some applications can also be started via deeplinks. This sections is about how to easily use already configured deeplinks.

## Command Line
Deeplinks can be started via the terminal (or any other command line tool). 

#### Open simulator app:
```
open /Applications/Xcode.app/Contents/Developer/Applications/Simulator.app/
```

#### Start deeplink in booted simulator:
```
xcrun simctl openurl booted "your_deeplink_url_here"
```

#### Launch specific simulator:

List all the simulators
```
xcrun simctl list
```
Open specific simulator
```
xcrun simctl boot 50BDB70D-8475-4B38-920A-253A445888AA
```
