# Java benchmarks

Here are some Java benchmarks I conducted in my free time.

Test system specs:

- AMD Ryzen 7 9800X3D
- NVIDEA GeForce RTX 4080 SUPER (Driver 591.74)
- ASUS TUF GAMING X870-PLUS WIFI (BIOS ver. 5.60)
- RAM Corsair Vengeance DDR5 6000MHz 32GB 2x16GB CL30
- Kioxia Exceria Plus G3 2TB
- Windows 11 Pro 24H2

# Game loading times

An average of 10 runs of every Java version and garbage collector. This was tested in an [optimized StoneBlock instance](/modpack-specific/packs-1.12.2.md#stoneblock). Java 8 and 21 were from Adoptium. The time was measured with VintageFix.

![average](https://github.com/user-attachments/assets/bdeb79d7-2ae6-4f71-ac8d-c9cff1d7fdf8)

GraalVM 24 with G1GC performs best here, followed by GraalVM 24 with Generational ZGC. Java 8 is considerably slower than everything else.

### Data from all 10 runs:

![all 10 runs](https://github.com/user-attachments/assets/ae575d18-40a6-472d-b1a0-2fabebd656df)
