# Unix Terminal

* [General](#general)
* [Swift](#swift)
    * [Hummingbird](#hummingbird)

## General

Selects the listing of files any of whose Internet address matches the address specified in `i`\
`lsof -i :8080`

non-catchable, non-ignorable kill\
`kill -9 [PID]`

## Swift

`xcrun swift --version`

Toolchain location\
`xcrun -f swift`\
Export\
`export TOOLCHAINS=swift`

### Hummingbird
Just run the server\
`swift run Server`

Custom hostname and port\
`swift run Server --port 3000`\
`swift run Server --hostname 0.0.0.0 --port 3000`

Short version\
`swift run Server -p 3000`\
`swift run Server -h 0.0.0.0 -p 3000`

Set the log level (https://github.com/apple/swift-log#log-levels)\
`LOG_LEVEL=notice swift run Server -p 3000`

Make release build\
`swift build -c release`

Copy release build to the local folder\
`cp .build/release/Server ./Server`

Run the executable\
`LOG_LEVEL=notice ./Server -p 3000`















































dffd
