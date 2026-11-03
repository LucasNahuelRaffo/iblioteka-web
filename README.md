# iblioteka — web

Landing de la **iblioteka**, estantería modular de diseño por **IRIZAR KON**.

Sitio estático: un `index.html` con sus imágenes en `assets/`. No necesita build ni dependencias.

## Antes de publicar

En `index.html`, buscá esta línea y poné el número real de WhatsApp (código de país + área + número, sin espacios ni `+`):

```js
window.IBLIOTEKA = { whatsapp: '5490000000000', animate: true };
```

También quedan marcados entre corchetes para completar: `[NÚMERO]`, `[DIRECCIÓN DEL SHOWROOM]`, `[DÍAS Y HORARIOS]`, `[LINK GOOGLE MAPS]`, el texto del estudio y la respuesta de precios y envíos.

## Publicar con GitHub Pages

1. Subí el contenido de esta carpeta a la raíz del repositorio `iblioteka-web`.
2. En GitHub: **Settings → Pages → Build and deployment → Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. En unos minutos queda en `https://<usuario>.github.io/iblioteka-web/`.
4. Para usar dominio propio: en la misma pantalla, **Custom domain**, y apuntá el DNS del dominio a GitHub Pages.

También funciona tal cual en Netlify o Vercel (arrastrando la carpeta).

## Probar en local

```bash
python3 -m http.server 8000
```

y abrí `http://localhost:8000`.
