
# 📱 Proyecto Android — App Multi‑Intents

**Versión del proyecto:**1.0  
**Versión mínima de Android:**Android7.0(API24)  
**Versión de Gradle (AGP):**8.5.0  
**IDE:**AndroidStudioGiraffeosuperior

---

## 🧩 Resumen del proyecto

Esta aplicación fue desarrollada en **AndroidStudio**, utilizando **JavayMaterialDesignComponents**.  
Su objetivo es demostrar el uso de **intents implícitos y explícitos**, así como el manejo del **ciclo de actividades**, menús y permisos básicos.

La app posee una pantalla principal (`HomeActivity`) desde donde se accede a distintas funcionalidades: perfil, cámara, enviar correo, navegador web, compartir texto y configuración de redWi‑Fi.  
También incluye una pantalla informativa (`AppActivity`) que explica brevemente la estructura y propósito de la aplicación.

---

## ⚙️ Intents implementados

### 🔹 **Intentsimplícitos(5total)**

| Descripción | Acción/URI | Cómoprobarlo |
|--------------|--------------|----------------|
| **Abrirsitioweb** | `Intent.ACTION_VIEW` +https://www.santotomas.cl | Pulsa **"Abrirsitioweb"**→se abre el navegador. |
| **Enviarcorreo** | `Intent.ACTION_SENDTO` +`mailto:` | Pulsa **"Enviarcorreo"**→se abre la appdecorreo con los datos delusuario. |
| **Compartirtexto** | `Intent.ACTION_SEND`(text/plain) | Pulsa **"Compartirtexto"**→elige una app(p.ej.WhatsApp). |
| **Abrircámara** | `Intent.ACTION_IMAGE_CAPTURE` | Pulsa **"AbrirCámara"**→abre la cámara deldispositivo. |
| **ConfiguraciónWi‑Fi** | `Settings.ACTION_WIFI_SETTINGS` | Pulsa **"AbrirConfiguraciónWi‑Fi"**→abre losajustesdelsistema. |

---

### 🔹 **Intentsexplícitos(3total)**

| Descripción | Destino | Cómoprobarlo |
|--------------|----------|----------------|
| **IraPerfil** | `PerfilActivity` | Pulsa **"IraPerfil(resultado)"**→editaelnombrey vuelvealHome. |
| **IraVistaApp** | `AppActivity` | Pulsa **"IraVistaApp"**→muestrainformacióndelproyecto. |
| **Menú→Perfil** | `PerfilActivity` | Abreelmenúsuperiory selecciona**Perfil**. |

---

## 🧪 Pasos de prueba rápida

1. **Compila y ejecuta la app** desde AndroidStudio o instala el APKdebug.
2. En la pantalla de iniciodesesión (si aplica), accedeal**Home**.
3. Prueba los botones uno por uno:

   - **IraPerfil**→navegayregresacondatoseditados.
   - **Abrirsitioweb**→abreunanuevapestañadelnavegador.
   - **Enviarcorreo**→lanzaclientedecorreo.
   - **Compartirtexto**→muestraelselectordelsistema.
   - **AbrirCámara**→activalacámaradeldispositivo.
   - **AbrirConfiguraciónWi‑Fi**→abrelosajustesdelsistema.
   - **IraVistaApp**→muestrainformacióndelproyecto.

4. Usa la barra superior (**menú⋮**) para accederaacciones adicionales.

---

## 💻 Fragmentos de código clave

**Intentexplícito→PerfilActivity**
```java
Intent i = new Intent(HomeActivity.this, PerfilActivity.class);
i.putExtra("email_usuario", emailUsuario);
editarPerfilLauncher.launch(i);
Contraer
readme.txt
4 KB
﻿
momo de tuais
Purtaco
purtaco
He/Him
 
 
Trans male
Constantly struggling
Be gentle, I'm sensitive
# 📱 Proyecto Android — App Multi‑Intents

**Versión del proyecto:** 1.0  
**Versión mínima de Android:** Android 7.0 (API 24)  
**Versión de Gradle (AGP):** 8.5.0  
**IDE:** Android Studio Giraffe o superior  

---

## 🧩 Resumen del proyecto

Esta aplicación fue desarrollada en **Android Studio**, utilizando **Java y Material Design Components**.  
Su objetivo es demostrar el uso de **intents implícitos y explícitos**, así como el manejo del **ciclo de actividades**, menús y permisos básicos.

La app posee una pantalla principal (`HomeActivity`) desde donde se accede a distintas funcionalidades: perfil, cámara, enviar correo, navegador web, compartir texto y configuración de red Wi‑Fi.  
También incluye una pantalla informativa (`AppActivity`) que explica brevemente la estructura y propósito de la aplicación.

---

## ⚙️ Intents implementados

### 🔹 **Intents implícitos (5 total)**

| Descripción | Acción / URI | Cómo probarlo |
|--------------|--------------|----------------|
| **Abrir sitio web** | `Intent.ACTION_VIEW` + https://www.santotomas.cl | Pulsa **"Abrir sitio web"** → se abre el navegador. |
| **Enviar correo** | `Intent.ACTION_SENDTO` + `mailto:` | Pulsa **"Enviar correo"** → se abre la app de correo con los datos del usuario. |
| **Compartir texto** | `Intent.ACTION_SEND` (text/plain) | Pulsa **"Compartir texto"** → elige una app (p.ej. WhatsApp). |
| **Abrir cámara** | `Intent.ACTION_IMAGE_CAPTURE` | Pulsa **"Abrir Cámara"** → abre la cámara del dispositivo. |
| **Configuración Wi‑Fi** | `Settings.ACTION_WIFI_SETTINGS` | Pulsa **"Abrir Configuración Wi‑Fi"** → abre los ajustes del sistema. |

---

### 🔹 **Intents explícitos (3 total)**

| Descripción | Destino | Cómo probarlo |
|--------------|----------|----------------|
| **Ir a Perfil** | `PerfilActivity` | Pulsa **"Ir a Perfil (resultado)"** → edita el nombre y vuelve al Home. |
| **Ir a Vista App** | `AppActivity` | Pulsa **"Ir a Vista App"** → muestra información del proyecto. |
| **Menú → Perfil** | `PerfilActivity` | Abre el menú superior y selecciona **Perfil**. |

---


## 🧪 Pasos de prueba rápida

1. **Compila y ejecuta la app** desde Android Studio o instala el APK debug.  
2. En la pantalla de inicio de sesión (si aplica), accede al **Home**.  
3. Prueba los botones uno por uno:

   - **Ir a Perfil** → navega y regresa con datos editados.  
   - **Abrir sitio web** → abre una nueva pestaña del navegador.  
   - **Enviar correo** → lanza cliente de correo.  
   - **Compartir texto** → muestra el selector del sistema.  
   - **Abrir Cámara** → activa la cámara del dispositivo.  
   - **Abrir Configuración Wi‑Fi** → abre los ajustes del sistema.  
   - **Ir a Vista App** → muestra información del proyecto.  

4. Usa la barra superior (**menú⋮**) para acceder a acciones adicionales.

---

## 💻 Fragmentos de código clave

**Intent explícito → PerfilActivity**
```java
Intent i = new Intent(HomeActivity.this, PerfilActivity.class);
i.putExtra("email_usuario", emailUsuario);
editarPerfilLauncher.launch(i);