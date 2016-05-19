# sastantua @ 42
```
Allosimanius Syneca is a planet noted for ice, snow, mind-hurtling beauty and
stunning cold. The view from the top of the Ice Crystal Pyramids of Sastantua
is widely known for its ability to release the observer’s mind to hitherto
unexperienced horizons of beauty.
```

This is one of the numerous projects done during the 42 piscine in July 2015.
It was completed in a week and can display fancy pyramids in ASCII that follow
a simple set of rules. The objective was to recreate the output of a given
binary perfectly.

The unix utility [`diff`](http://linux.die.net/man/1/diff) was useful when
testing.

## Compiling
The project currently only has the functions for generating the pyramid. To
compile, you will need a main. Assuming you have a working
[libft](https://github.com/pbondoer/42-libft):

```c
#include "libft.h"

int	main(int argc, char *argv[])
{
	if (argc < 2)
		return 0;

	sastantua(ft_atoi(argv[1]));
}
```

Alternatively, you can replace `ft_atoi` with the standard `atoi` 
implementation (using `stdlib.h` instead).

## Usage
Compiling this into a `sastantua` executable, you get:

```
$ ./sastantua 3

               /*\
              /***\
             /*****\
          /***********\
         /*************\
        /***************\
       /*****************\
    /***********************\
   /*************************\
  /************|||************\
 /*************|||*************\
/**************|||**************\
```
