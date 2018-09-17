# Fillit

<img width="698" alt="st123" src="https://user-images.githubusercontent.com/26527567/45608892-f3cfb200-ba5d-11e8-9b3c-5b42d0714ffe.png">

Fillit is a project that let you discover and/or familiarize yourself with a recurring
problematic in programming: searching the optimal solution among a huge set of possibilities,
in a respectable timing. In this particular project, you will have to find a way to
assemble a given Tetriminos set altogether in the smallest possible square.

<img width="622" alt="st1232" src="https://user-images.githubusercontent.com/26527567/45608938-35605d00-ba5e-11e8-83a5-a2c5c307eed0.png">

A Tetriminos is a 4-blocks geometric figure you probably already heard of, thanks to
the popular game Tetris.

<img width="624" alt="st1232222" src="https://user-images.githubusercontent.com/26527567/45608981-6a6caf80-ba5e-11e8-9858-d12e01dc9a94.png">

Your executable must take only one parameter, a file which contains a list of Tetriminos
to assemble. This file has a very specific format : every Tetrimino must exactly fit in a
4 by 4 chars square and all Tetrimino are separated by an newline each.

<img width="664" alt="st1232222" src="https://user-images.githubusercontent.com/26527567/45609004-91c37c80-ba5e-11e8-8632-55bbd6c64695.png">

If the number of parameters sent to your executable is not 1, your program must display
its usage and exit properly. If you don’t know what a usage is, execute the command
cp without arguments in your Shell. It will give you an idea. Your file should contain
between 1 and 26 Tetriminos.

<img width="638" alt="st1232222" src="https://user-images.githubusercontent.com/26527567/45609081-0a2a3d80-ba5f-11e8-858e-6c7691cb5e0a.png">

The description of a Tetriminos must respect the following rules :
• Precisely 4 lines of 4 characters, each followed by a new line (well... a 4x4 square).
• A Tetrimino is a classic piece of Tetris composed of 4 blocks.
• Each character must be either a block character(’#’ ) or an empty character (’.’).
• Each block of a Tetrimino must touch at least one other block on any of his 4 sides
(up, down, left and right).

A few examples of valid descriptions of Tetriminos:

A few examples of invalid descriptions of Tetriminos

The goal of this project is to arrange every Tetriminos with each others in order to make
the smallest possible square. But in some cases, this square should contains holes when
some given pieces won’t fit in perfectly with others.

Even if they are embedded in a 4x4 square, each Tetrimino is defined by its minimal
boundaries (their ’#’). The 12 remaining empty characters will be ignored for the
Tetriminos assemble process.

<img width="622" alt="st1232222" src="https://user-images.githubusercontent.com/26527567/45609033-c0d9ee00-ba5e-11e8-90a7-2fc9a4e6377b.png">

Tetriminos are ordered by they apparition order in the file. Among all the possible
candidates for the smallest square, we only accept the one where Tetriminos is placed on
their most upper-left position.

