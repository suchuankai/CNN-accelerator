# Dual-port Sram test

This is a simple test of dual port sram which generated by memory compiler.

- This SRAM supports simultaneous read and write operations. In the program, the A port is used for writing the values obtained from the tb, while the B port is used to read the values from SRAM memory.
- If simultaneous read and write operations are desired, the addresses for read and write operations must differ by 8. Otherwise, the read operation will take priority over the write operation.
- Each data entry is 64 bits.
- Because of memory size is mem[0:511][511:0].