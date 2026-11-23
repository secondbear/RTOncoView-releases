# RTOncoView-releases

A radiotherapy DICOM viewer and tag editor for Windows: CT, MR and PET with structures, dose
(colour wash and isodose lines), plans and treatment records; a fast DICOM tag editor; and
anonymisation based on the DICOM PS3.15 basic profile.

> **For research use only – not for clinical use.** RTOncoView is not a medical device. Do not
> use it for diagnosis, treatment planning or any other decision about an individual patient.

## Download

From the [latest release](../../releases/latest):

| File                                         | For                                                                                                            |
| -------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `RTOncoView.App-win-Setup.exe`             | **Recommended.** Installs for your Windows user only: no administrator rights, and updates itself.       |
| `RTOncoView-<version>-portable-folder.zip` | No installation: unzip anywhere (USB stick, network share) and run `RTOncoView.exe`. Does not update itself. |

Windows 10 or 11, 64-bit. Nothing else needs to be installed.

The installer is not code-signed yet, so Windows may show "Windows protected your PC". Choose
**More info › Run anyway**.

## Trial and licence

RTOncoView runs as a 90-day trial without any licence file; after that it keeps working and
shows a reminder. Colleagues in research can ask for a free licence: open **Help › Licence…**, choose **Copy a licence request** and email it to

<!-- contact address or form link -->. You will get a `.lic` file to load in the same window.

## Licence

Copyright © 2026 André Haraldsson. RTOncoView is free for noncommercial research use under the
[PolyForm Noncommercial License 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0).
It is not a medical device and is not intended for clinical or diagnostic use. Commercial use
requires a separate licence from the copyright holder. The full text and third-party notices are
in the `Licences` folder of every download.

## Your data

DICOM files are read where they are; nothing is uploaded anywhere. The app keeps its index and
image cache in `%LOCALAPPDATA%\RTOncoView` (uninstalling leaves it in place – delete the folder to
remove it). Every DICOM file RTOncoView writes is marked as research output in a private
element (group 0011, creator "RTOncoView").
