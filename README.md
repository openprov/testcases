# Southampton Provenance Tool Suite Test Cases

Test cases for software that uses documents represented using the [W3C
PROV Data Model](http://www.w3.org/TR/prov-dm/).

These test cases are used to test the [Southampton Provenance
Suite](https://provenance.ecs.soton.ac.uk).

## Test Cases

A single test case consists of a set of files, where each file holds a
document in one of the PROV representations:

| Representation                                       | Extension     |
|------------------------------------------------------|---------------|
| [PROV-N](http://www.w3.org/TR/prov-n/)               | .provn        |
| [PROV-O](http://www.w3.org/TR/prov-o/) (Turtle)      | .ttl          |
| [PROV-O](http://www.w3.org/TR/prov-o/) (TriG)        | .trig         |
| [PROV-XML](http://www.w3.org/TR/prov-xml/)           | .provx        |
| [PROV-JSON](http://www.w3.org/Submission/prov-json/) | .json         |

For example, a test case whose name is testcase1 consists of the files
testcase1.provn, testcase1.xml, testcase1.json, testcase1.ttl, and
testcase1.trig. Each document within a single test case is
semantically equivalent to the others within the same test case. Some
test cases only have files for a subset of representations, as there
are cases that can't be validly encoded in a particular representation
(e.g. XML).

A library for W3C Provenance Data Model supporting PROV-JSON and
PROV-XML import/export

## Current test cases

testcase1

* Created from [primer.pn](https://raw.github.com/lucmoreau/ProvToolbox/master/prov-n/src/test/resources/prov/primer.pn) available as "Primer" example in [ProvTranslator](https://provenance.ecs.soton.ac.uk/validator/view/translator.html) and [ProvValidator](https://provenance.ecs.soton.ac.uk/validator/view/validator.html). 
* Each document was manually created from primer.pn using these online forms.

testcase2

* Created from [sculpture.prov-asn](https://raw.github.com/lucmoreau/ProvToolbox/master/prov-n/src/test/resources/prov/sculpture.prov-asn) available as "Sculpture" example in ProvTranslator and ProvValidator.

testcase3

* Created from [pc1.xml](https://raw.github.com/lucmoreau/ProvToolbox/master/prov-xml/src/test/resources/pc1.xml) available as "PC1" in ProvTranslator and ProvValidator

testcase4

* prov.json was created by running [ProvPy](https://github.com/trungdong/prov)'s [PROV document with a bundle](http://prov.readthedocs.org/en/latest/usage.html#prov-document-with-a-bundle) example.
* Other documents were creatyed using [ProvToolbox](https://github.com/lucmoreau/ProvToolbox/) prov-convert script on prov.json.

## License

These test cases are released under the MIT license.
