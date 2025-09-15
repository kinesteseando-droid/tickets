[README_Version3.md](https://github.com/user-attachments/files/22348502/README_Version3.md)
# Kinesteseando Tickets - Panel Administrativo

Sistema web para gestión de eventos y tickets usando Google Sheets como base de datos y Google Apps Script como backend.

---

## 🚀 ¿Qué es esto?

Una app administrativa para manejar eventos, usuarios y tickets desde cualquier dispositivo, con toda la información guardada en tu Google Sheets.

---

## 🛠️ Instrucciones de instalación y uso

### 1. Prepara tu Google Sheets

- Crea una nueva hoja de cálculo en [Google Sheets](https://sheets.google.com).
- Abre **Extensiones > Apps Script**.
- Borra cualquier código de ejemplo y **pega el script** que encuentras en este repositorio como `Code.gs`.
- Guarda el proyecto.

**Publica el Apps Script como WebApp:**

1. Haz clic en `Implementar > Nueva implementación`.
2. Selecciona **Tipo: Aplicación web**.
3. Ponle un nombre (ejemplo: "API Tickets").
4. **Acceso:** selecciona “Cualquiera” (Anyone).
5. Haz clic en **Implementar** y autoriza los permisos.
6. Copia la **URL del WebApp** (la necesitarás en el frontend).

---

### 2. Consigue tu Spreadsheet ID y API Key

- **Spreadsheet ID:**  
  Está en la URL de tu hoja:  
  `https://docs.google.com/spreadsheets/d/SPREADSHEET_ID/edit`
- **API Key:**  
  1. Ve a [Google Cloud Console](https://console.cloud.google.com/).
  2. Crea un proyecto o usa uno existente.
  3. Habilita **Google Sheets API**.
  4. Ve a “APIs y servicios > Credenciales” y crea una **clave de API**.

---

### 3. Configura el Frontend (`index.html`)

- Este archivo ya tiene pre-configurado tu Spreadsheet ID, API Key y Proxy URL.  
  Si necesitas cambiarlos, edítalos en el HTML directamente.
- **No necesitas configurar nada extra** si usas los valores que ya están.

---

### 4. Sube el frontend a GitHub y activa Pages

1. Sube el archivo `index.html` (y este `README.md`) a tu repositorio en GitHub, por ejemplo: [`kinesteseando-droid/tickets`](https://github.com/kinesteseando-droid/tickets).
2. Ve a **Settings > Pages**.
3. En **Source**, elige la rama principal (`main`) y la carpeta `/` (root).
4. Guarda.  
   GitHub te dará una URL como:  
   `https://kinesteseando-droid.github.io/tickets/`

---

### 5. ¡Accede y comienza a usarlo!

- Ingresa a la URL pública (de GitHub Pages).
- Administra eventos, usuarios y tickets desde cualquier navegador.
- Todo queda guardado y sincronizado en tu Google Sheets.

---

## ℹ️ Notas

- **Seguridad:** Si quieres agregar protección extra, implementa validaciones en tu Apps Script.
- **Personalización:** Puedes editar el diseño y funciones en `index.html`.
- **Respaldo:** Los datos siempre estarán en tu Google Sheets, ¡haz backups si lo necesitas!

---

## 📄 Archivos incluidos

- `index.html`: Panel administrativo listo para usar.
- `Code.gs`: Script para pegar en tu Apps Script de Google Sheets.
- `README.md`: Esta guía de instalación y uso.

---

## 💬 Soporte

¿Tienes mejoras o dudas?  
Crea un issue en este repo o contacta al equipo de Kinesteseando.
