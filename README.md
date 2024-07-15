# Cambiar distribucion de teclado en linux

### Verificar la configuración
```
setxkbmap -query
```

###  Cambiar la distribución temporalmente

```
setxkbmap -layout latam
```

###  Cambiar la distribución permanentemente

- Editar el archivo de configuración
```
sudo nano /etc/default/keyboard
```

- Modificar la línea XKBLAYOUT
```
XKBLAYOUT="latam"
```

- Guardar y salir
Si usaste nano, guarda los cambios presionando Ctrl + O, luego presiona Enter, y sal con Ctrl + X

- Aplicar cambios
```
sudo service keyboard-setup restart
```
