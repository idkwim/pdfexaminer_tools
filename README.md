pdfexaminer
===========

PDFExaminer PDF malware analysis tools - submit PDF and XDP (encapsulated PDF) files for analysis and receive results.

Search reports by any hash:
---------------------
GET or POST https://www.pdfexaminer.com/pdfapirep.php

### Query Params:

hash: Any md5, sha1 or sha256

md5: md5

sha1: sha1

sha256: sha256

A not found report will return json 'filename' "not found".


Upload file for analysis:
-------------------------
POST https://www.pdfexaminer.com/pdfapi.php

### Query Params:

sample[]: File content

message: note or email headers

email: your email address for report by emails

Limits
------

File uploads limited to approximately 12mb.
