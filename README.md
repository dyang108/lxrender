### A tool to compile LaTeX on the fly
Clone this repository and write all your LaTeX files easily, regenerating on the fly without any fancy extra tools.

### Installation
Try this: `bash ./config.sh`. If it doesn't work, install manually:

Ensure that you have npm [installed](https://nodejs.org/en/download/). Then:
```
npm install -g nodemon
```
Ensure that `pdflatex` is in your `$PATH`:
```
which pdflatex
```
If the above has no output, you need to link the command to your bin, like so:
```
ln -s /Library/TeX/Distributions/Programs/texbin/* /usr/local/bin
```
Run the following command from within this directory to 
```
ln -s $(pwd)/lxrender /usr/local/bin/lxrender
```

### Running
I recommend the use of a pdf viewer like [Skim](http://skim-app.sourceforge.net/) in order to refresh the pdf. In Skim, go to `Skim > Preferences > Sync` and click the box for "Check for file changes."

To run lxrender, run:
`lxrender {{directory_name}} {{filename.tex}}`
where directory_name is the directory where the .tex file is, and filename is the name of the .tex file.

Input files are referenced from the directory where this repository is cloned (the directory containing the `lxrender` script). Thus, you should place image files in this directory.
