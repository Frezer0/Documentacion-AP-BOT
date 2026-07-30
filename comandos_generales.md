# 📜 Lista General de Comandos

A continuación se detalla la inmensa librería de comandos integrados en Ap BOT v3, clasificados por módulo y función.

> **Nota:** La etiqueta `[Admin]` o `[Mod]` indica que el comando requiere permisos especiales preconfigurados.

---

## 💰 1. Economía y Billeteras
Todo lo relacionado con el balance virtual de plata del gremio.

*   `/saldo` - Muestra tu saldo actual de billetera.
*   `/transferir` - Transfiere saldo a otro jugador.
*   `/movimientos` - Muestra tus movimientos de billetera (historial de transacciones).
*   `/cobrar_diario` - Cobra tu recompensa diaria de billetera.
*   `/tesoreria` `[Admin]` - Muestra saldo acumulado por impuestos y comisiones del gremio.
*   `/balance_total` `[Admin]` - Muestra la suma de todo el dinero que existe actualmente entre todos los jugadores.
*   `/ajustar_saldo` `[Admin]` - Suma o resta saldo a un jugador de forma manual.
*   `/ajustar_saldo_party` `[Admin]` - Reparte un monto total de dinero equitativamente entre los inscritos de una party (ideal para pagos de ZvZ).
*   `/auditar_movimientos` `[Admin]` - Muestra movimientos de un jugador específico.
*   `/revertir_movimiento` `[Admin]` - Revierte una transacción usando su ID (TX ID).
*   `/config_economia` `[Admin]` - Configura parámetros base de la economía (moneda, etc.).
*   `/config_impuestos` `[Admin]` - Configura el impuesto base por transferencia.
*   `/config_comisiones` `[Admin]` - Configura las comisiones del banco por transferencia.

---

## 🛡️ 2. Sistema de Registro Albion
Control y verificación de jugadores usando la API oficial de Albion Online.

*   `/registrar` - Abre el panel para que un usuario se verifique.
*   `/perfil` - Muestra la ficha completa y estadísticas de un jugador registrado.
*   `/albion_stats_user` - Consulta las estadísticas (PVE/PVP) de un jugador directamente en la API.
*   `/albion_stats_guild` - Consulta las estadísticas globales de un gremio.
*   `/agregar_alianza` / `/agregar_nap` - Agrega gremios o alianzas amistosas al registro del bot.
*   `/eliminar` - Elimina un NAP o alianza configurada.
*   `/registrar_jugador` `[Admin]` - Fuerza el registro de un jugador sin que él lo haga manualmente.
*   `/modificar_registro` `[Admin]` - Corrige el personaje registrado de un usuario en la base de datos.
*   `/desregistrar` `[Admin]` - Elimina por completo el registro de Albion de un jugador.
*   `/limpiar_servidor` `[Admin]` - Detecta usuarios registrados que ya no están en el gremio/alianza y permite su expulsión.
*   `/rol_ingreso` `[Admin]` - Configura qué rol se le da a cualquiera que entre al servidor (Ej: Visitante).

---

## ⭐ 3. Reputación y Votos
Sistema social para recompensar o castigar el comportamiento de los jugadores.

*   `/votar_jugador` - Vota por el desempeño de un jugador registrado.
*   `/editar_votos` `[Admin]` - Suma, resta o reinicia manualmente los votos de un jugador.
*   `/config_votos` `[Admin]` - Configura cuántos votos necesita alguien para ser VIP o las recompensas.
*   `/config_ranking` `[Admin]` - Configura y publica el Leaderboard visual de los mejores jugadores.

---

## ⚖️ 4. Sistema de Multas
Sanciones económicas por faltas en ZvZ o reglas del gremio.

*   `/multar_jugador` `[Mod]` - Registra una multa y actualiza el panel del infractor.
*   `/panel_multa` `[Admin]` - Imprime el panel principal donde los jugadores pueden ver y pagar sus multas (`/fine_pay` integrado en botones).
*   `/config_multas` `[Admin]` - Configura reglas y montos estándar de multas.

---

## 🛑 5. Seguridad y Blacklist
Prevención de espías y control de baneos.

*   `/agregar_blacklist` `[Mod]` - Agrega un usuario a blacklist y lo banea localmente.
*   `/quitar_blacklist` `[Mod]` - Remueve un usuario de blacklist.
*   `/lista_baneados` `[Mod]` - Muestra el listado de jugadores baneados en la red de AP BOT.
*   `/ver_blacklist` `[Mod]` - Muestra la evidencia y detalles de un jugador blacklisted.
*   `/config_blacklist` `[Admin]` - Abre el panel interactivo de configuración de seguridad.

---

## 🎮 6. Partys y Composiciones
Todo para organizar ZvZ, ganks y PVE.

*   `/crear_party` - Abre el constructor guiado interactivo para crear una Party.
*   `/auto_ping` - Publica un embed de auto-ping en un canal con composiciones pre-guardadas.
*   `/lanzar_party` - Lanza una composición directamente al canal actual sin pasar por menús.
*   `/mis_compos` - Muestra las composiciones personales guardadas por el Caller.
*   `/crear_categoria` / `/crear_composiciones` - Permite a los Callers guardar plantillas de builds.
*   `/modificar_party` / `/editar_party` - Ajusta los roles o la hora de un Ping activo.
*   `/eliminar_party` - Cancela y borra un llamado activo.
*   `/stats_party` `[Admin]` - Analiza un CSV de loot exportado del juego y muestra estadísticas de quién asistió.
*   `/exportar_party` / `/importar_party` `[Admin]` - Migra composiciones enteras entre servidores mediante archivos JSON/ZIP.

---

## ⚙️ 7. Utilidades, Sorteos y Herramientas

*   `/config_servidor` - **COMANDO MAESTRO:** Abre el Hub de control general del bot.
*   `/info_servidor` - Muestra un resumen de todo lo configurado en este guild.
*   `/utc` - Consulta la hora oficial de servidores (muy útil para ZvZ).
*   `/buscar_ruta` - Herramienta para buscar y reportar conexiones de Caminos Avalonianos.
*   `/crear_reglas` - Imprime un embed bonito con las reglas del servidor.
*   `/crear_canales` / `/eliminar_canales` `[Admin]` - Construye (o destruye) mágicamente canales básicos y categorías recomendadas para gremios de Albion.
*   `/sorteo` / `/editar_sorteo` / `/finalizar_sorteo` `[Admin]` - Sistema completo de Giveaways interactivos.
*   `/crear_contador` / `/estado_contador` `[Admin]` - Crea canales de voz que actúan como "relojes" mostrando stats (Ej: "Miembros: 150").
*   `/crear_tickets` / `/sistema_reportes` `[Admin]` - Construye automáticamente el sistema de canales privados para Tickets de soporte.
*   `/crear_panel` / `/agregar_boton` `[Admin]` - Permite crear Embeds personalizados con botones funcionales.
*   `/rol_masivo` / `/crear_roles` `[Admin]` - Constructores para dar o quitar roles a muchas personas al mismo tiempo.
*   `/cv_temporal` / `/config_canaldevoz` - Soporte y configuración para salas de voz que se borran solas al quedar vacías.
*   `/objetivo` - Publica un temporizador y ping para objetivos de mapa en mundo abierto.
*   `/reload` `[Admin]` - Recarga toda la caché y configuración del bot para aplicar cambios críticos sin reiniciar.
*   `/help` - Muestra el menú de ayuda básico.

---
[⬅️ Volver al Inicio](./index.html)
