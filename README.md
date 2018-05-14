# go-chip8

A practise project to learn about emulation, implements CHIP-8 in golang.

Note: Current implementation has major bug in rendering, which makes it unusable. Currently in process of hunting and solving.

## Screenshots

**__TODO__**

## Installing

- Get dependencies

```
go get -u github.com/veandco/go-sdl2/sdl
go get -u github.com/veandco/go-sdl2/mix
```

Note: Read the installation instructions for sdl2 library from [`go-sdl2`](github.com/veandco/go-sdl2) for your os platform.

- Get code

```
go get -u github.com/SKatiyar/go-chip8
```

## Running

Sample [roms](https://github.com/SKatiyar/go-chip8/tree/master/roms) can be used to test the installation.

```
go run main.go <modifier> <path/to/rom>
```

Modifier sets the logical size to pixel. Default resolution supported by `CHIP8` is `64 x 32`, setting modifier to `10` makes window of size `640 x 320`.

```
go run main.go 10 roms/filter.ch8
```

## Sources

- [How to write an emulator chip-8 interpreter](http://www.multigesture.net/articles/how-to-write-an-emulator-chip-8-interpreter/)
- [Cowgod's Chip-8 Technical Reference](http://devernay.free.fr/hacks/chip8/C8TECH10.HTM)
- [Chip-8 opcode table](https://en.wikipedia.org/wiki/CHIP-8)
