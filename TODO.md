# Bugs

- missing closing bracket in: extends B ( break connect ( b [2 * i ] , a [ i ]) ;
- check uses of "<=" etc. inside text (turns to arrows)
- check uses of "(C)"  (turns to copyright symbol)
- check uses of elipsis vs "..."
- add headers to tables
- fix xrefs
- fix latex in Appendix B and C
- convert EBNF to ISO/IEC 14977
- update copyright year
- fix table in 7.1.3. Restrictions on the Kind of Base Class
- fix table in 7.2.3. Merging of Modifications

Build with:

sudo docker run --rm -it -v $PWD:/documents/ asciidoctor/docker-asciidoctor asciidoctor -B /documents/ -b html5 --failure-level WARN -v --attribute=revnumber=3.7-dev --attribute=revdate=$(date +%F) docs/index.adoc

Regexes:

\\lstinline!Boolean*! -> `Boolean`

\\lstinline![^!]*!
`$1`

^=+[ X]
==$0

