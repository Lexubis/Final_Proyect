markdown
# 📱 Proyecto Android — App Multi‑Intents

*Versión del proyecto:* 1.0  
*Versión mínima de Android:* Android 7.0 (API 24)  
*Versión Gradle (AGP):* 8.5.0  
*IDE:* Android Studio Giraffe o superior

---

## 🧩 Resumen del proyecto

Esta aplicación fue desarrollada en *Android Studio, utilizando **Java* y *Material Design Components*.  
Su objetivo es demostrar el uso de *intents implícitos y explícitos, así como el manejo del **ciclo de actividades*, menús y permisos básicos.

La app posee una pantalla principal (HomeActivity) desde donde se accede a distintas funcionalidades: perfil, cámara, correo, navegación web, compartir texto, configuración de red, entre otras.  
También incluye una pantalla informativa (AppActivity) que explica brevemente la estructura de la app.

---

## ⚙️ Intents implementados

### 🔹 *Intents Implícitos (5 total)*

|
#
|
Descripción
|
Acción / URI
|
Cómo probarlo
|
|
---
|
--------------
|
--------------
|
----------------
|
|
1
|
**
Abrir sitio web
**
|
Intent.ACTION_VIEW
+
https://www.santotomas.cl
|
Pulsa
**
“Abrir sitio web”
**
en la pantalla principal. Se abrirá el navegador.
|
|
2
|
**
Enviar correo
**
|
Intent.ACTION_SENDTO
+
mailto:
|
Pulsa
**
“Enviar correo”
**
→ se abrirá una app de correo con los datos del usuario.
|
|
3
|
**
Compartir texto
**
|
Intent.ACTION_SEND
(text/plain)
|
Pulsa
**
“Compartir texto”
**
, selecciona una app (por ejemplo WhatsApp).
|
|
4
|
**
Abrir configuración Wi‑Fi
**
|
Settings.ACTION_WIFI_SETTINGS
|
Pulsa
**
“Abrir Configuración WiFi”
**
para abrir los ajustes del sistema.
|
|
5
|
**
Abrir cámara (implícito)
**
|
Launch de
CamaraActivity
(usa la cámara del dispositivo)
|
Pulsa
**
“Abrir Cámara”
**
, se abre la cámara de fotos.
|

---

### 🔹 *Intents Explícitos (3 total)*

|
#
|
Descripción
|
Destino
|
Cómo probarlo
|
|
---
|
--------------
|
----------
|
----------------
|
|
1
|
**
Ir a Perfil
**
|
PerfilActivity
|
Pulsa
**
“Ir a Perfil (resultado)”
**
; podrás editar/retornar el nombre.
|
|
2
|
**
Ir a Vista App (información)
**
|
AppActivity
|
Pulsa
**
“Ir a Vista App”
**
para ver detalles del proyecto.
|
|
3
|
**
Menú → Perfil (opción superior)
**
|
PerfilActivity
vía menú
action_perfil
|
Abre el menú superior y selecciona
**
Perfil
**
.
|

---

## 🧪 Pasos de prueba rápida

1. *Compila y ejecuta la app* desde Android Studio (o instala el APK debug).
2. En la pantalla de inicio de sesión (si aplica), accede al *Home*.
3. Prueba los botones uno por uno:
    - *Ir a Perfil:* navega y regresa con datos.
    - *Abrir sitio web:* se abre una nueva pestaña del navegador.
    - *Enviar correo:* se lanza la app de correo.
    - *Compartir texto:* menú de compartir del sistema.
    - *Abrir Cámara:* se activa la cámara del dispositivo.
    - *Abrir Configuración WiFi:* abre directamente los ajustes del sistema.
    - *Ir a Vista App:* muestra la información del proyecto.
4. Desde la barra superior *menú⋮*, también se puede navegar entre las acciones.

---

## 🖼️ Capturas de pantalla

(Guarda tus imágenes en una carpeta /screenshots dentro del proyecto y enlázalas aquí)

|
Pantalla
|
Imagen
|
|
-----------
|
--------
|
|
Inicio de sesión
|
!
[
login
](
screenshots/login.png
)
|
|
Menú principal
|
!
[
home
](
screenshots/home.png
)
|
|
Perfil del usuario
|
!
[
perfil
](
screenshots/perfil.png
)
|
|
Vista informativa (AppActivity)
|
!
[
info
](
screenshots/app.png
)
|