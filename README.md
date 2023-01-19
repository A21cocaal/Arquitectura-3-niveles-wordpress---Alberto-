**Alberto Cobos Camacho – 2ºASIR** 

|<p>Implantación de aplicaciones web</p><p></p><p>Práctica 4.2 Instalar Wordpress en una arquitectura de tres niveles</p><p></p><p>Alberto Cobos Camacho</p><p>2º Administración de sistemas informáticos en red</p>|
| :-: |





# **Servidor nfs**
Lo instalaremos el servidor nfs en la maquina NFS

![](Aspose.Words.293fc4ea-2ebf-44c2-9239-1d461be368ac.002.png)
# **Cliente nfs**
Instalaremos nfs-common en los clientes

![](Aspose.Words.293fc4ea-2ebf-44c2-9239-1d461be368ac.003.png)

# **Archivo exports**

Pondremos lo siguiente en el archivo /etc/exports

Pondremos la línea por cada cliente que vaya a usar nfs

![](Aspose.Words.293fc4ea-2ebf-44c2-9239-1d461be368ac.004.png)

Ahora reiniciaremos el servicio

![](Aspose.Words.293fc4ea-2ebf-44c2-9239-1d461be368ac.005.png)
# **Creación de punto de montaje para el cliente NFS**
Haremos eso en todos los clientes

![](Aspose.Words.293fc4ea-2ebf-44c2-9239-1d461be368ac.006.png)

Y para comprobar que se ha montado correctamente usamos el comando df -h para ver si se ha montado

![](Aspose.Words.293fc4ea-2ebf-44c2-9239-1d461be368ac.008.png)

Para hacer que se monte cada vez que se inicie la maquina pondremos esta línea en el /etc/fstab para que se monte automáticamente al iniciar

![](Aspose.Words.293fc4ea-2ebf-44c2-9239-1d461be368ac.010.png)

Y por último instalaremos WordPress en el nfs

![](Aspose.Words.293fc4ea-2ebf-44c2-9239-1d461be368ac.011.png)

Alberto Cobos Camacho		       2ºASIR – 22/23
