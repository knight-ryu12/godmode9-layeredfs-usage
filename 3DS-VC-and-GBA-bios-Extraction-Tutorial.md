
# How to extract a ROM file out of a 3DS Virtual Console 
>by GlazedBelmont

Some games are so rare that a physical copy is very expensive, though if the game is available on the Virtual Console, it is a lot cheaper. Buying a Virtual Console is like buying the cart, you can dump the ROM and use it on emulators and rom hacks. 

Note that the same rules apply on digital games and physical games:
- You own ONE license so installing the game in multiple consoles is illegal.
- Sharing the rom is illegal

_For more info, please visit https://3ds.eiphax.tech/piracy.html._

**Note that this is for 3DS-only**

This tutorial is valid for: 
- Gameboy,
- Gameboy Color,
- Gameboy Advance,
- GameGear

NES VC uses the TNES header which makes them not playable if dumped and trying to fix the header is quite a pain.

SNES VC are strangely made so the ROM is altered and cannot be extracted without being vanilla. If you were to extract it correctly, the sound would be destroyed.



 **What you'll need:**
- A 3ds family system (3ds,2ds,etc.)
- CFW (Luma+B9S) if you don't have CFW, go on https://3ds.hacks.guide/ to install it.
- Godmode9 (You should already have it due to the CFW guide.)
- Access to your SD card
- Any valid 3DS Virtual Console game

***

### Section I: Dumping

1. Boot while holding the Start button to access Godmode9. 

![](https://i.imgur.com/feXDLre.png)

2. Navigate to 《[A:] SYSNAND SD》 and press A.

![](https://i.imgur.com/mekBeB2.png)

3. Hover on 《title》 and press R+A.

![](https://i.imgur.com/kvrNZ74.png)

4. Press A on 《Search for titles》 and wait until it finishes searching.

![](https://i.imgur.com/yZzUGgi.png)

5. At this point, you will see all your installed titles.

6. Find the Virtual Console game that you want to extract the ROM from and press A on it.

![](https://i.imgur.com/vA2UTXo.png)

7. Press A on 《TMD file options...》.
 
![](https://i.imgur.com/m2vcAAu.png) 

8. Press A on 《Mount CXI/NDS to drive》.

![](https://i.imgur.com/yvYXUFo.png) 

9. Confirm with A.

![](https://i.imgur.com/ZSTWP2T.png)

10. Now, you will be into the files of the Virtual Console game.

## **THE NEXT STEPS WILL BE DIFFERENT IF YOU ARE DUMPING A GBA VIRTUAL CONSOLE**

***

### Section II: Extracting a Non-GBA Virtual Console

1. You will see a folder called 《romfs》 , press A on it.

![](https://i.imgur.com/z7kFzl6.png)

2. Follow the instructions depending on the system:

**Gameboy and Gameboy Color**

 1. Open the folder called: 《rom》.

![](https://i.imgur.com/eufTmQK.png)

2. Press A on the file shown.

![](https://i.imgur.com/FxWxCm1.png)

3. Press A on 《Copy to gm9/out》.

![](https://i.imgur.com/gYtnIxQ.png)

4. Change the file extension to either 《.gb》 for original Gameboy games and 《.gbc》 for Gameboy Color games.
 
- It is useful to know that DMG is Original Gameboy and CGB is Gameboy Color.

**NES**

1. Open the folder called 《rom》.

![](https://i.imgur.com/WosubKW.png)

2. Press A on the file shown. 

![](https://i.imgur.com/kzfbYeE.png)

3. Press A on 《Copy to gm9/out》.

![](https://i.imgur.com/vzCZZcq.png)

4. Rename the file extension to 《.nes》.

**GameGear**

1. Open the folder called 《system》.

![](https://i.imgur.com/NUVx4CD.png)

2. Open the folder called 《roms》.

![](https://i.imgur.com/mGHt92x.png)

3. Press A on the file.

![](https://i.imgur.com/ENVAvPO.png)

4. Press A on 《copy to gm9/out》.

![](https://i.imgur.com/n1jI4sD.png)

### Section II.I: Extracting a GBA VC title 

1. Navigate to the folder named 《exefs》 and press A.

![](https://i.imgur.com/61aLxV4.png)

2. Press A on the file named 《.code》.

![](https://i.imgur.com/FkEIgTh.png)

3. Press A on 《copy to gm9/out》.

![](https://i.imgur.com/DaCts1B.png)

4. Press B until you return to main menu of gm9.

![](https://i.imgur.com/feXDLre.png)

5. Go in 《SD》 then in 《gm9》 and then in 《out》.

![](https://i.imgur.com/0aBfyru.png)

6. Press A on the file 《.code》.

![](https://i.imgur.com/RWKcn5p.png)

7. Press A on 《GBA image options》.

![](https://i.imgur.com/76fKTn2.png)

8. Press A on 《Rename file》.

![](https://i.imgur.com/z5H012n.png)

9. Confirm with A.

![](https://i.imgur.com/kNlfjt0.png)

10. Done!

![](https://i.imgur.com/OVJcbfG.png)

### Section III: Dumping a GBA bios

**Nintendo has included GBA bios in many VC titles, you can use this bios with gbarunner2 or an emulator to recreate that nostalgic boot screen.**

1. In the 《romfs》 folder, if there is a file called 《agb.bin》, guess what, that's your GBA bios.

![](https://i.imgur.com/zRvVML9.png)

2. Press A on 《copy to gm9/out》 and you now have a legally obtained GBA bios.

![](https://i.imgur.com/ZEJhWgg.png)

***

### Acknowledgements
I'd like to thank Chromaryu#6870, Spunky#0030, radostin04#1337, Hikaru#1042, eip∞#3283 and validusername16#9643.

Thanks to arm9#6666 for the markdown conversion.

 This tutorial wouldn't be the same without your help. 

***

_~_ ![](https://i.imgur.com/s2O6pJd.png) _GlaZed_Belmont_
