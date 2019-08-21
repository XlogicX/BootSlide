# BootSlide
Boot Sector version of the 15 number slider puzzle

<img src=https://github.com/XlogicX/BootSlide/blob/master/15slider.png width="400">

# Controls
* Arrow Keys
* Any other key should re-scramble puzzle

# Object of the Game
Get the numbers in order by using the arrow keys to move the 'tiles' around. Assemble the 'evil' version for an impossible challange

# Assemble and Play
* nasm bootslide_evil.asm -f bin -o bootslide
* qemu-system-i386 -hda bootslide_evil

# Issues
* Scrambling doesn't work well on QEMU on macos (rdtsc works differently)
