# Bitacora de sesiones

La bitacora es el registro cronologico del trabajo. Anade una entrada al final
de cada sesion y conserva las anteriores. Escribe datos comprobables y enlaza
las evidencias utiles; evita frases generales como "he trabajado en Proxmox".

## Sesion 01 - FECHA

- Objetivo: iniciar GitHub y la documentacion Markdown.
- Acciones realizadas: PENDIENTE: configuraciones, cambios o investigacion.
- Decisiones y motivos: PENDIENTE: eleccion realizada y alternativas valoradas.
- Pruebas y resultados: PENDIENTE: resultado esperado, comando o metodo y resultado obtenido.
- Documentos o evidencias: [Ficha inicial](00-ficha-inicial.md).
- Incidencias y solucion o estado pendiente: PENDIENTE.
- Siguiente paso: PENDIENTE: accion concreta para la proxima sesion.

Anadir una entrada con esta estructura en cada sesion. El historial de
GitHub registra los commits; no hace falta incluir el hash del propio
commit dentro de su entrada de bitacora.

## Sesion 02 - 13/10/2026

-Objetivo: Analizar el hardware y la compatibilidad del equipo fisico para la instlación del hipervisor Proxmox 

-Acciones realizadas: 
  · Obtención de las especificaciones del hardware mediante [comandos](../evidencias)
  · Documentacion de las fuentes técnicas principales (Wiki de proxmox, de los sistemas operativos que virtualizaremos)
  · Escritura de la viabilidad del proyecto y realización completa de la [Fase 1](../docs/01-inventario-hardware.md)

-Decisiones y motivos: 
  ·Se clasificó el sistema como "apto con condiciones" al comprobarse arquitectura de 64 bits y soporte de virtualización hardware, condicionándolo a la verificación del firmware.
  ·Se estableció el almacenamiento mecánico (HDD TOSHIBA) como el principal cuello de botella del nodo frente al rendimiento de CPU y RAM.

-Pruebas y resultados: 
  ·Ejecución de [systemd-detect-virt](../evidencias/systemd-detect-virt.jpeg), obteniendo como resultado none, lo que confirma que el entorno opera de forma nativa sin capas de virtualización previas.

-Documentos o evidencias: 
  ·Ficha técnica de hardware, tabla comparativa de requisitos, análisis de componentes críticos, fuentes primarias y dictamen de viabilidad integrados en la documentación del repositorio (docs/).

-Incidencias y solución o estado pendiente: 
  ·Detectado aviso de mitigación (VMX disabled) en la CPU; pendiente comprobación y habilitación física del soporte Intel VT-x en la BIOS/UEFI de la placa base.

-Siguiente paso: 
  ·Diseñar la topología de red y el esquema de direccionamiento IP para el nodo Proxmox y los servicios necesarios para el proyecto.
  

[Volver al indice](../README.md)
