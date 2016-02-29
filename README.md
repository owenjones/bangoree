#BangorEE
(An *unofficial*) Bangor Electronic Engineering Dissertation LaTeX Class.

This is a heavily modified version of Cameron Gray's "bangorcsthesis", the official Computer Science Thesis LaTeX Class - [https://www.ctan.org/pkg/bangorcsthesis?lang=en]("bangorcsthesis")

##Included Files
* ``bangoree.cls`` - The Electronic Engineering class file
* ``example.tex`` - An example document file
* ``skeleton.tex`` - A skeleton (ready to go) document file

##Required Class Options
* ``bsc`` - Sets degree to **Bachelor of Science**
* ``msc`` - Sets degree to **Master of Science**
* ``beng`` - Sets degree to **Bachelor of Engineering**
* ``meng`` - Sets degree to **Master of Engineering**

##Optional Class Options
* ``noindent`` - Prevents indentation of the first line of each paragraph
* ``nohyphen`` - Attempts to prevent words becoming hyphenated
* ``draft`` - Places a DRAFT watermark across the document

##Class Macros
* ``\statements`` - Creates the statements page, using the name specified as the dissertation author
* ``\abstract{<abstract>}`` - Creates an abstract page.
* ``\acknowledgements{<acknowledgements>}`` - Creates an acknowledgements page.
* ``\course{<Electronic Engineering|Computer Systems Engineering>}`` - Sets the name of your course, which is printed on the title page.
* ``\supervisor{<supervisor>}`` - Adds a supervisor. For multiple supervisors call this macro multiple times.
* ``\tables`` - Generates the contents, figures, and tables pages.
* ``\abbrv{<abbreviation>}{<definition>}`` - Adds an abbreviation to the abbreviations page
* ``\bibinit`` and ``\addbibresource{<bibliography>}`` - Setup the bibliography.
* ``\content`` - Marks the point at which the main document body begins.
* ``\references`` - Creates the references pages.

##Abbreviations
This package has the ability to generate an abbreviations page, using the ``\abbrv`` macros mentioned abov.

After typesetting the document run the command ``makeindex <document title>.nlo -s nomencl.ist -o <document title>.nls`` to sort the abbreviations, then typeset your document again.

