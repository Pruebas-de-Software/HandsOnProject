# 🤖 LogisticaGlobal.com: Gestión de Incidentes Robóticos en Warehouse

![logisticaglobal](./recursos/logisticaglobal.png)

## 🧩 El Problema

Carlos, supervisor de operaciones de la empresa **LogísticaGlobal.com**, se encarga de mantener un registro detallado y generar reportes mensuales y anuales sobre los incidentes de los robots que gestionan el inventario en los almacenes automatizados de la compañía.

Estos robots, responsables de mover productos y organizar existencias, sufren incidentes de distinta naturaleza (fallos mecánicos, colisiones, errores de software), los cuales deben ser clasificados según su tipo y causas.

Hasta ahora, Carlos lleva este control manualmente en Excel, pero con el aumento en la cantidad de robots y almacenes, esta solución se ha vuelto ineficiente. La trazabilidad del estado de los incidentes (creado, en investigación, resuelto) es casi imposible de gestionar, y los reportes manuales consumen demasiado tiempo.

El documento del incidente es llenado físicamente por el jefe de turno, quien se encarga del registro inicial indicando el identificador del robot afectado. Una vez listo, lo pasa a un documento Word y lo envía al supervisor en formato PDF.

Un incidente puede estar asociado a varios robots al mismo tiempo, pero se debe llenar una ficha distinta para cada robot, indicando el nombre o identificador del incidente.

Todos los incidentes comienzan con el estado **"Creado"**. Cuando el supervisor lo recibe, clasifica el incidente, define su gravedad y asigna a los técnicos de mantenimiento la reparación. Los técnicos, al completar el trabajo, devuelven el nuevo estado del robot con una breve descripción del trabajo realizado.

Finalmente, el supervisor revisa, firma, actualiza el estado, y genera el incidente en un documento PDF.

> Este proceso manual es propenso a errores y retrasos, por lo que Carlos ha contratado a tu equipo para desarrollar una aplicación web que centralice el registro, facilite la trazabilidad y automatice la generación de reportes.

---

## 💡 La Solución

**Gestión de Incidentes Robóticos** será una aplicación web que permita a Carlos y su equipo registrar, clasificar y dar seguimiento a los incidentes de los robots de inventario de forma centralizada y accesible desde cualquier dispositivo.

Cada incidente se registrará con base en una hoja física que llena el jefe de turno, incluyendo los siguientes campos:
- Fecha y hora del incidente
- Ubicación en el almacén (ej. sector o pasillo)
- etc.

La aplicación permitirá buscar, ordenar y filtrar incidentes por fecha, tipo, gravedad, estado o identificador, y generará reportes mensuales y anuales con estadísticas básicas (número de incidentes por tipo, gravedad promedio, etc.).

También incluirá una interfaz administrativa para que Carlos:
- Defina la gravedad
- Asigne técnicos de mantenimiento
- Firme digitalmente los casos resueltos
- etc.

Los técnicos reportarán el estado final del robot y una descripción del trabajo realizado. El supervisor tendrá una vista general.

---

## 🎯 Misión

Proporcionar una herramienta eficiente y confiable para registrar y gestionar incidentes de robots de inventario, mejorando la operatividad de los almacenes de logística del futuro mediante un control centralizado y reportes accesibles.

---

## 👁️ Visión

Ser la solución líder en la gestión digital de incidentes robóticos para empresas de logística automatizada, optimizando el seguimiento de fallos y apoyando la toma de decisiones basada en datos.

---

## 💬 Principios

- ✅ **Simplicidad y accesibilidad**: Facilitar el registro y consulta de datos para usuarios con distintos niveles de experiencia tecnológica.  
- 🔒 **Confiabilidad**: Garantizar que los datos sean precisos y trazables para mantener la eficiencia de la gestión de inventario automatizado.  
- ⚙️ **Eficiencia**: Reducir el tiempo dedicado a la generación de reportes y coordinación mediante automatización.  

---

## 🛠️ Requerimientos del Sistema

- 📝 Registro de incidentes ingresados desde hojas físicas.
- 🔗 Asociación de un incidente a múltiples robots mediante un identificador único, con fichas individuales.
- 🔍 Búsqueda, ordenamiento y filtros..
- 📦 Trazabilidad completa de estado de cada incidente con marcas de tiempo (al estilo seguimiento de paquetes como Starken).
- 👨‍💼 Interfaz para supervisores que permita:
  - Definir gravedad.
  - Asignar técnicos.
  - Revisar y firmar digitalmente.
- 👨‍🔧 Interfaz para técnicos:
  - Reportar estado final del robot (ej. operativo, en reparación, fuera de servicio).
  - Describir el trabajo realizado.
- 📊 Generación de reportes mensuales y anuales: tiempos, tipos de resolución, etc.
- 🔐 Registro de usuarios con login/password para todos los roles.
- 📋 Panel administrativo para gestionar usuarios y monitorear el sistema.
- 📱 Diseño responsive.

## Autor

- [@bastiansv Bastián Salomon](https://github.com/bastiansv)
---
