# RedLotus_Acquisition
‖ Extract process dumps and analyze signed or unsigned files of all sorts.

- The acquisition conducts three stages of processes when deployed:
  (1) Dumps all Administrative process memories [process.dmp] and saves them in a  ProcessDump folder
  (2) Users can CTRL+C in order to break the operation at any moment after the acquisition if they do not want to proceed with stage 2.
  (3) Stage 2 consists of downloading and unzipping Eric Zimmerman's BSTRINGS
  (4) Stage 3 extracts all win_path data from dumped process.dmp files and generates a list of file paths under paths.txt
- After the acquisition is over and bstrings extracts paths, files are scanned for signature verification
- Average time for the full process to be over is ~20 minutes
- Users can modify the script in any way they desire. I would add the silent switch to bstrings to speed up paths extraction process.

## Used Utilities
BSTRINGS - https://ericzimmerman.github.io/#!index.md;

Timeline Explorer - https://ericzimmerman.github.io/#!index.md;

Powershell 7 - https://learn.microsoft.com/en-us/shows/it-ops-talk/how-to-install-powershell-7;

## REDLOTUS
https://discord.gg/redlotus

**YOUTUBE DEMO** https://youtu.be/cIrdJHYtw4g
