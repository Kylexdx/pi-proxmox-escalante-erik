# Inventario investigado y viabilidad

## Contexto de la observacion

- Fecha y sistema utilizado: 13/10/2026 SO Lliurex.
- Modalidad, equipo anfitrion y VM VirtualBox si procede: Equipo Anfitrion
- Version de Proxmox prevista: 9.2-1 (VE)

## Inventario inicial

| Area | Dato observado y evidencia | Especificacion y fuente | Limite o diferencia | Justificacion |
|---|---|---|---|---|
| CPU |Nombre: Intel(R) Pentium(R) CPU G4560 @ 3.50GHz 2 nucleos 4 hilos| Se consulta el nombre del procesador, el numero de cores y el numero total de hilos del procesador |Cumple con la arquitectura y el conjunto de instrucciones de virtualizacion necesario. | El procesador soporta virtualizacion por hardware de manera nativa, se ha comprobado via consola con el comando [ lscpu ] |
| RAM | | | | |
| Almacenamiento | | | | |
| Red | Interfaz de red Ethernet disponible en el equipo de aula [gestionada por el hipervisor o por host en este caso] | Al menos una interfaz de red (NIC) física para la conectividad de red y gestión del nodo | Cuenta con conectividad de red operativa unicamente en el aula, con restricciones de firewall | Permite configurar el puente de red (vmbr0) para que el nodo Proxmox y sus máquinas virtuales tengan acceso a la red local y conectividad exterior. |
| Plataforma | | | | |

## 1. Puedo instalar Proxmox en este equipo?

Contrastar el inventario con requisitos oficiales de la version prevista.
Responder por separado y justificar con datos y fuentes:

- Puedo instalar y arrancar Proxmox: PENDIENTE.
- Puedo ejecutar el servidor ASO y el cliente del proyecto: PENDIENTE.
- Condiciones o comprobaciones pendientes: PENDIENTE.

## 2. Que limitaciones tendre con este hardware?

Analizar RAM, CPU, disco y red para las cargas previstas. Identificar lo
medido y lo estimado. En VirtualBox, investigar host real y VM: version,
RAM reservada al anfitrion, vCPU, VDI, espacio fisico y red local.
No se utiliza el Proxmox del centro como recurso.

### Reparto de recursos

| Elemento | CPU/vCPU | RAM | Disco | Justificacion |
|---|---|---|---|---|
| Proxmox | | | | |
| srv-aso | | | | |
| cli-linux | | | | |
| Plantilla, ISOs y copias | No aplica | No aplica | | |
| Margen de operacion | | | | |

Mostrar calculos de RAM y disco, reparto de vCPU, unidades y supuestos.
Explicar las cargas que pueden funcionar simultaneamente.

| Limitacion | Evidencia o estimacion | Consecuencia | Medida y limite que permanece |
|---|---|---|---|
| | | | |

## 3. Que componentes son mas criticos en mi servidor y por que?

Ordenar al menos tres componentes para este equipo y su servicio.
Distinguir cuello de botella, disponibilidad e integridad de los datos.

| Prioridad y componente | Funcion | Efecto si es insuficiente | Efecto si falla | Evidencia y justificacion |
|---|---|---|---|---|
| 1. | | | | |
| 2. | | | | |
| 3. | | | | |

Componente que mejoraria primero y motivo para priorizarlo frente a otro:
PENDIENTE.

## Fuentes tecnicas

Consultar al menos tres fuentes primarias, incluyendo Proxmox y
fabricante o plataforma virtual. Relacionarlas con las tres respuestas.

| Fuente y URL | Version/modelo y fecha de consulta | Afirmacion respaldada | Aplicacion al nodo |
|---|---|---|---|
| | | | |

## Dictamen de viabilidad

Apto, apto con condiciones o no apto para la propuesta actual: PENDIENTE.

Sintetizar las tres respuestas y las condiciones pendientes de comprobar.

## Evidencias y revision docente

Enlazar salidas revisadas desde ../evidencias/. Un listado automatico no
sustituye la investigacion. Registrar la pregunta de defensa y respuesta.

[Volver al indice](../README.md)
