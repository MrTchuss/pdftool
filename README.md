INSTALL
=======

`sudo install -m 755 pdftool /usr/bin`

Split PDF
=========

`pdftool -s doc.pdf`

will create `doc_001.pdf`, `doc_002.pdf`, ... each document containing exactly
one page from the original document.

Merge PDF
=========

`pdftool -mdoc.pdf doc1.pdf anotherdoc.pdf ...`

will merge `doc_001.pdf`, `anotherdoc.pdf`, ... into `doc.pdf`.

**Please note that there is no space between `-m` and `doc.pdf`.**

Known bugs
==========

No space allowed between `-m` and parameter.
