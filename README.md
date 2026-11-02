# CORTEX 6.0

Cripto y deportes en vivo en una app Android nativa, escrita en Java puro y compilada sin Gradle
(aapt2 + javac + d8 + apksigner). Android 7 o superior.

## Lo que tiene

- **Cripto**: precios al segundo de BTC, ETH, SOL, BNB y USDT desde Kraken, grafica de 30 dias
  con velas reales, maximo y minimo del periodo, y variacion con color.
- **Deportes**: marcadores en directo con API-Football (la clave se pone en Ajustes) y respaldo
  con TheSportsDB. El minuto avanza solo.
- **IA**: analisis de jugadas con Poisson y su explicacion en lenguaje claro.
- **IPTV**: lector de listas M3U con las categorias y canales de la lista que cargues.
- **Ajustes**: cantidades de cada moneda, clave de deportes y lista de IPTV.

Sin cuentas, sin registro y sin datos personales. Solo se guarda en el telefono lo que tu escribes.

## Diseño

Paleta clara: fondo azul muy suave, tarjetas blancas con borde fino, texto oscuro y azul de
confianza. Verde para lo que sube, rojo para lo que baja. Todos los colores estan en una sola
clase (`Paleta.java`) y en `values/colores.xml`.

## Versiones

| Version | Que cambio |
|---------|------------|
| 6.0 | Fuera login, usuarios y panel familiar. Tema claro. Grafica real de velas de Kraken. |
| 5.0 | Precios al segundo con Kraken, IPTV, animacion de pulsacion, analisis de jugadas. |
| 4.3 | API-Football con control de cupo y contador de peticiones. |
| 2.2 | Reintentos y cache para CoinGecko; deportes reales con TheSportsDB. |
| 1.0 | Primera version con cartera, analisis tecnico y deportes. |

## Aviso

El APK se compila con la clave de API-Football que pongas en `ClienteDeportes.CLAVE_POR_DEFECTO`.
Si esa clave esta escrita en el codigo, viaja dentro del APK y cualquiera que lo tenga puede leerla.
Para un APK publico, dejala vacia y ponla desde Ajustes en el telefono.

Las cantidades y los avisos de este proyecto son informativos, no son consejo financiero ni de apuestas.
