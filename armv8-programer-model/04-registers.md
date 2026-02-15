# ARMv8 Registers

## General Registers

31 × 64-bit general-purpose registers (`X0`-`X30`) at all times and in all Exception levels. They also has a 32-bit (W0-W30) form.

## ![image-20260215214058402](./04-registers.assets/image-20260215214058402.png)Special registers

![image-20260215214145057](./04-registers.assets/image-20260215214145057.png)

- `XZR` is 64 bits, `WZR` is the lower 32 bits, they are zero register: all writes are ignored and all reads return 0
- `SP` is 64bits, `WSP` is the lower 32 bits: Current stack pointer
- `PC` is 64 bits: Program counter

In AArch64, the exception return state is held in:

- `ELR` Exception Link Register
- `SPSR` Saved Processor State Register