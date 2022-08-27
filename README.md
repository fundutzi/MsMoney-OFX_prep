# MsMoney-OFX_prep
Cleans OFX file so you can auto import to MsMoney

1. Ensure you have these files in same directory {with no spaces}
  Example directory: c:\OfxPrep
  a.  "2050-OFX_prep_MsMoney.bat"
  b.  "sed.exe" for windows.  
      "sed" I use, source is here: http://unxutils.sourceforge.net/   ; sed.exe md5: 6221606e3aaefc39c20bae7ba4269098
  c.  The OFX file you dopwnloaded from the bank. Say "123456.ofx"

2.  Simply drag and drop the "123456.ofx" onto the bat file.
  The theory, all non compatible "TRNTYPE" field types will be replaced so you can import the OFX file to MsMoney.

3.  If your OFX file still fail to import search for lines with "TRNTYPE".
  Ensure you replace the transactio types with "OTHER"
  
Example, say you find:

    <TRNTYPE>Card Purchase
    or say 
    <TRNTYPE>THE QUICK BROWN FOX

      =>  Change the above to:

    <TRNTYPE>OTHER
    or say 
    <TRNTYPE>OTHER

4.  Hope that helps.
Bye

  

