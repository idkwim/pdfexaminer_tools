pdfexaminer
===========

PDFExaminer PDF malware analysis tools - submit PDF and XDP (encapsulated PDF) files for analysis and receive results.

Search reports by any hash:
---------------------
GET or POST https://www.pdfexaminer.com/pdfapirep.php

### Query Params:

type: output format: json, ioc, xml, php (serialized array), severity, rating, is_malware, text, summary

hash: Any md5, sha1 or sha256

md5: md5

sha1: sha1

sha256: sha256

A not found report will return json 'filename' "not found".

### Example:

https://www.pdfexaminer.com/pdfapirep.php?type=json&sha256=2392ed21e8b91450a391da6a202ce13256ba6275395ddaf155e149144e5e3c21


Upload file for analysis:
-------------------------
POST https://www.pdfexaminer.com/pdfapi.php

### Query Params:

type: output format: json, ioc, xml, php (serialized array), severity, rating, is_malware, text, summary

sample[]: File content

message: note or email headers

email: your email address for report by emails

Limits
------

File uploads limited to approximately 12mb.
