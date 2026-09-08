# AZ-104 · Microsoft Azure Administrator

Material de estudio para el examen **AZ-104** (Azure Administrator Associate). Es un sitio estático en HTML: módulos de repaso, flashcards, trampas de examen, escenarios con solución y labs para hacer en el portal.

El contenido está contrastado bullet por bullet contra el [skills outline oficial](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/az-104). Cada tema indica si es **núcleo** (entra en el examen), **mixto** o solo **contexto**.

## Cómo abrirlo

No hay build ni dependencias. Abrí `index.html` (redirige al índice) o `00-indice.html` en el navegador.

```bash
open 00-indice.html
```

O serví la carpeta con cualquier servidor estático si preferís no usar `file://`.

## Qué hay adentro

| Tipo | Archivos | Contenido |
| --- | --- | --- |
| Módulos de repaso | `01`–`17` | Teoría, tablas comparativas, callouts de trampas y flashcards |
| Práctica | `18`, `19` | 260 escenarios de examen + 134 labs en el portal |
| Anexos | `20`–`22`, `24`–`26` | Mapas visuales, comparativas y plan de 18 días |
| Extra | `23` | AKS operativo — **no entra en el examen** |

Números del índice: **17** módulos, **427** flashcards, **324** tablas comparativas y **305** trampas de examen.

## Dominios del examen

| Dominio | Peso | Módulos |
| --- | --- | --- |
| 1 · Identidades y gobernanza | 20–25% | Entra ID, RBAC, governance y costos |
| 2 · Almacenamiento | 15–20% | Cuentas, seguridad, Blob / Files / movimiento de datos |
| 3 · Compute | 20–25% | VMs, HA/VMSS, contenedores, App Service, ARM/Bicep |
| 4 · Redes virtuales | 15–20% | VNets/DNS, seguridad de red, balanceo, híbrido |
| 5 · Monitoreo y mantenimiento | 10–15% | Azure Monitor, Backup y Site Recovery |

## Prioridades

Varios servicios que históricamente se estudiaban para AZ-104 **ya no figuran en el outline**: AKS, Application Gateway, WAF, Front Door, Traffic Manager, VPN Gateway, ExpressRoute, Virtual WAN y Azure Firewall.

Siguen en el material porque un escenario puede nombrarlos como distractores. Priorizá lo marcado como núcleo.

- **Núcleo** — mapea a bullets vigentes. Acá se juega el examen.
- **Mixto** — parte entra y parte quedó afuera. La nota amarilla dice qué es cada cosa.
- **Contexto** — ningún bullet lo pide. Lectura de reconocimiento, al final y sin memorizar.

## Orden sugerido

Ordenado por retorno de examen, no por número de archivo.

1. **Identidad, gobernanza y compute** — `01` · `02` · `03` · `07` · `08` · `10` · `11`  
   Entre 40% y 50% del examen y todo núcleo.
2. **Storage completo** — `04` · `05` · `06`  
   Cobertura literal del outline; mejor relación esfuerzo/puntaje.
3. **Redes y monitoreo, salteando lo fuera de scope** — `12` · `13` (sin Firewall/JIT/DDoS) · `14` (solo Load Balancer) · `16` · `17`  
   Sumá Container Apps y escalado de `09`.
4. **Práctica** — `18` (escenarios) y después `19` (labs en el portal).

Hay un calendario listo en [`22-plan-18-dias.html`](22-plan-18-dias.html).

## Cómo usar cada módulo

1. **Leer** el módulo entero. Armá el mapa mental; no pares en las flashcards.
2. **Cazar trampas.** Solo los callouts amarillos de «Trampa del examen».
3. **Flashcards.** Lo que caiga en «a repasar», volvé a la sección; no lo memorices suelto.
4. **Escenarios** en [`18-ejercicios.html`](18-ejercicios.html): resolvé sin mirar la solución.
5. **Portal** en [`19-labs-portal.html`](19-labs-portal.html): clicar Azure de verdad. No reemplaza a los escenarios.
6. **Antes del examen:** tablas comparativas, flashcards fallidas y escenarios marcados mal. Nada de contenido nuevo.

## Mapa de archivos

```
00-indice.html                         Índice (home)
01–03                                  Identidad y gobernanza
04–06                                  Storage
07–11                                  Compute (09 es mixto: AKS fuera de outline)
12–15                                  Redes (15 es solo contexto)
16–17                                  Monitor, backup y ASR
18-ejercicios.html                     Escenarios con solución colapsable
19-labs-portal.html                    Labs en la suscripción
20-monitor-mapa.html                   Anexo visual de 16
21-comparacion-lb.html                 Anexo visual de 14
22-plan-18-dias.html                   Calendario de estudio
23-aks-fundamentos.html             Extra operativo, fuera de examen
24-geografia-visual.html               Anexo visual de 08
25-policy-visual.html                  Anexo visual de 03
26-storage-redundancy-visual.html      Anexo visual de 04
```
