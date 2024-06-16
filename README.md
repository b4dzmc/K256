# What is K-Arch?
the K-Arch is a SOC arch like ARM, but designed primarly to be a chip you would find in a NES or SNES. These special SOC are designed to play games and be fast, they are small and quick.
Most K-Arch based CPUs will feature K256 assembly, as it is the assembly language the K-Arch Decoder uses. Luckly, K-Arch actually supports MALS (MultiAssemblyLanguageSupport) meaning it can run 2 assembly languages at once via 2 decoders and custom commands.

The K256 SOC is heavily moddable, and can do basically anything. The entire machine is ran from a "Game Card" which is a ROM file you will give to the machine for it to run commands from. ROM files typically store Sprite files too, which store up to 256 Sprites for the game/program to be able to use on the GPU.

# What makes it special?

The K-Arch features the ability to have it's iGPU do CPU processes, allowing for much better game input response time or just porcessing in general as it acts as 2 cores. This makes most games much better in Minecraft as they don't need to waste a CPU instruction to run math for the GPU, or to move a VRAM value to RAM to Registers to jump, rather you can directly use GPU Registers.

K-Arch also features DSL (Direct Sprite Loading) which allows for Sprite ROM to store up to 256 sprites and the SOC be able to grab a sprite and laod it into one of the Sprite Slots the SOC may have.
K-Arch is very good for 8-bit gaming as it is designed around being a chip for gaming, inspired by the IHML SOCs designed by TheWhyNow.

I will make more on this, but just know it's a arch designed for gaming for now.
