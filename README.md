# vagrant-restore
Recuperación de un sitio Web hecho con Vagrant

Requerimientos

1.  Tener instalado drush en la maquina virtual creada con VirtualBox  y Vagrant en Windows.
2.  Haber generado un respaldo del sitio web con drush archive-backup. 

Pasos
 
1. Instalar Vagrant y el plugin hostsupdater (vagrant plugin install vagrant-hostsupdater)
2. Siga las instrucciones de https://www.webfoobar.com/node/52
3. Levantar el sitio en la carpeta con el comando: vagrant provision up

Si los tres pasos anteriores no cargan del todo la configuracón el sitio web anterior, siga los siguientes pasos:

1. Asegurese de que drush está instalado 
2. Ejecute drush archive-restore <nombre del archivo backup generado con drush> .   El nombre del archivo fue generado con drush archive-dump desde el directorio hmtl o docroot según el tipo de servidor.
  
  
  
  
  
