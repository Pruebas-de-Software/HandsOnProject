# 🎭 Caso: “Teatro Mora”

---

## 🧩 El Problema

María, dueña de un teatro mediano, enfrenta problemas recurrentes con la venta de boletos para sus eventos debido a que su página web colapsa por la alta demanda durante los lanzamientos. Los usuarios intentan comprar entradas simultáneamente, lo que provoca errores, afectando las ganancias y la reputación del teatro.

Actualmente, María crea eventos manualmente en la página, pero no tiene control sobre los actores involucrados ni interacción con el público más allá de la venta. Para resolver esto, ha contratado a tu equipo para desarrollar una aplicación web que implemente una **cola virtual**: los usuarios se unen a un evento, reciben un enlace único con su número de turno y esperan para comprar boletos.

Además, quiere poder: Crear eventos, asignar actores con perfiles propios, ofrecer espacios interactivos por evento donde el público y los actores puedan conversar.

---

## 💡 La Solución

**“Teatro Mora Virtual”** será una aplicación web que permita a María gestionar eventos teatrales y ventas de boletos de forma eficiente y accesible desde cualquier dispositivo.

- Los usuarios deberán crear un perfil con login y contraseña para poder comprar boletos.
- María podrá crear eventos ingresando detalles como nombre, fecha, hora y descripción.
- Podrá asignar actores desde una lista de perfiles que ella misma gestionará (cada actor tendrá un nombre, biografía y foto).

Cada evento tendrá una página de detalles que incluirá:
- Información del evento,
- Botón de “Unirse a la cola virtual” (habilitado una hora antes de la venta),
- Foro interactivo donde los usuarios con perfil podrán hacer preguntas y los actores o María podrán responder.

---

## ⏳ Funcionamiento de la Cola Virtual
- Una hora antes de la venta, los usuarios con perfil se unen al evento.
- Reciben un número de turno.
- Esperan en tiempo real hasta que les toque comprar.
- El sistema mostrará un contador de espera y notificará cuando llegue su turno.
- Podrán seleccionar asientos y completar la compra dentro de un límite de tiempo.

Los foros permitirán interacción pública, con mensajes visibles para todos los usuarios registrados.

---

## 🎯 Misión

Proporcionar una herramienta eficiente y confiable para gestionar eventos teatrales y ventas de boletos, mejorando la experiencia del público del teatro de María mediante una **cola virtual robusta** y **foros interactivos**.

---

## 👁️ Visión

Ser la solución definitiva para teatros medianos, optimizando la venta de boletos y fomentando la interacción entre actores y público a través de una plataforma digital moderna.

---

## 💬 Principios

- 🎟️ **Simplicidad y accesibilidad:** Facilitar la gestión de eventos y la compra de boletos para usuarios con distintos niveles de experiencia tecnológica.
- 🔒 **Confiabilidad:** Garantizar que el sistema soporte alta demanda sin colapsos y ofrezca una experiencia fluida.
- 💬 **Interactividad:** Promover la conexión entre actores y público mediante foros dinámicos.

---

## 🛠️ Requerimientos del Sistema

- 👥 Registro de usuarios con perfil (login/password) obligatorio para comprar boletos y participar en foros.
- 🎫 Interfaz para María para crear eventos (nombre, fecha, hora, descripción) y asignar actores desde una lista de perfiles gestionados.
- 🎭 Gestión de perfiles de actores por María (nombre, biografía, foto), visibles en los detalles de cada evento.
- 📄 Página de detalles por evento con:
  - Información del evento,
  - Botón “Unirse a la cola virtual” (activo 1 hora antes de la venta),
  - Foro interactivo.
- ⏱️ Cola virtual simulada en tiempo real:
  - Usuarios se unen,
  - Reciben enlace único con número de turno,
  - Ven contador de espera,
  - Son notificados al llegar su turno para comprar.
- 🪑 Selección de asientos y compra de boletos dentro del turno asignado, con límite de tiempo para completar la transacción.
- 💬 Foro interactivo por evento:
  - Usuarios registrados hacen preguntas,
  - Actores o María responden,
  - Mensajes públicos visibles para todos.
- 🛠️ Interfaz administrativa para María para editar eventos, actores y moderar foros (eliminar mensajes si es necesario).
- 🔐 Seguridad básica de datos (protección de perfiles y transacciones).
- 📱 Diseño responsive para uso en computadoras y dispositivos móviles.

---
