[![CI](https://github.com/allyourcodebase/tracy/actions/workflows/ci.yaml/badge.svg)](https://github.com/allyourcodebase/tracy/actions)

# Tracy Profiler

This is [Tracy](https://github.com/wolfpld/tracy), packaged for [Zig](https://ziglang.org/).

## Installation

Install Zig 0.13.0 and then run the following command:

```
zig build
./zig-out/bin/tracy-profiler
```

You can also directly run the Tracy Profiler with the `run` step:

```
zig build run
```

### System Dependencies

#### Client

- `ws2_32` (windows)
- `dbghelp` (windows)
- `advapi32` (windows)
- `user32` (windows)
- `execinfo` (freeBSD)

#### Profiler

- `Ws2_32` (windows)
- `ole32` (windows) 
- `uuid` (windows)
- `shell32` (windows)
- `AppKit` (macOS)
- `UniformTypeIdentifiers` (macOS)
- `libGL` (linux)
- `libdbus-1` (linux, can be disabled with `-Dno-fileselector` or `-Dportal=false`)
- `libgtk+-3.0` (linux, when using `-Dportal=false`)
