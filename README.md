# Motorola 68k Architecture Plugin (v0.1)
Original Author: [**Alex Forencich**](http://www.github.com/alexforencich)

_A disassembler and lifter for the Motorola 68k architecture._

## Description:

This plugin disassembles Motorola 68k machine code and generates LLIL.

To install this plugin, navigate to your Binary Ninja plugins directory, and run

```git clone https://github.com/wrigjl/binaryninja-m68k.git m68k```

## Minimum Version

This plugin requires the following minimum version of Binary Ninja:

 * release (Personal) - 1.1

## License

This plugin is released under a [MIT](LICENSE) license.

## Modifications by [Jason Wright](http://www.github.com/wrigjl)

 * register with ELF loader
 * fixups for binja il changes
 * fixed 'rtd' instruction to parse correctly
 * labels for 'jmp' and 'bra'
 * fixed 'roxr'/'roxl' instructions to add correct flag
 * fixed signedness of branches
 * added bhi, bls, bcc, bcs support
 * mark indirect jump/call as unresolved so il can figure it out
