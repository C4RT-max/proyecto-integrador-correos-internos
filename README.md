# Correos internos entre dos sedes

Proyecto integrador de tercer nivel de Ingeniería en Sistemas de Información.
Periodo académico: septiembre de 2026 a enero de 2027.

**Estado: fase 1, contexto, planificación y organización.** Aplicación seleccionada: gestión de correos internos. No hay aplicación implementada ni resultados de pruebas.

## Problema y propuesta

Una empresa de soluciones tecnológicas ha abierto una segunda sede y necesita comunicación institucional entre ambas, usuarios autenticados y protección de información. Proponemos un sistema interno de mensajes con bandejas de entrada y enviados, lectura y eliminación. No incluye correo externo ni integración SMTP.

La base académica exige una aplicación cliente-servidor en Go, autenticación con FastAPI e infraestructura de dos sedes con OpenWrt, VLAN y OSPF. Son condiciones del proyecto completo, todavía no implementadas. La fase 1 organiza el trabajo y justifica la selección.

## Equipo y responsabilidades propuestas

| Integrante | Coordinación principal | Apoyo y revisión |
| --- | --- | --- |
| Jose Martin Fuel | Contexto, selección y coordinación del componente de software | Revisión del contrato y del guion |
| Kevin Almache | Organización de infraestructura, repositorio y seguimiento | Revisión del contexto y viabilidad |
| Felipe Montenegro | Integridad académica, seguridad y perspectiva social y cuantitativa | Revisión de roles y evidencias |

Los tres participan en decisiones, revisiones y video. La distribución debe ser ratificada por el equipo; no acredita trabajo individual todavía no realizado.

## Documentos

- [Contexto, selección, actores, roles y planificación](docs/FASE_1.md).
- [Contrato de comunicación propuesto](docs/CONTRATO_COMUNICACION.md).
- [Integridad, licencia y registro de IA](docs/INTEGRIDAD_Y_LICENCIA.md).
- [Tablero de seguimiento de la fase 1](docs/TABLERO.md).
- [Guion del video para tres integrantes](docs/GUION_VIDEO.md).
- [Estado de entrega y pasos de GitHub](docs/ENTREGA.md).
- [Licencia MIT preliminar](LICENSE).

## Organización

El repositorio contiene README, LICENSE, .gitignore y documentos en docs/.
No se crean componentes de software, configuraciones de red ni prototipos en esta fase.

## Requisitos, instalación y pruebas

Para revisar esta entrega basta un lector de Markdown o GitHub. No existen pasos de instalación de una aplicación, variables de entorno, credenciales ni pruebas ejecutables en fase 1.
El hardware, las versiones, los comandos de ejecución y las pruebas se documentarán en las fases correspondientes. La base institucional contempla Raspberry Pi con OpenWrt o plataforma equivalente autorizada.

## Colaboración

Cada tarea tiene responsable, revisor, plazo relativo y evidencia en el tablero.
Los integrantes usarán sus propias cuentas para registrar contribuciones reales.
Repositorio remoto privado: [https://github.com/C4RT-max/proyecto-integrador-correos-internos](https://github.com/C4RT-max/proyecto-integrador-correos-internos), propiedad de C4RT-max. Usuarios de los otros integrantes y acceso docente: pendientes de configurar.
No publicar contraseñas, tokens, datos personales de prueba ni el PDF institucional sin autorización de sus titulares.

## Licencia y créditos

Licencia preliminar: MIT para las aportaciones propias de este repositorio. No modifica las licencias de terceros ni concede derechos sobre mensajes o datos de usuarios. Consultar [la justificación y declaración](docs/INTEGRIDAD_Y_LICENCIA.md).

Fuente académica: “PROYECTO INTEGRADOR – TERCER NIVEL”, apartados 1–5 (páginas 3–5) y apartado 6, fase 1 (página 6). El PDF se consultó, pero no se redistribuye.
Asistencia: Codex ayudó a interpretar la consigna, preparar borradores y proponer organización y guion el 9 de octubre de 2026. La revisión y defensa corresponden a los estudiantes.
