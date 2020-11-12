# vim-slides

Use vim for quick presetions.  Presentation script expects a single argument, the name of the presentation file.  This file must exist in the ```slidedecks``` directory.  A line with ```#``` in the first column denotes the start of a news slide.  The script splits the file into separate slide files and loads them into Vim using a custom vimrc file.  Each slide file is loaded into its own buffer and the vimrc file remaps the cursor keys to to move forward and backward through the buffer.  It is assumed the slides will be presented on an 80x24 terminal and the vimrc sets column 81 to a different color so you can tell if the terminal is too wide.  When you quit the presentation, the temporary files from the split are removed.

## Starting a Presentation

Pass the filename of the presentation.  For example:</br>
```./present git```

## Stoping the Presentation

Just quit all buffers (```:qa```)

## Switching to a Shell

If you want to switch out to a shell for a quick demo, use Vim's command line (```:sh```).  Exiting the shell (```exit``` or ^d) will return you to Vim as normal.
