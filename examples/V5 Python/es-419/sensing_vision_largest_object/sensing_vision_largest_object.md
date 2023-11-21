category: sensing  
signature: vision.largest_object()
description: Reports information about a detected object from the Vision Sensor.

# Objeto Existe

Reporta sobre un objeto detectado desde el Vision Sensor.

```don
vision.largest_object()
```

## Cómo Utilizar

Para utilizar el bloque de objetos Visión, siga estos pasos:

1. Configure su Vision Sensor mediante la ventana Dispositivos.
2. Utilice la instantánea (snapshot) para capturar una imagen de Vision Sensor y busque una firma / código de color.
3. Utilice Objeto Existe para comprobar si el sensor de visión ha detectado la firma o el código de color solicitados.
4. Una vez que el Vision Sensor detecta un objeto, puede utilizar otros comandos de Visión para obtener más información sobre el objeto detectado.

* Utilice Definir Elemento de Objeto de Visión para establecer el objeto detectado sobre el que desea obtener más información. De forma predeterminada, se utiliza el objeto más grande detectado.
* Utilice Recuento de Objetos para determinar cuántos objetos se han detectado de ese código de firma/color solicitado.
* Utilice Objeto de Visión para determinar qué información se debe informar del objeto detectado.


<advanced>
</advanced>
