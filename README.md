# tgatool.c
simple tool for TGA images
## HELLO
   I would like to present your attention a simple tool for TGA images.
   
## HOW TO USE?
   1. Compile the object module. Like this:
   `gcc -o tgatool.o -c ./tgatool.c`
   2. Include header file in your code, uses *include* macro:
   `#include "tgatool.h"`
   3. Use function from header, whith them usage (more details in tgatool.h);
   4. Indicate the object module in parametr list, when you compile your main program: `gcc -o program.bin ./main.c ./tgatool.o`
   5. Fun.

## FOR WHAT?
   This tool was created for educational purposes. You can use it to study 
   computer graphics. For example, you can create a canvas and draw a line 
   on it using the Bresenham algorithm. Next, you can make a simple parser 
   of .obj wavefront files and draw 3D models.
   
## DEPENDENCIES
   - C compiler;
   - Standart C library.
   
## LIMITATIONS
   - Writing to the color-maped type is not completed but
    opening color-maped images is allowed;
   - Ignoring the byte order. Some pictures may open upside down.
   - Everything is ultimately stored in a matrix of int's
    thus, pictures with a color depth greater than 32 will lose quality.
   - Only original TGA format supported, no extension/developer zone.
   
