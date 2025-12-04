# beamer-template
Template for my beamer slides

## Use

Define the `\title` and `\author` variables as you would usually. Additionaly you should set the custom `\presenter` *(your name)* and `\venue` *(conference name)* variables which are used in the tile frame and in frame footers.

Add your main content frames to the [`content.tex`](./content.tex) file, you supplementary material to the [appendix.tex](./appendix.tex) file.  

You can customize the aknowledgments in the [`thanks.tex`](./thanks.tex) file.

Add you references in the [`talk.bib`](./talk.bib) file or at least make sure you add your file with `\addbibresource{YOUR_FILE.bib}` in [`main.tex`](./main.tex).

## Build
I juste use [VimTeX](https://github.com/lervag/vimtex) but if you want you can build the slides manually using:  
`latexmk -lualatex --output-directory=build main.tex`
