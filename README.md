# TreeUI
A GUI for performing analysis on a ROOT TTree stored in a .root file.

Requires ROOT, tested on version 6.30/06.

## How to install
For bash
```bash
git clone https://github.com/charlievelas/TreeUI.git
cd TreeUI
export TreeUI=$PWD
alias antiConGUI="root $TreeUI/antiConGUI"
alias antiConSaveGUI="root $TreeUI/antiConSaveGUI"
alias fitGUI="root $TreeUI/fitGUI"
alias loadGUI="root $TreeUI/loadGUI"
alias moreConsGUI="root $TreeUI/moreConsGUI"
alias moreMoreConsGUI="root $TreeUI/moreMoreConsGUI"
alias moreConsSaveGUI="root $TreeUI/moreConsSaveGUI"
alias orMoreConsGUI="root $TreeUI/orMoreConsGUI"
alias loadGUI="root $TreeUI/loadGUI"
alias saveGUI="root $TreeUI/saveGUI"
alias tandemGUI="$TreeUI/tandemGUI"
alias ThreeDGUI="root $TreeUI/ThreeDGUI"
```
It's recommended to add all of these aliases to your bash_alias, bashrc or equivalent file

## How to run
All GUIs, except tandemGUI, can be run by doing the following

    [GUI name] /location/of/root/file.root

For example

    loadGUI /location/of/root/file.root

tandemGUI is an exception due to addtional, optional execution option. 

tandemGUI can be run by
	
    root 'tandem("/location/of/root/file1.root","/location/of/root/file2.root")'

Both root files must have the same branches. If not, then the override option can be used

    root 'tandem("/location/of/root/file1.root","/location/of/root/file2.root","override")'	

