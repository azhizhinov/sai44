![20250221_154534](https://github.com/user-attachments/assets/0850a692-3fcd-44b7-a864-f737b6b71859)
![20250221_154259](https://github.com/user-attachments/assets/1dd42fe0-a154-42db-8a10-87368bcf6b22)


ZMK firmware that is compatible with ZMK Studio.  
Split keyboard with Dongle.  
Dongle has a display.  
  
Display configuration:
sck to pin 20  
sda to pin 17     
vcc and gnd to vcc and gnd 
 
If you want to have the Nice Nano face up, solder the pads on the bottom. For face down, solder the pads on top.

Info from the reddit post:
https://www.reddit.com/r/ErgoMechKeyboards/comments/1iv1ksa/sai44_a_katana_layout_wireless_split_using_zmk/

Introduction

This is my newest keyboard I'm calling the sai44. I've been using an ortho staggered (churri and then the PCB variant Hellebore) for nearly two years now. I loved the ergonomics and the customizations that come from QMK and Vial, but there was always something drawing me away from it. I'm not sure if it was the aesthetics of it of my love of the standard slab style keyboards. I first saw the katana layout about a month or two after building my first ortho staggered board. The sunk cost fallacy made me convince myself that I liked the one I just built more, but it was always there in the back of my head. Finally, I had an itch to build a new board as I had made multiple modifications to my Hellebore board but was never satisfied.
Naming

At first I was going to call this board Banana Katana and have a banana icon inlay somewhere on the board. As I was working on this project, the name just didn't feel right so I went back to the drawing board with it. I landed on sai44. The reasoning: The Katana board is a single piece, a single sword, where as this one was going to be a split, dual wielded if you will. So the Sai was the logical choice in my opinion.
Iterations

If you look in my post history, you will see a dead bug styled hand wired that I built (Only the left side and never bothered with the firmware). It was too busy for my liking so I scrapped that idea. Also, it looked a lot better in pictures than in person. My next idea was I was going to use to ScottoModule and use the STM32 chip and have the footprint be just be keys and no MCU visible. Well I designed it and got it printed but made a big flaw and put the STM32 way too far from the USB so it never communicated with the computer. At that point I was juggling the idea to either redo it, or pivot and go with ZMK. I decided on ZMK obviously, and here is the final revision... For now. When it was going to be a STM32 build, I needed to make the LED's north facing to fit the USB sockets. After I pivoted I didn't realize that I left them that way until I was soldering everything. If I make a MRK2 I will 100% make them south facing. I also wish I integrated a track point into it to give it a Thinkpad vibe.
Build

Not much to say about this, it's a standard PCB sandwich with a 3d printed base and MCU covers. The only thing of note that I really like is that I didn't bother with any mounting for the plate to the PCB. On my hand wired build, I realized that the friction on the switches sitting in the hotswap sockets was enough for it to hold itself down. It adds a clean aesthetic that I really appreciate. As for the MCU covers, I'm not sure that I like them or not. It is something I may change in the future.
Switches and keycaps

For the switches, I saw a post a couple months ago about the Gateron Grey Heron KS-33 switches that are directly compatible with MX hotswap sockets. This spoke to me deeply as I have been wanting a low profile board but want it to be compatible with the switches I already have as I like swapping things often. This is another reason that I decided to not mount the plate to the PCB as I would not have to change the height of the standoffs. The keycaps were a blank set of white low profiles from AliExpress. Since I wanted this board to be all black, I disassembled the switches and dyed them black along with the keycaps. They didn't turn out entirely black (I think I diluted the dye too much) so I will most likely go back for another round of dying (The keycaps, not the switches. That was a lot of work I do not want to repeat). I have done this for the caps on my Hellebore keyboard and have gotten them jet black so I know that it is possible. A note to anyone who might want to get the Gateron Grey Heron switches, the 1.6mm plate thickness of normal MX switches is too thick. You will need to use a 1.2mm plate. I made this "mistake", which I'm not too upset about as I have plates for mx switches.
MCU and hardware

I am using Nice Nano clones from AliExpress. I found a seller that sells the updated version with the correct resistor so that should help with the battery life. If it does not, I will shell out for the proper Nice Nanos. The Batteries are 401230 as I had a bit of extra space with my Mill Max sockets. The Dongle is a Nice Nano clone with one of those cheap OLED screens. I contemplated the Prospector dongle but decided against it as I really wont be looking at it except checking the battery life so this is fine. Maybe I'll upgrade in the future if I get restless.
Plans

I think I want to figure out some tenting solution that is more stealth. I've had some success with using line of sight to hide the tenting and using magnets to hold it in place, but nothing that I'm satisfied with yet. If it's worth sharing, I'll make another post.
Ergonomics...

I'm aware that this is for sure a step back in ergonomics from my column staggered ortho board I was using previously. I have medium to large hands, so I can reach all the keys with little wrist movement. For me, aesthetics are very important as I will not enjoy using a device if I don't like how it looks. The split nature of these ergo boards have gotten me to a happy spot in ergonomics, so I don't mind taking a step or two backwards. That being said, I am finding it easier to type on this than I did on my other board. One thing that at first made me think that this was a dead end and I'd have to scrap the idea was my old keymap. It was not designed for this board but I was using it anyways. It caused some over reaching with my thumb which caused quite a bit of pain. After some tweaking though, I can say that this issue has been improved/resolved.
Final thoughts

I hope that you guys like this as much as I do. This feels like I've satiated something I've been craving ever since I got into this hobby. I'm on the fence on whether I will make the files available. It's a bit jank right now and I don't know that I want to put in the effort to make it more polished to a point where I would feel comfortable having other people make it. After I posted the churri files, about 4 of 5 months later, I tried building it again and realized what a terrible experience it was. It made me feel awful that I might have put some people through that and I don't want to repeat that feeling.
