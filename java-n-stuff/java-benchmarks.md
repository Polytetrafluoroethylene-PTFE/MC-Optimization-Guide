# Java benchmarks

Here are some Java benchmarks I conducted in my free time.

Test system specs:

- AMD Ryzen 7 9800X3D
- NVIDEA GeForce RTX 4080 SUPER (Driver 591.74)
- ASUS TUF GAMING X870-PLUS WIFI
- RAM Corsair Vengeance DDR5 6000MHz 32GB 2x16GB CL30
- Kioxia Exceria Plus G3 2TB
- Windows 11 Pro 24H2

# Game loading times

An average of 10 runs of every Java version and garbage collector. This was tested in an [optimized MeatballCraft, Dimensional Ascension](/modpack-specific/packs-1.12.2.md#meatballcraft-dimensional-ascension). Java 8 and 25 were from Adoptium. The time was measured with VintageFix.

![average](https://github.com/user-attachments/assets/87568d20-7bbf-40c3-882f-fc8942539596)

Adoptium 25 with G1GC performs best here, followed by Adoptium 25 with Generational Shenandoah. Java 8 is considerably slower than everything else.

> [!CAUTION]
> Based on my testing, Generational Shenandoah has been extremely unstable, crashing in 4 out of 10 launches (40%)
