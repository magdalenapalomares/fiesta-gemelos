🎂 Invitación de Cumpleaños: 
Mauricio y Patricio (4 Años)
Esta es una aplicación web de invitación electrónica totalmente funcional, diseñada para el cuarto cumpleaños de los gemelos Mauricio y Patricio. Incluye gestión de invitados en tiempo real, ubicación y mesa de regalos.

✨ Características
Diseño Premium y Responsivo: Optimizado para dispositivos móviles (WhatsApp) usando Tailwind CSS.
Confirmación RSVP: Formulario integrado que guarda la asistencia directamente en la nube.
Mesa de Regalos: Enlaces directos a Amazon Wishlist y modal interactivo para el código de barras de Liverpool.
Ubicación: Integración con Google Maps para llegar a "Hashiko Bahías".
Panel de Administración Privado:
Protegido por contraseña.
Visualización de invitados en tiempo real.
Contador automático de personas confirmadas.
Descarga de la lista completa en formato CSV (Excel).

🚀 Tecnologías Utilizadas
Frontend: HTML5, CSS3 (Tailwind CSS).
Iconos: Lucide Icons.
Backend: Firebase (Firestore para base de datos y Authentication para acceso anónimo).
🛠️ Configuración Necesaria

Para que la base de datos funcione en tu propia cuenta, debes realizar estos pasos:
Firebase Console:
Crea un proyecto en Firebase.
Habilita Firestore Database en modo de prueba.
Habilita Anonymous Sign-in en la sección de Authentication.

Reglas de Firestore:
Copia y pega estas reglas en la pestaña "Rules" de tu base de datos:
rules_version = '2';
service cloud.firestore {
  match /databases/{database}/documents {
    match /{document=**} {
      allow read, write: if true;
    }
  }
}

Archivo index.html:
Busca el objeto myManualConfig (alrededor de la línea 161).
Reemplaza los valores con las credenciales de tu "Web App" de Firebase.

📦 Despliegue Rápido

Opción A: Netlify Drop (La más fácil)
Pon el archivo index.html dentro de una carpeta.
Arrastra la carpeta a Netlify Drop.
¡Copia el link y compártelo por WhatsApp!

Opción B: GitHub Pages
Sube el archivo index.html a un repositorio de GitHub.
Ve a Settings > Pages.
En "Branch", selecciona main y guarda. Tu sitio estará disponible en minutos.
Nota para el Administrador: Para ver los asistentes, haz clic en el botón "Acceso Papás" al final de la invitación e ingresa la clave maestra.
