# BootSlide
Boot Sector version of the 15 number slider puzzle

<img src=https://github.com/XlogicX/BootSlide/blob/master/15slider.png width="400">

# Controls
* Arrow Keys
* 'x' is the int 0x20 exit (for BootOS)
* Any other key should re-scramble puzzle

# Object of the Game
Get the numbers in order by using the arrow keys to move the 'tiles' around. There is a 1/16 chance you will be in 'evil' mode where the board is red instead of blue. Evil mode is an impossible challange ;)

# Assemble and Play
* nasm bootslide.asm -f bin -o bootslide
* qemu-system-i386 -hda bootslide

# Issues
* Scrambling doesn't work well on QEMU on macos (rdtsc works differently)
