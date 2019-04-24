# ZENsim
Simulation of a nearly net-zero GHG-emission neighbourhood, with distributed hydronic heating &amp; cooling, and building-integrated PV electricity generation.

### Functionality
- This program can simulate a whole neighbourhood consisting of multiple building categories, using hourly climate data. It summates the net water-borne heat demand (split between high temperature, i.e. domestic hot water, and low-temperature, i.e. space heating & ventilation heating coil), water-borne cooling demand (space cooling & ventilation cooling coil), and net electric demand (+ve) or production from building-integrated PV-panels (-ve), for multiple energy-distrubution hubs (nodes) in the neighbourhood. Electric loads are split between indoors (heat gain from lighting and equipment) and outdoors loads (e.g. outdoor lighting, car charging).
- The building model is singe-zone thermal model that has been validated against EN 15265 & BESTEST.
- Infiltration heat loss is estimated using the LBL infiltration model.
- Photovoltaic systems are modelled in accordance with EN 15316-4-6, with the Perez anisotropic sky model, and  added possibility of battery storage (e.g. electric cars).
- Loads can be stochastic, assuming a log-normal distribution. The standard deviation is defined in a 24-hour schedule for weekdays and weekends.
- Reads EPW climate data files (can be downloaded from https://energyplus.net/weather). One year of hour climate data is simulated for 7 consecutive years, so that peak loads are simulated on all 7 days of the week. You can also simulate climate change by morphing exsisting EPW files using online applications.

### Installation and activation
- Simply download the spreadsheet file and open it in Microsoft Excel. No installation or registration is needed.
- However, this is a Visual Basic macro-enabled spreadhseet. You must activate macros for it to function: 
  - When you open the file for the first time in Excel, you will see a yellow bar at the top of the window, with the message *"PROTECTED VIEW Be careful... [Enable Editing]"*. Click on the 'Enable Editing' button. 
  - Next, depending on the security settings on your installation of Microsoft Excel, a red bar may appear at the top of the window, with the message *"BLOCKED CONTENT Macros in this document have been disabled..."*. This can be solved by moving the file to a directory on your PC that you designate for files that you trust, then open the file in Excel. To designate a 'trusted directory', click on **File > Options > Trust Center > Trust Center Settings > Trusted Locations > Add new location**, then browse to a directory, e.g. C:\TEMP\. Finally check that **Trust Center Settings > Trusted Documents > Disable Trusted Documents**  is not ticked.
  - When macros are properly activated, **EpXL** shows a small square splash-screen when you open the file. This splash screen shows the licence info, and advises you if an update is available for download from GitHub. Simply press 'Close' button to close the splash-screen. 
  - If still no splash-screen appears, then you might be able to fix it by menu option **File > Options > Trust Center > Trust Center Settings > Macro Settings > Disable all macros with notification**, which is a suitable level of security.

### License & warranty
- Distributed free under the "CC BY-SA 4.0" lisence (https://creativecommons.org/licenses/by-sa/4.0/). BY-SA is Attribute-ShareAlike but does not require source-code disclosure. Provided without warranty of any kind.
- Please acknowledge/attribute use of this software in your report/publication with an appropriate author citation and URL to this site.
- If you wish to apply or elaborate on this model in your research, you are welcome to contact the author below.

### Author & copyright owner
© Peter.Schild@OsloMet.no
