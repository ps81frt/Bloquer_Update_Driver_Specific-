# Bloquer la mise a jour d'un ou plusieurs pilote specifique


## Remplacer la valeur HardwareIDs par les id du periphérique en question 
### Enregister en .reg

    Windows Registry Editor Version 5.00

    [HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\DeviceInstall]

    [HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\DeviceInstall\Restrictions]
    "DenyDeviceIDs"=dword:00000001
    "DenyDeviceIDsRetroactive"=dword:00000000

    [HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\DeviceInstall\Restrictions\DenyDeviceIDs]
    "1"="HardwareIDs"
    "2"="HardwareIDs"
    "3"="HardwareIDs"




