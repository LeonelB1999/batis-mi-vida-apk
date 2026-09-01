# 😎 Mi Vida — APK Android

App nativa Android (wrapper **Capacitor**) que carga la web de **Mi Vida** en vivo:
`http://129.159.90.187:8080/mivida/`

Cada push a `main` compila el APK automáticamente con **GitHub Actions** y lo publica en
**Releases** → descarga e instala directamente en tu celular.

## Descargar el APK

👉 https://github.com/LeonelB1999/batis-mi-vida-apk/releases/latest

- Instala **sobre** versiones anteriores sin desinstalar (mismo `applicationId`)
- Ícono nativo de Mi Vida 😎 (adaptativo + legacy)
- Tema oscuro `#0f172a` en splash y barra de estado

## Stack

- Capacitor 8 + Android (Java 21 en CI)
- La app es un espejo de la web: cualquier mejora en la web llega sola al APK
  (no hay que recompilar por cambios del sistema)

## Build local

```bash
npm install
npx cap sync android
cd android && ./gradlew assembleRelease
```
