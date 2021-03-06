2016/04/06

Comet version "2016.01 rev. 2".
This is a maintenance release of Comet.
http://comet-ms.sourceforge.net

- Reverts the modification encoding in the "output_txtfile" output back
  to reporting variable modification mass difference (e.g. DLSTM[16.0]HK)
  instead of the actual modified residue mass values (e.g. DLSTM[147]HK).


Comet is an open source MS/MS database search engine released under the
Apache 2.0 license.

Current supported input formats are mzXML, mzML, mgf, ms2, and cms2.
Current supported output formats are pepXML, Percolator tsv, SQT,
tab-delimited text, and .out files.

To run a search on an input file requires the Comet binary, a search
parameters file (comet.params), an input file, and a protein sequence
database in FASTA format.  The syntax of a search:

   comet.exe input.mzXML
   comet.exe input.ms2

Search parameters, such as which sequence database to query, modifications to
consider, mass tolerances, output format, etc. are defined in the comet.params
file.

One can generate a parameters file with the command

   comet.exe -p

Rename the created file "comet.params.new" to "comet.params".

Windows and linux command line binaries are included with this release.
