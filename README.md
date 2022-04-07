# FullProfAPP-beta
Distribution for the beta version of the FullProfAPP, includes binaries and examples.

The development of the FullProfAPP is carried out in the frame of a collaboration between CIC energiGUNE (Spain; Oier Arcelus, Montse Casas-Cabanas, Javier Carrasco, Marine Reynaud), ICMAB-CSIC (Spain; Oier Arcelus, M. Rosa Palacín, Carlos Frontera, Ashley Black), Institut Laue Langevin (France; Juan Rodríguez Carvajal, Nebil Katcho) and ALBA Synchrotron (Spain; François Fauth, Oriol Vallcorba). It is supported through a project of the first Stakeholder Initiative of the BIG-MAP project (in turn part of the European research initiative BATTERY 2030+), which has recieved funding from the European Union's Horizon 2020 research and innovation program under grant agreement No 957189.

## LICENSE
This software is distributed under the **GNU General Public License version 3 (GPLv3)**. For more information about the licensing terms read the LICENSE file, or go [here](https://www.gnu.org/licenses/gpl-3.0.en.html).

In compliance with the terms and conditions of **GPLv3**, the source code for the beta version is available by petition of the users (see contact information).

## Developers
Oier Arcelus, Juan Rodriguez-Carvajal, and Nebil Ayape Katcho.

## Compatibility
Tested on Windows 10 64bit computers

## How to run the APP
FullProfAPP is distributed as a standalone executable binary, which means that there is not need to install anything! Just download the repository using Git or downloading a .zip file and run the `fpapp.exe` binary that you can find in the `..\FullProfAPP-beta\dist\fpapp` directory.

FullProfAPP acts as a wrapper for the refinement program FullProf, managing I/O files and calling for its execution when needed. Therefore, in order to properly run the APP, make sure that FullProf Suite is properly installed and included in the `PATH` environmental variable.

FullProf Suite is also in active development and some of its features have been adapted for FullProfAPP. Thus, before launching the `fpapp.exe` binary, make sure that you replace the binaries in your FullProf Suite distribution (e.g. `C:\FullProf_Suite\CIFs_to_PCR.exe`) by the ones we provide in this distribution (`..\FullProfAPP-beta\fpsuite_mods\CIFs_to_PCR.exe`)

A video-walkthrough of FullProfAPP is also included in `..\FullProfAPP-beta\tutorial`, we strongly encourage you to watch it.

## Known BUGS
- FullProf considers that the space group contains the inversion center at the origin (setting 2 in the International Tables). FullProfAPP does not handle this issue yet, so it is the responsability of the user to choose CIF files that contain the correct setting.
- FullProf considers that Trigonal space groups are always given in the Hexagonal setting, therefore the same applies to the CIF files that contain Trigonal space groups with the Rhombohedral setting. FullProf will not give correct results, and its the responsability of the user to carefully inspect the CIF files first.

## Contact
CIC energiGUNE

fullprofapp@cicenergigune.com
