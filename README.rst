Southampton Provenance Tool Suite Test Cases
============================================

Test cases for software that uses documents represented using the `W3C PROV Data Model <http://www.w3.org/TR/prov-dm/>`_.

These test cases are used to test the `Southampton Provenance Suite <https://provenance.ecs.soton.ac.uk>`_.

Test Cases
----------

A single test case consists of a set of files, where each file holds a document in one of the PROV representations:

+--------------------------------------------------------+---------------+
| Representation                                         | Extension     |
+========================================================+===============+
| `PROV-N <http://www.w3.org/TR/prov-n/>`_               | .provn        |
+--------------------------------------------------------+---------------+
| `PROV-O <http://www.w3.org/TR/prov-o/>`_ (Turtle)      | .ttl          |
+--------------------------------------------------------+---------------+
| `PROV-O <http://www.w3.org/TR/prov-o/>`_ (TriG)        | .trig         |
+--------------------------------------------------------+---------------+
| `PROV-XML <http://www.w3.org/TR/prov-xml/>`_           | .provx        |
+--------------------------------------------------------+---------------+
| `PROV-JSON <http://www.w3.org/Submission/prov-json/>`_ | .json         |
+--------------------------------------------------------+---------------+

For example, a test case whose name is testcase1 consists of the files testcase1.provn, testcase1.xml, testcase1.json, testcase1.ttl, and testcase1.trig. Each document within a single test case is semantically equivalent to the others within the same test case. Some test cases only have files for a subset of representations, as there are cases that can't be validly encoded in a particular representation (e.g. XML).

A library for W3C Provenance Data Model supporting PROV-JSON and PROV-XML import/export

License
-------

These test cases are released under the MIT license.
