# Perfiles del Logitech G602 y Comentarios sobre su uso con Linux.

## Motivacion: 
Compartir datos sobre la configuración que puede hacerse para dejar configurados los botones programables de  este ratón en linux . 
Si dudas entre el MX master S2 y este por que lo quieres usar en linux , ya has aclararo tu duda sobre cual es mejor para eso:p , si además de echarte las partidas en windows lo quieres para usarlo con linux y tener keybindings de tu ide preferido , este es por el que yo me he decantado, sobre todo por que puede guardar un perfil interno, que es lo intenersante.

## Sin soporte de la app oficial para Linux .
Para la configuracion hay que usar la herramienta oficial , la de mac o la de linux
https://support.logitech.com/es_es/product/g602-wireless-gaming-mouse
Usa la que menos rabia te de .

## Perfiles.
Por lo que he visto hay 2 tipos de perfiles: 
 1. El nativo , que es el que nos interesa para usarlo en el linux
 2. El de sofware  ( que permite cambiarse segun aplicaciones etc ), 
 
 
 Estos 2 formatos no son compatibles, por lo que si exportas un perfil de sowftware luego no lo puedes importar en nativo y viceversa.
 
 
 
El ubuntu .dat contiene un perfil que asigna 
super+alt+n (para 4 <= n <=9)  a los botones opcionales 
De esta forma se puede usar xdotool para rebindearlos
sin tener que estar arrancando un win para usar la herramienta.
Funciona pero tiene cierto delay , ya que primero se ejecuta la combinacion , luego se remapea. 
No es mala opcion para hacerla generica , pero 
mejor usar directamente perfiles concretos.

Esta basado en el post de https://robustiana.com/343-configuracion-botones-logitech-g602-ubuntu 

Mi opcion sera usar un perfil .dat , sin rebindeos con el xdotool aunque la herramienta es tan versatil que merece la pena , ese pequeño delay nos va a dar igual si queremos hacer una macro realmente compleja. 

Ire actualizando y metiendo perfiles para las nuevas aplicacioens. 



### PhpStorm.dat & Chrome dev.

botones alante/atras se dejan default , phptorm los usa para navegar a ultimos puntos de cursor.
Los G7/G8 -> alt+leftArrow / alt+right Arrow , (emulan mismo comportamiento que cambio de pestaña en chrome con ctrl+tab)
G9 -> F12  ( abrir consola chrome.)
G6 -> Ctrl + shift + F ( phpstorm busqueda proyecto y chrome)
