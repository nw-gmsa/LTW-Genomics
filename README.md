See [North West Genomics HL7/IHE Implementation Guide](https://nw-gmsa.github.io/R4)

Guidance on updating this Implementation Guide can be found on [Guidance for FHIR IG Creation](https://build.fhir.org/ig/FHIR/ig-guidance/index.html)

Related links:
 - [HL7 FHIR Implementation Guide Build Notications](https://chat.fhir.org/#narrow/stream/179297-committers.2Fnotification)

## Sending HL7 v2 Message

Note files must use CR or CRLF (not unix/mac LF)

### Mac

curl --request POST --data-binary "@OML_O21_PDF.txt" http://192.168.1.50:9980
curl --request POST --data-binary "@ORU_R01_PDF.txt" http://192.168.1.50:9980 

### Windows 

Invoke-RestMethod -Method POST -Uri http://192.168.1.50:9980 -InFile "OML_O21_PDF.txt"
Invoke-RestMethod -Method POST -Uri http://192.168.1.50:9980 -InFile "ORU_R01_PDF.txt"
