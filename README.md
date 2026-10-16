Espiral
Emulador de Dreamcast para PlayStation 4, por Cajaritohh.
Espiral está basado en Flycast y en el port para PS4 Resonance, que usa gráficos Vulkan gracias al port RADV de DolphinPS4. Tiene interfaz propia, temas animados y actualizaciones automáticas desde este repositorio.
Características
Dreamcast, además de NAOMI y Atomiswave (arcade).
Gráficos por Vulkan: puedes subir la resolución sin perder casi rendimiento.
Formatos: CHD, GDI, CDI y otros que soporta Flycast.
Pantalla de inicio con carátulas en 3D y 5 temas: Espiral, Órbita, Canal, Estante y Barra cruzada.
Menús en español y en 13 idiomas más.
Partidas guardadas por slot (save states), tarjetas de memoria (VMU), trucos y parches (60 fps, pantalla ancha).
Juegos desde la red (carpetas compartidas NFS y SMB).
Actualizaciones desde la propia consola.
Requisitos
PS4 con GoldHEN.
Opcional: BIOS de Dreamcast. Sin BIOS funciona igual con la BIOS integrada (HLE), pero algunos juegos andan mejor con la original.
Instalación
Descarga el `.pkg` de la sección Releases de esta página.
Cópialo a la PS4, por ejemplo por FTP a `/data/pkg`, o desde un USB.
Instálalo con el Package Installer de GoldHEN.
Abre Espiral desde el menú de la PS4. La primera vez crea su carpeta `/data/Espiral`.
Dónde va cada cosa
Todo vive en `/data/Espiral`, accesible por FTP:
Carpeta	Para qué
`/data/Espiral/games`	Tus juegos (`.chd`, `.gdi`, `.cdi`…). Pueden ir en subcarpetas.
`/data/Espiral/data`	BIOS: `dc_boot.bin` y `dc_flash.bin`. Para arcade: `naomi.zip`, `awbios.zip`. Aquí también quedan las partidas guardadas y las VMU.
`/data/Espiral/covers`	Tus propias carátulas: `<nombre del juego>.png` o `.jpg`. Si no hay, se descargan solas.
`/data/Espiral/cheats`	Trucos `.cht` o `.txt`.
`/data/Espiral/patches`	Parches propios por juego.
Uso
En la pantalla de inicio:
Izquierda / Derecha: elegir juego.
L1 / R1: saltar de 5 en 5.
✕: jugar.
□: cambiar de tema.
R3: volver a buscar juegos.
△: ajustes.
Durante el juego: presiona el touchpad (o L3 + R3) para abrir el menú rápido, que tiene:
Reanudar.
Guardar y cargar partida (por slot).
Trucos y parches.
Cambiar disco.
Mostrar FPS.
Volumen.
Ajustes.
Cerrar juego.
Ajustes:
Video: resolución, pantalla ancha, filtros, frecuencia de cuadros.
Audio: volumen y procesador de sonido.
Controles: mandos y dispositivos en los puertos de la Dreamcast.
Sistema: región, idioma, BIOS, CPU.
Pantalla de inicio: tema, idioma, carátulas.
Tarjetas de memoria: ver, copiar y borrar partidas de las VMU.
Biblioteca en red: juegos en carpetas NFS/SMB de tu PC o NAS.
Controles arcade: monedas y botones de NAOMI/Atomiswave.
Acerca de: versión y buscar actualizaciones.
Actualizar
En Espiral, entra a Ajustes → Acerca de → Buscar actualizaciones. También busca solo al abrir la app.
Si hay una versión nueva, presiona ✕. Se descarga a `/data/pkg`.
Instálala con el Package Installer de GoldHEN. Tus juegos, partidas y ajustes no se pierden.
Problemas
Si algo falla, los registros quedan en `/data/Espiral`: `boot-trace.log`, `crash.log` y `flycast.log`. Adjúntalos al reportar el problema en la pestaña Issues de este repositorio.
Créditos y licencia
Flycast: flyinghead y colaboradores.
Resonance: iHaiDeeZ.
Port RADV/Vulkan de DolphinPS4.
Mesa, Dear ImGui, libnfs, libsmb2, OpenOrbis.
Espiral se distribuye bajo la licencia GPL-2.0, igual que Flycast. No incluye juegos ni BIOS: usa solo copias de tus propios discos.
