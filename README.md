# Public-Nxlog-Configs
This repository has NxLog configs that use a modular approach to configs. 
A master config file that will contain global values sets a include varaible, %ROOT%\conf\nxlog.d. 
All configs placed in %ROOT%\conf\nxlog.d will be run after the master config file loads the global values.

The file NxLog-Globalconfig.conf should be copied to %ProgramFiles%\nxlog\conf\ as nxlog.conf
This sets up all the required global variables as well as log management for NxLog logs.
Copy the moduless for the events you wish to collect to %ProgramFiles%\nxlog\conf\nxlog.d\ and Nxlog will run them.
The nice thing about this method is that if any one config file has a error, it will not stop the other modules from running.

Be sure and update the config files with the correct IP address for your forwarder \ collector \ sensor. 
Enjoy!
