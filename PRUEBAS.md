# Informe de Pruebas - Mommy Eventos

Este documento presenta las pruebas realizadas a los principales módulos del sistema web Mommy Eventos.

---

## 📊 Configuraciones utilizadas

- **Servidor local**: Live Server / Vite
- **Hosting**: Netlify
- **Base de datos**: No relacional (envío por EmailJS o Formspree)
- **Navegadores probados**: Chrome, Firefox, Edge
- **Dispositivos**: Escritorio, tablet y celular

---

## 🔧 Pruebas por módulo

### 1. Formulario de Reservas
- ✅ Envió exitoso con datos completos
- ⚠️ Error visual al dejar campos vacíos
- ✅ Formato de fecha correcto (Flatpickr)
- ✅ Estilos responsive correctos

### 2. Formulario de Contacto
- ✅ Mensaje enviado correctamente vía EmailJS
- ⚠️ Simulación de error si no hay conexión

### 3. Navbar y enlaces
- ✅ Funcionamiento correcto en todos los botones
- ✅ Despliegue correcto en pantalla pequeña

### 4. Galería
- ✅ Carga correcta de imágenes
- ✅ Interacción fluida con efecto de zoom

### 5. Login y Registro
- ✅ Validación de campos completa
- ⚠️ Advertencia si contraseñas no coinciden
- ✅ Redirección funcional

---

## 🌐 Ambientes de prueba

- **Desarrollo**: VSCode + Live Server (localhost)
- **Pruebas online**: Despliegue en Netlify (preview + producción)
- **Producción**: mommy-eventos.netlify.app

---

## 🔓 Resultados

| Módulo       | Resultado | Comentarios                       |
|--------------|-----------|-----------------------------------|
| Reservas     | ✅       | Opera correctamente en todos los campos |
| Contacto     | ✅       | El envío vía email es exitoso     |
| Galería      | ✅       | Todas las imágenes se muestran bien |
| Login        | ✅       | Validación y redirección correcta  |
| Registro     | ✅       | Mensajes y coincidencia funcional |

---

## 📊 Conclusión

El sistema cumple correctamente sus funciones principales. Todas las pruebas de los módulos fueron superadas con éxito en el entorno de pruebas y producción.

