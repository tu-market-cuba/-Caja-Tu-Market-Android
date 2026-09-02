# Caja Tu Market para Android

Aplicación Android de Caja Tu Market con impresión Bluetooth directa para la
impresora térmica MHT-P11. No necesita Thermer ni abre anuncios al imprimir.

## Primera instalación

1. Emparejar la MHT-P11 desde los ajustes Bluetooth de la tableta.
2. Instalar y abrir **Caja Tu Market**.
3. Autorizar Bluetooth y cámara cuando Android lo solicite.
4. Conectar internet una vez para descargar productos y dependientes.
5. Realizar una venta y pulsar **Cobrar e imprimir**.

Después de la primera sincronización, la Caja conserva localmente los productos
y dependientes para trabajar sin internet. Las ventas pendientes se sincronizan
cuando vuelve la conexión.

## Compilación

Abrir esta carpeta en Android Studio (JDK 17), esperar la sincronización de
Gradle y seleccionar **Build > Build APK(s)**. El APK se genera en
`app/build/outputs/apk/debug/app-debug.apk`.

Identificador Android: `com.tumarket.caja`

Versión: `1.1.0` (métodos de pago, efectivo y vuelto, pago combinado,
descuentos y devoluciones con clave del dueño, historial, reimpresión y cierre
de turno con resumen imprimible).

## Compilación automática en GitHub

El proyecto incluye `.github/workflows/build-apk.yml`. Al subir el contenido a
la rama `main`, GitHub Actions compila el APK y lo deja disponible como el
artefacto **Caja-Tu-Market-APK**.
