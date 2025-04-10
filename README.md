Sysmon info corpus

Data collected from 15000+ computers at the University of Oslo.
250000+ entrys.

filename: sha256 of the image

File contents example:

```json
{
    "Company": "Microsoft Corporation",
    "FileVersion": "1.349.213.0",
    "IMPHASH": "73EFFD46557538D5FA5561EEE3FFC59C",
    "Image": "AM_Delta_Patch_1.349.193.0.exe",
    "MD5": "3BFF07F07626055F3FF043819530AD37",
    "OriginalFileName": "AM_Delta_Patch_1.349.193.0.exe",
    "ParentImage": "wuauclt.exe",
    "Product": "Microsoft Malware Protection",
    "SHA256": "00001E12FF472ADCA30870584785277E28D7AF90D237C72B6C2B70AD9B7C8D43"
  }
  
  ```

The data is free to use.  


update_2025-04-10 folder contains a sqllite-database with 600 000 items. Updated 2025-04-10

```
CREATE TABLE IF NOT EXISTS binaries (
    sha256 TEXT PRIMARY KEY,
    image TEXT,
    original_file_name TEXT,
    file_version TEXT,
    company TEXT,
    product TEXT,
    md5 TEXT,
    imphash TEXT,
    parent_image TEXT
);
```
