# Windows Filesystem Minifilter Driver
Filesystem driver for windows. Get's information from the configuration file about processes permissions. Controlls access to reading and writting files in the filesystem. Access control is realised with discretionary model. Added support for updating the configuration file without stopping the driver. Configuration file should be placed in the /System_root/ directory and named 'config.txt'. It should consist records for processes rigths for the files in such format: number of records, and all records one by one:

2

write.exe wfile.txt rw

new.exe nfile.txt r-
