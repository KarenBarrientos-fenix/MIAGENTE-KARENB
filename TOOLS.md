# Notas de Uso de Herramientas

Las funciones de las herramientas se proporcionan automáticamente mediante llamadas de función.  
Este archivo documenta restricciones importantes y patrones de uso.

## exec — Límites de Seguridad

- Los comandos tienen un tiempo máximo de ejecución (por defecto 60 segundos).
- Los comandos peligrosos están bloqueados (rm -rf, format, dd, shutdown, etc.).
- La salida de los comandos se limita a 10,000 caracteres.
- La configuración `restrictToWorkspace` puede limitar el acceso a archivos solo al espacio de trabajo del proyecto.

## cron — Recordatorios Programados

- Esta herramienta se utiliza para programar recordatorios o tareas automáticas.
- Permite crear, listar o eliminar recordatorios programados.
- Se debe usar cuando el usuario solicite recordatorios en un horario específico.

Para más detalles sobre su uso, consultar la documentación de la herramienta `cron`.