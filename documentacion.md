# Documentación de Módulos y Componentes - Mommy Eventos

Esta documentación describe los módulos del sistema web de Mommy Eventos, incluyendo entradas, salidas y comportamientos esperados.

---

## Módulo: Formulario de Reservas (reservas.html)

- **Entradas**:
  - Nombre, teléfono, email (string)
  - Fecha, hora (date / select)
  - Temática (select)
  - Invitados (número)
  - Comentarios (texto libre)
  - Método de pago (radio)

- **Salidas esperadas**:
  - Validación visual de campos
  - Alerta de éxito si se envía correctamente
  - Resumen de reserva actualizado

---

## Módulo: Formulario de Contacto (contacto.html)

- **Entradas**:
  - Nombre, correo, asunto, mensaje

- **Salidas esperadas**:
  - Validación de campos requeridos
  - Envío de correo (vía EmailJS o Formspree)
  - Alerta de confirmación o error

---

## Módulo: Navegación (Navbar en todas las páginas)

- **Componentes**:
  - Enlaces a páginas
  - Botones "Ingresar" y "Registrarse"
  - Comportamiento responsive

---

## Módulo: Login (login.html)

- **Entradas**:
  - Email, contraseña

- **Salidas esperadas**:
  - Autenticación exitosa simula acceso
  - Redirección a página de inicio o dashboard

---

## Módulo: Registro (registro.html)

- **Entradas**:
  - Nombre, email, contraseña, confirmación

- **Salidas esperadas**:
  - Validación de coincidencia de contraseña
  - Alerta de registro exitoso
  - O redirección a login

---

## Módulo: Galería (galeria.html)

- **Entradas**:
  - Interacción del usuario

- **Salidas esperadas**:
  - Ampliación de imágenes
  - Navegación entre imágenes (opcional con lightbox)

---

## Componente: Calendario (Flatpickr)

- **Ubicación**: reservas.html
- **Entradas**: fecha
- **Salidas**: fecha seleccionada mostrada en resumen

---

## Componente: Botón WhatsApp flotante

- **Función**: enlace directo a WhatsApp para contacto rápido
- **Entrada**: click del usuario
- **Salida**: abre WhatsApp Web

---

## Estilos (Main.css)

- Contiene reglas globales de diseño: fuentes, botones, colores, espaciado, etc.
- Responsivo y basado en Bootstrap 5

---

## Script principal (Main.js)

- Inicializa tooltips y validaciones
- Controla comportamiento de formularios
- Carga dinámica de resumen de reservas

