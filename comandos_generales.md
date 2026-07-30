> 🇪🇸 **Español** | 🇺🇸 [English](./en/comandos_generales.html) | 🇧🇷 [Português](./pt/comandos_generales.html)

# 📜 Lista de Comandos

Aunque el 90% de las funciones de Ap BOT v3 se controlan cómodamente a través de menús y botones, existen comandos específicos (`/slash_commands`) diseñados para el uso diario de los jugadores y moderadores.

A continuación tienes la lista completa de comandos disponibles, organizados por categoría. *(Los comandos marcados con 🛡️ requieren permisos de Moderador o Administrador).*

## ⚙️ Configuración y Sistema
*   🛡️ `/config_servidor` - Despliega el **Panel Maestro** desde donde se configuran todos los módulos del bot (Canales, Roles, Multas, etc.).
*   🛡️ `/server_panel` - Imprime el panel público de Registro en el canal actual para que los usuarios vinculen sus cuentas de Albion.
*   `/utc_commands` - Muestra la hora UTC actual y herramientas de conversión de zonas horarias (muy útil para programar CTAs de Albion).

## 💰 Economía y Billeteras
*   `/wallet [usuario]` - Muestra el balance actual (plata), reputación y estado de la billetera de un jugador. Si no mencionas a nadie, muestra la tuya.
*   `/transfer [usuario] [monto]` - Transfiere plata de tu billetera personal a la de otro miembro del gremio.
*   🛡️ `/economy_add [usuario] [monto]` - (Solo Cajeros) Inyecta dinero creado de la nada a la billetera de un jugador (Ej: Premios por asistir a ZvZ).
*   🛡️ `/economy_remove [usuario] [monto]` - (Solo Cajeros) Descuenta dinero de la billetera de un jugador.

## ⚖️ Multas (Fines)
*   🛡️ `/fine_add [usuario] [monto] [razón]` - Emite una multa al jugador. El monto debe ser pagado obligatoriamente a la tesorería del gremio.
*   `/fine_pay [id_multa]` - Permite a un jugador pagar una multa pendiente utilizando el dinero de su propia Wallet.

## 🚫 Seguridad y Blacklist
*   🛡️ `/blacklist_add [nombre_albion] [razón]` - Añade a un jugador a la lista negra global del gremio. Si intenta usar el Panel de Registro, será expulsado automáticamente.
*   🛡️ `/blacklist_remove [nombre_albion]` - Perdona a un jugador y lo borra de la lista negra, permitiéndole registrarse nuevamente.

---
[⬅️ Volver al Inicio](./index.html)
