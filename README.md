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
* ``indent`` - Indents the first line of each paragraph
* ``nohyphen`` - Attempts to prevent words becoming hyphenated
* ``draft`` - Places a DRAFT watermark across the document
* ``twosided`` - Adjusts margins and inserts blank pages to allow the document to be printed double sided

##Class Macros
* ``\statements`` - Creates the statements page, using the name specified as the dissertation author
* ``\abstract{<abstract>}`` - Creates an abstract page.
* ``\acknowledgements{<acknowledgements>}`` - Creates an acknowledgements page.
* ``\course{<Electronic Engineering|Computer Systems Engineering>}`` - Adds the course scheme, which is printed verbatim, to the title page.
* ``\supervisor{<supervisor>}`` - Adds a supervisor. For multiple supervisors call this macro multiple times.
* ``\partner[<vertical spacing>]{<content>}`` - Adds content to the title page, underneath the Bangor logo and school information. If a vertical spacing is omitted the content is centred between the crest and degree information.
* ``\tables`` - Generates the contents, figures, and tables pages.
* ``\abbrv{<abbreviation>}{<definition>}`` - Adds an abbreviation to the abbreviations page
* ``\content`` - Marks the point at which the main document body begins.
* ``\references`` - Creates the references pages.

##Abbreviations
This package has the ability to generate an abbreviations page, using the ``\abbrv`` macros mentioned above.

After typesetting the document run the command ``makeindex <document title>.nlo -s nomencl.ist -o <document title>.nls`` to sort the abbreviations, then typeset your document again.

