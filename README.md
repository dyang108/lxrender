### A tool to compile LaTeX on the fly
Clone this repository and write all your LaTeX files easily, regenerating on the fly without any fancy extra tools.

### Installation
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

### Running
Put your LaTeX projects in this directory, naming each .tex file such that it can be referenced from this directory as `[name]/[name].tex`

I recommend the use of a pdf viewer like [Skim](http://skim-app.sourceforge.net/) in order to refresh the pdf. In Skim, go to `Skim > Preferences > Sync` and click the box for "Check for file changes."

Input files are referenced from the directory where this repository is cloned (the directory containing the `lxrender` script). Thus, you should place image files in this directory.
