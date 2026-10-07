# Olivia Fest — cómo ponerla en línea

Archivos: **index.html** (la invitación) · **admin.html** (tu panel) · **config.js** (donde pegas la URL de la hoja) · **Codigo.gs** (la hoja de Google) · **fotos/** (tus fotos).

## 1. Hoja de Google (5 min)
1. Crea una hoja **nueva** en Google Sheets llamada *Olivia Fest*.
2. **Extensiones → Apps Script** → borra todo y pega el contenido de **Codigo.gs**.
3. Cambia `CAMBIA-ESTA-CLAVE` por tu clave (la usarás para entrar al panel).
4. Elige la función **configurar** → **Ejecutar** → acepta los permisos.
5. **Implementar → Nueva implementación → Aplicación web** · Ejecutar como: **Yo** · Acceso: **Cualquier usuario** → Implementar.
6. Copia la URL que termina en **/exec**.

## 2. Pega la URL (un solo lugar)
Abre **config.js**, pega la URL entre las comillas de `api: ""` y guarda. Sirve para la invitación y para el panel.

## 3. Fotos (carpeta fotos, .jpg, ~1200 px y menos de 1 MB)
- Álbum del libro: `mes1.jpg` … `mes12.jpg`
- Nuestra princesa: `olivia1.jpg` … `olivia10.jpg` (las que tengas)
- Nuestra familia: `familia1.jpg` … `familia8.jpg` (las que tengas)
Si falta una foto, se queda el marco decorado.

## 4. Subir a GitHub y publicar
1. github.com → **New repository** → nombre **olivia-fest** → **Public** → Create.
2. **uploading an existing file** → arrastra **todo el contenido** de la carpeta (incluida *fotos*) → **Commit changes**.
3. **Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save**.
4. En unos minutos (hasta 10) queda en:
   - Invitación: `https://gianfrancorondon01.github.io/olivia-fest/`
   - Panel: `https://gianfrancorondon01.github.io/olivia-fest/admin.html`

## 5. Lista de invitados y pases
En la pestaña **Invitados** de la hoja (o desde el panel): columna A el nombre del invitado (ej. *Pepito Pérez*), columna B sus pases (ej. *2* si va con su esposa, *4* si va con su familia).
- Con la lista cargada, **solo confirman las personas de la lista** y cada una ve únicamente los pases que tiene (1, 2, 4…).
- Si tiene **1 pase**, solo elige *Sí* o *No*. Si tiene **2 o más**, elige cuántos usará y escribe el nombre de cada acompañante.
- Si la lista está vacía (pruebas), cualquiera puede confirmar hasta 4 personas.
- En el panel, **Copiar enlace** crea un enlace personal que saluda al invitado por su nombre.

## 6. Fotos de los regalos
Cada regalo puede tener foto: ponla en `fotos/regalos/` con el nombre que indica `fotos/regalos/LEEME.txt` (ej. `jug-mesa.jpg`). Si falta, se ve un icono.

## 7. Si ya habías creado la hoja con una versión anterior
Borra la pestaña **Regalos**, pega de nuevo el **Codigo.gs** nuevo, ejecuta **configurar** y publica una versión nueva (Implementar → Administrar implementaciones → ✏️ → Versión nueva).

## 8. Cambiar algo después
- Fotos nuevas o cambios: en GitHub entra a la carpeta → **Add file → Upload files** (los mismos nombres reemplazan a los anteriores).
- Si cambias **Codigo.gs**: Implementar → Administrar implementaciones → ✏️ → Versión nueva (la URL no cambia).
