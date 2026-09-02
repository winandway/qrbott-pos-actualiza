# QRBott POS OS — buzón de parches

Aquí viven los parches **firmados** que las cajas QRBott bajan solas
(`manifest.json` + `manifest.json.sig` + `parche-<versión>.tar.gz`).
Cada caja comprueba la firma Ed25519 con la llave pública que trae de fábrica
y la huella SHA-256 del paquete antes de aplicar nada. La llave privada no
está en este repositorio ni en ninguna caja.

Publicar un parche: `cd /Users/windocellc/qrbott-java-pos/os && ./actualiza/publicar-parche.sh "qué trae"`
y subir `os/build/actualiza/` aquí.
