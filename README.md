This a fork of python library from @Aypac which allows conversion of gds (II) files / gdspy libraries to (lua-)latex and subsequently svg, pdf, png, jpeg from third party softwares. A major change has been included to assure that the library handle real full chip GDS files with a circuit layout bigger than 100 x 100 um^2. Original version often crashes lualatex/pdflatex during pdf generation. The solution proposed in this fork is changing the scaling and fixing the figure size to the documentclass page width (maximum size)

Install using pip:

`pip install git+https://github.com/DrPiBlacksmith/GDSLatexConverter.git`


Usage examples can be found <a href='/examples/inv_example.ipynb'>here</a>.
A fully operational application tool can be found <a href='https://github.com/DrPiBlacksmith/icLayoutRender'>icLayoutRender</a>.

Special thanks to <a href='https://github.com/mwb0506'>Marc Beekman</a>.
Special thanks to <a href='https://github.com/Aypac'>René Vollmer</a>.

## Dependencies
*Python*
 - numpy
 - gdspy
 - re (regex library, installed by default)

*Other*
 - Lualatex or PDFlatex
