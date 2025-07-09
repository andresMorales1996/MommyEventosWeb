# Manual Técnico del Proyecto - Mommy Eventos

Este manual está dirigido a desarrolladores y administradores que deseen mantener o escalar la plataforma web **Mommy Eventos**.

---

## 🔧 Tecnologías

- **Frontend**: HTML5, CSS3, Bootstrap 5.3, JavaScript ES6
- **Backend simulado**: EmailJS / Formspree (contacto y reservas)
- **Despliegue**: Netlify (funciones opcionales con `netlify/functions`)
- **Dependencias**:
  - Animate.css
  - Flatpickr.js
  - FontAwesome

---

## 📝 Instalación y despliegue local

1. Clonar el repositorio:

```bash
git clone git@github.com:andresMorales1996/MommyEventosWeb.git
```

2. Abrir `index.html` con Live Server (VSCode) o navegador.

3. Si se usa Vite/Netlify:

```bash
npm install
npm run dev
```

4. Para funciones (Netlify):

- Crear carpeta `netlify/functions`
- Agregar `sendEmail.js` con la lógica deseada
- Definir variables en `.env` local y Netlify dashboard

---

## 📂 Estructura

```
project/
├── index.html
├── pages/
├── assets/
│   ├── images/
│   └── styles/Main.css
├── Main.js
└── netlify/functions/sendEmail.js
```

---

## 🚹 Configuración del servidor y base de datos

- **Servidor**: Netlify
- **Base de datos**: No se utiliza. Formularios se envían vía correo (API de EmailJS/Formspree)
- **Configuración Netlify**:
  - Ruta de funciones: `netlify/functions`
  - Variables: `ELEVENLABS_API_KEY`, `SERVICE_ID`, `TEMPLATE_ID`

---

## ⚖️ Consideraciones

- El proyecto puede escalarse con backend en Node.js o Firebase
- Puede conectarse a Firestore o MongoDB si se requiere persistencia
- Las funciones actuales solo simulan envíos

---

## 🔐 Seguridad

- Evitar exponer API keys en frontend
- Usar `.env` local y Netlify para proteger tokens

---

## 🔄 Actualización del sistema

- Modificar estilos en `Main.css`
- Ajustar formularios desde `reservas.html` o `contacto.html`
- Agregar páginas al directorio `pages/`

---

## 📄 Mantenimiento

- Revisar enlaces rotos o imágenes faltantes
- Probar el formulario de contacto periódicamente
- Verificar que las dependencias estén actualizadas (Bootstrap, Flatpickr)

---

## 🔗 Enlaces clave

- Sitio desplegado: [https://mommyeventos.netlify.app](https://mommyeventos.netlify.app)
- Repositorio GitHub: [https://github.com/andresMorales1996/MommyEventosWeb](https://github.com/andresMorales1996/MommyEventosWeb)

