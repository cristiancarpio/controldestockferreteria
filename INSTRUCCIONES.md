# FerrStock — Instrucciones para subir a internet

## ¿Qué vamos a hacer?
1. Crear una cuenta de Google (Gmail) — gratis
2. Activar Firebase (base de datos gratis de Google) — gratis
3. Subir la app a Netlify para que tenga un link fijo — gratis

---

## PASO 1 — Crear una cuenta Gmail (si no tiene)

1. Ir a https://gmail.com
2. Hacer clic en "Crear cuenta"
3. Seguir los pasos (nombre, usuario, contraseña)
4. ¡Listo! Ya tiene Gmail

---

## PASO 2 — Crear la base de datos en Firebase

### 2.1 Entrar a Firebase
1. Ir a https://console.firebase.google.com
2. Iniciar sesión con la cuenta Gmail
3. Hacer clic en "Crear un proyecto"

### 2.2 Crear el proyecto
1. Nombre del proyecto: ferrstock
2. Clic en Continuar
3. Cuando pregunta Google Analytics → elegir NO
4. Clic en "Crear proyecto" y esperar

### 2.3 Crear la base de datos Firestore
1. En el menú izquierdo buscar "Firestore Database"
2. Clic en "Crear base de datos"
3. Elegir "Comenzar en modo de prueba" ← MUY IMPORTANTE
4. Región: us-east1
5. Clic en Habilitar

### 2.4 Obtener las claves
1. Clic en el engranaje ⚙️ arriba a la izquierda
2. "Configuración del proyecto"
3. Bajar a "Tus apps" → clic en el ícono </> (Web)
4. Nombre de app: ferrstock-web
5. NO marcar Firebase Hosting
6. Clic en "Registrar app"
7. Copiar el bloque de código que aparece (apiKey, authDomain, etc.)

---

## PASO 3 — Pegar las claves en index.html

1. Abrir index.html con el Bloc de Notas
2. Buscar: apiKey: "PEGA_TU_apiKey_ACÁ"
3. Reemplazar cada línea con los valores copiados de Firebase
4. Guardar (Ctrl + S)

ANTES:
  apiKey: "PEGA_TU_apiKey_ACÁ",
  authDomain: "PEGA_TU_authDomain_ACÁ",

DESPUÉS (ejemplo):
  apiKey: "AIzaSyBxxxxxxxxxxxxxxxx",
  authDomain: "ferrstock-12345.firebaseapp.com",

---

## PASO 4 — Subir a Netlify

1. Ir a https://netlify.com
2. "Sign up" con Google (mismo Gmail)
3. En la página principal, arrastrar la CARPETA completa
   (la que tiene index.html, manifest.json y sw.js)
   a la zona que dice "Drag and drop your site folder here"
4. Netlify da un link como: https://ferrstock-juan.netlify.app
5. Puede cambiar el nombre en: Site settings → Change site name

---

## PASO 5 — Instalar como app

En el CELULAR (Chrome o Safari):
- Abrir el link de Netlify
- Menú → "Agregar a pantalla de inicio"

En la COMPUTADORA (Chrome):
- Abrir el link de Netlify
- Clic en el ícono ⊕ en la barra de dirección
- Clic en "Instalar"

---

## ¡Listo!
- Los datos se guardan en la nube (Firebase)
- Funciona desde celular, tablet o computadora
- 100% gratis
