# 📦 Administración de Servicios con `systemctl`

Guía básica en formato claro para administrar servicios y el sistema en Linux usando `systemctl`.

---

## 🔧 Gestión de servicios

Reinicia un servicio, una demo del sistema

```
systemctl restart nombre.service
```

Detiene un servicio, una demo del sistema.

```
systemctl stop nombre.service
```

Inicia un servicio, una demo del sistema.

```
systemctl start nombre.service
```

Recarga la configuración de un servicio sin detenerlo (útil cuando cambias archivos de configuración).

```
systemctl reload nombre.service
```

Recarga todos los servicios y configuraciones del sistema.

```
systemctl daemon-reexec
```

Recarga los archivos de configuración del systemd (cuando haces cambios en servicios).

```
systemctl daemon-reload
```

Habilita un servicio para que inicie automáticamente al arrancar el sistema.

```
systemctl enable nombre.service
```

Deshabilita un servicio para que no inicie al arrancar el sistema.

```
systemctl disable nombre.service
```

Muestra el estado de un servicio.

```
systemctl status nombre.service
```

Lista todos los servicios activos.

```
systemctl list-units --type=service
```

Lista todos los servicios (activos e inactivos).

```
systemctl list-unit-files --type=service
```

---

## 🖥️ Gestión del sistema

Detiene el sistema.

```
systemctl halt
```

Reinicia el sistema.

```
systemctl reboot
```

Apaga el sistema.

```
systemctl poweroff
```

Suspende el sistema.

```
systemctl suspend
```

Hiberna el sistema.

```
systemctl hibernate
```

Suspende e hiberna (modo híbrido).

```
systemctl hybrid-sleep
```

---

## 📊 Información útil

Todos los archivos de registro están en este directorio.

```
/var/log/
```

Ver logs del sistema con journalctl.

```
journalctl
```

Ver logs en tiempo real.

```
journalctl -f
```

Ver logs de un servicio específico.

```
journalctl -u nombre.service
```

---

## ✅ Notas

* Reemplaza `nombre.service` por el nombre real del servicio.
* Algunos comandos requieren permisos de administrador (`sudo`).
* Usa `status` para verificar si los cambios se aplicaron correctamente.

---

✔️ README listo para copiar y usar en tu repositorio.

