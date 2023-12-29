# A script to convert tmx files to tab-delimited txt files

This is a tmx-to-txt converter. It accepts one bilingual tmx file and 
one optional argument containing language codes separated by the # symbol. 
Examples: en-US#ar-SA; EN-US#RU-RU. All characters are case sensitive. 
The default codes are en-US and ru-RU. The script extracts TU text only. 
No fields are extracted. The output is a bilingual tab-delimited txt file.

## How to install on Windows in Windows PowerShell

```
$ python3 -m venv .venv
$ .\.venv\Scripts\Activate.ps1
$ python3 -m pip install --upgrade pip
$ python3 -m pip install tmx2txt
```
### How to use

In Windows PowerShell:
```
$ python3 -m tmx2txt \path\file.tmx -c en-US#ar-SA
```
In Google Colab:
```
!pip install tmx2txt
!tmx2txt file.tmx -c en-US#ar-SA
```