# Digital Forensics: Data Carving & File Recovery

## Overview

This repository contains my practical work for **Data Carving and File Recovery Techniques**. The lab focuses on recovering and analyzing digital evidence when filesystem metadata is missing, damaged, deleted, or unreliable.

## Objectives

* Analyze binary files using `xxd`
* Identify JPEG file signatures and boundaries
* Examine metadata-like content using `strings`
* Reconstruct files from hexadecimal data
* Analyze forensic images using The Sleuth Kit
* Identify embedded content with Binwalk
* Recover deleted files using Scalpel
* Verify recovered evidence using MD5 and SHA-256
* Document forensic procedures, findings, and limitations

## Tools Used

* Kali Linux
* `xxd`
* `strings`
* The Sleuth Kit
* Binwalk
* Scalpel
* `md5sum`
* `sha256sum`

## Lab Activities

### Part A: File Signatures & Hex Analysis

Examined a JPEG file using hexadecimal analysis, identified JPEG SOI and EOI signatures, and reconstructed the file from a hexadecimal dump.

### Part B: Metadata Examination

Used `xxd` and `strings` to search for visible camera, software, name, date, and other metadata-like information.

### Part C: Sleuth Kit Analysis

Used `img_stat`, `mmls`, `fsstat`, `fls`, `istat`, `icat`, and `blkcat` to examine filesystem and data-unit structures.

### Part D: Embedded File Discovery

Used Binwalk to identify recognizable embedded file structures and signatures.

### Part E: USB Image Preparation

Extracted the USB forensic image from `120M.7z`, calculated hashes, and confirmed the partition structure and offset using `mmls`.

### Part F: File Carving

Configured Scalpel and carved recoverable JPEG/JPG files from the forensic USB image. Recovered files were examined and hashed for verification.

## Evidence Integrity

Original evidence files were preserved and treated as read-only. MD5 and SHA-256 hashes were calculated to support evidence integrity and verification.

## Conclusion

This lab provided practical experience in **file signature analysis, hexadecimal examination, filesystem analysis, embedded-file discovery, and forensic file carving**. It demonstrated how investigators can recover potential evidence when normal filesystem metadata is unavailable or unreliable.

> **Note:** This repository contains educational forensic work performed in a controlled laboratory environment.
