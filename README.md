#Instalacion de Niresh Mavericks en PC

## Especificaciones del equipo

Procesador: AMD FX-6100
Mother: M5A97pro
Memoria: 8 Gb 1333mhz Kingstone
HD: SATA 120gb

## Pasos de instalacion

Instalar Niresh Maverics (http://hackintosh.zone/downloads/confirmation/75-niresh-mavericks-109-with-amd-intel/)
- Crear particion Mac OS (Con registro) de tipo GUID
- Personalizar la instalacion y destildar Trackpad, PS/2 Mouse & Keyboard Support
- Instalar (Tarda entre 15-20 minutos)
- Al reiniciar, cuando aparece el gestor Chameleon presionar cualquier tecla para que aparesca el prompt "boot:" y ahi teclamos "amdfx -x -v GraphicsEnabler=No" y presionamos ENTER.
- Continuamos con la instalacion normalmente
- Una vez instalado vamos a una terminal, nos dirigimos a /System/Libraries/Extensions/AMD7000Controller.kext y editamos el archivo Info.plist. En el mismo reemplazamos donde fuere 0x68181002 por 0x68191002.
- Luego editamos el archivo Into.plist de la ruta /System/Libraries/Extensions/AMDRadeonX4000.kext y tambien reemplazamos 0x68181002 por 0x68191002.
- Vamos al Kext Wizard o Kext Utility y ejecutamos Reparar Permisos y Rebuild Cache.
- Por ultimo hay un problema con el sonido que se escucha bajo y con interferencia de fondo. El unico metodo que encontre para mas o menos mitigarlo due ir a Perferencia de Sistema->Sonido->Salida y seleccionar "Line-out (Green Rear).


