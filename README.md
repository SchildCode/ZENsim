# ZENsim
Simulation of a nearly net-zero GHG-emission neighbourhood, with distributed hydronic heating &amp; cooling, and building-integrated PV electricity generation.

### Functionality
- This program can simulate a neighbourhood consisting multiple building categories, using one year of hourly climate data (EPW weather data file). It summates the net heat demand (hydronic high and low temperature), cooling demand, and net electric demand (+ve) or production (-ve) in energy-distrubution hubs (nodes) in the neighbourhood.
- The building model is singe-zone thermal model that has been validated against EN 15265 & BESTEST.
- Infiltration heat loss is estimated using the LBL infiltration model.
- Photovoltaic systems are modelled in accordance with EN 15316-4-6, with the Perez anisotropic sky model, and  added possibility of battery storage (e.g. electric cars).

### Installation and activation
- Simply download the spreadsheet file and open it in Microsoft Excel. No installation or registration is needed.
- However, this is a Visual Basic macro-enabled spreadhseet. You must activate macros for it to function: 
  - When you open the file for the first time in Excel, you will see a yellow bar at the top of the window, with the message *"PROTECTED VIEW Be careful... [Enable Editing]"*. Click on the 'Enable Editing' button. 
  - Next, depending on the security settings on your installation of Microsoft Excel, a red bar may appear at the top of the window, with the message *"BLOCKED CONTENT Macros in this document have been disabled..."*. This can be solved by moving the file to a directory on your PC that you designate for files that you trust, then open the file in Excel. To designate a 'trusted directory', click on **File > Options > Trust Center > Trust Center Settings > Trusted Locations > Add new location**, then browse to a directory, e.g. C:\TEMP\. Finally check that **Trust Center Settings > Trusted Documents > Disable Trusted Documents**  is not ticked.
  - When macros are properly activated, **EpXL** shows a small square splash-screen when you open the file. This splash screen shows the licence info, and advises you if an update is available for download from GitHub. Simply press 'Close' button to close the splash-screen. 
  - If still no splash-screen appears, then you might be able to fix it by menu option **File > Options > Trust Center > Trust Center Settings > Macro Settings > Disable all macros with notification**, which is a suitable level of security.

### License & warranty
- Distributed under the GLP v3 lisence (https://www.gnu.org/licenses/gpl-3.0.en.html). Please acknowledge/attribute use of this software in your report/publication with an appropriate author citation and URL to this site.
- Provided without warranty of any kind.

### Author & copyright owner
© Peter.Schild@OsloMet.no
