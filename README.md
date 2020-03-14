# Brightness and contrast control

I have a Linux system with multiple monitors. I couldn't find a GUI widget that controls the brightness and contrast of the monitor (the only ones I could find modified the screen using software, which is not what I'm looking for). So I made my own commandline tool.


## Usage

First configure the scripts using the instructions in the source. You should have one line for each monitor. The brightness and contrast scripts should be mostly identical, except for the value after the -r commandline switch.

Now, place the scripts somewhere in your $PATH. I have put them in ~/bin, and added the following line to my .zshrc file (this should be your .bashrc file if you use bash):

    export PATH=~/bin:$PATH

After this, you can use the scripts in different ways:

Read the current brightness:

    > brightness
    50

Increase the current brightness:

    > brightness +20
    70

Decrease the current brightness:

    > brightness -10
    60

Set the brightness:

    > brightness 65

Of course, the same thing works for the contrast.
