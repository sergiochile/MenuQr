# 🕹 CÓMO PUBLICAR LA CARTA EN INTERNET (GRATIS)

## OPCIÓN 1 — GitHub Pages (recomendado, URL permanente gratis)

### Paso 1 — Crea una cuenta en GitHub
👉 https://github.com/signup (si ya tienes, salta este paso)

### Paso 2 — Crea un repositorio nuevo
1. Ve a https://github.com/new
2. Nombre del repositorio: `carta-mundorumviator`
3. Ponlo en **Public**
4. Haz clic en **Create repository**

### Paso 3 — Sube los archivos
Abre la Terminal y ejecuta estos comandos uno a uno:

```bash
cd "/Users/sergecchile./Desktop/PROYECTOS WEB/Carta-Mundorumviator"
git init
git add .
git commit -m "Carta digital Mundorum Viator"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/carta-mundorumviator.git
git push -u origin main
```
(Cambia TU-USUARIO por tu nombre de GitHub)

### Paso 4 — Activa GitHub Pages
1. En GitHub, ve a tu repositorio → **Settings** → **Pages**
2. En "Source" selecciona **main** y carpeta **/ (root)**
3. Haz clic en **Save**
4. En 1-2 minutos tu URL estará disponible:
   `https://TU-USUARIO.github.io/carta-mundorumviator/`

### Paso 5 — Actualiza el QR
Abre `qr.html` y cambia la línea:
```js
const URL_CARTA = 'https://TU-USUARIO.github.io/carta-mundorumviator/mundorum_viator_carta_animada.html';
```

### Paso 6 — Imprime el QR
1. Abre `qr.html` en el navegador
2. Haz clic en **🖨 IMPRIMIR QR**
3. ¡Colócalo en las mesas del bar!

---

## OPCIÓN 2 — Netlify (drag & drop, aún más fácil)

1. Ve a https://app.netlify.com/drop
2. Arrastra la carpeta `Carta-Mundorumviator` al navegador
3. Netlify te da una URL tipo: `https://nombre-random.netlify.app`
4. Actualiza la URL en `qr.html` y vuelve a subir

---

## ARCHIVOS DEL PROYECTO

- `mundorum_viator_carta_animada.html` → La carta interactiva (la que escanean)
- `qr.html` → El cartel con QR para imprimir y poner en las mesas
- `Restaurant_Menu_Design_In_a_pixel_art_style_this_is_a_digital_menu_for_q5xG72yD.png` → Imagen de la carta

