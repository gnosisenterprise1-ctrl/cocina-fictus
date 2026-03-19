# Guía de Configuración: Sincronización Real-Time (Firebase)

Para que el panel de cocina (`admin.html`) y el menú del cliente (`index.html`) estén conectados en tiempo real, debes seguir estos pasos para obtener tus credenciales gratuitas de Firebase.

### 1. Crear el Proyecto en Firebase
1. Ve a [console.firebase.google.com](https://console.firebase.google.com/).
2. Haz clic en **"Agregar proyecto"** y nómbralo `Cocina Fictus Pro`.
3. (Opcional) Desactiva Google Analytics para este proyecto si quieres una configuración más rápida.

### 2. Crear una Aplicación Web
1. En el panel lateral del proyecto, haz clic en el icono de **Web (`</>`)**.
2. Registra la app como `Fictus Web`.
3. Al finalizar, Firebase te mostrará un objeto llamado `firebaseConfig`. **Cópialo**.

### 3. Activar la Base de Datos (Realtime Database)
1. En el menú lateral de Firebase, ve a **Compilación** > **Realtime Database**.
2. Haz clic en **"Crear base de datos"**.
3. Selecciona la ubicación más cercana (ej: `us-central1`).
4. **IMPORTANTE:** Selecciona **"Comenzar en modo de prueba"** para que los pedidos puedan entrar sin restricciones iniciales de seguridad.

### 4. Actualizar el Código
Abre `index.html` y `admin.html` en un editor de texto (como Notepad o VS Code).
Busca la sección que dice:
```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  ...
};
```
Reemplaza todo ese bloque con el que copiaste en el paso 2. **Guarda los cambios.**

---

### ✅ ¡Listo!
Ahora, cuando alguien haga un pedido en la web, la base de datos de Firebase se actualizará y la campana sonará en tu panel administrativo de inmediato, sin importar en qué parte del mundo estén los dispositivos.
