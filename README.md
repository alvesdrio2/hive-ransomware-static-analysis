# hive-ransomware-static-analysis
Static malware analysis of Hive ransomware in an isolated lab environment

This repository contains a static malware analysis case study of a Hive ransomware sample obtained from the TheZoo repository.

The objective of this project was to perform a structured static analysis in an isolated lab environment, focusing on file identification, integrity verification, executable triage, UPX unpacking, string inspection, and IOC extraction.

## Analysis Scope
- Static analysis only
- No live detonation
- No malware execution
- Isolated analysis environment

## Tools Used
- file
- sha256sum
- md5sum
- strings
- UPX
- Detect It Easy (diec)
- Bulk Extractor

## Methodology
1. Extraction of the sample package
2. MD5 and SHA256 hash verification
3. File type identification of extracted artifacts
4. Initial triage of the main Windows executable
5. Detection of UPX packing
6. Unpacking of the main executable
7. Post unpacking static inspection
8. Extraction of network artifacts

## Key Findings
- The extracted files matched the MD5 and SHA256 hashes provided by TheZoo repository.
- The package contained both Windows and Linux artifacts.
- hive.bin_exe was identified as the main Windows executable.
- The executable was packed with UPX 3.96.
- After unpacking, the file structure became clearer for analysis.
- RSA cryptography references were identified.
- Two .onion domains were found in the unpacked executable.

## Notable Artifacts
- hivecust6vhekztbqgdnkks64ucehqacge3dij3gyrrpdp57zoq3ooqd.onion
- hiveleakdbtnp76ulyhi52eag6c6tyc3xw7ez7iqy6wc34gd2nekazyd.onion

The full report is available in this repository.

## Safety Notice
This repository is shared for educational and portfolio purposes only.

- No malware binaries are included
- No live samples are redistributed
- No malicious files should be executed outside a properly isolated lab

## Author
**Dário Alves**  
Cybersecurity Student
