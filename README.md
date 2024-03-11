# auto-bspwm

> Este es un script Bash que automatiza la configuración de un entorno de hacking profesional para Kali Linux usando el gestor de ventanas en mosaico [bspwm](https://github.com/baskerville/bspwm).

## Installation
1. Instale las actualizaciones disponibles.

```shell
sudo apt update
sudo apt upgrade -y
```

2. Clonar el repositorio y navegar por él.

```shell
git clone https://github.com/r1vs3c/auto-bspwm.git
cd auto-bspwm
```

3. Concede permisos de ejecución al script.
```shell
chmod +x setup.sh && chmod 777 setup.sh
```

4. Ejecuta el script.

```shell
bash setup.sh
```

5. Una vez finalizado el script, se le pedirá que reinicie el sistema. Una vez reiniciado, seleccione `bspwm` como gestor de ventanas e inicie sesión con su usuario y contraseña habituales.

## ⚠️ IMPORTANTE ⚠️

__El script se debe ejecutar sin permisos de superusuario (root), de lo contrario no funcionará__

__Este software está pensado para ejecutarse en Kali Linux__

## Vista previa del entorno:
![overview1](/assets/overview1.png "overview1")

![overview2](/assets/overview2.png "overview2")

![overview3](/assets/overview3.png "overview3")


## Atajos del teclado:
- <kbd>Windows</kbd> + <kbd>Enter</kbd>: Abre una ventana del emulador de terminal (kitty).
- <kbd>Windows</kbd> + <kbd>W</kbd>: Cierra la ventana actual.
- <kbd>Windows</kbd> + <kbd>Alt</kbd> + <kbd>R</kbd>: Reinicia la configuración de bspwm.
- <kbd>Windows</kbd> + <kbd>Alt</kbd> + <kbd>Q</kbd>: Cierra sesión.
- <kbd>Windows</kbd> + <kbd>(⬆⬅⬇➡)</kbd>: Navegar por las ventanas del espacio de trabajo actual.
- <kbd>Windows</kbd> + <kbd>D</kbd>: Abrir Rofi. Presiona <kbd>Esc</kbd> para salir.
- <kbd>Windows</kbd> + <kbd>(1,2,3,4,5,6,7,8,9,0)</kbd>: Cambie al espacio de trabajo correspondiente.
- <kbd>Windows</kbd> + <kbd>T</kbd>: Cambia la ventana actual al modo mosaico.
- <kbd>Windows</kbd> + <kbd>M</kbd>: Cambia la ventana actual al modo "completo" (no ocupa la polibarra). Pulsa las mismas teclas para volver al modo mosaico.
- <kbd>Windows</kbd> + <kbd>F</kbd>: Cambia la ventana actual al modo de pantalla completa (ocupa toda la pantalla, incluida la polibarra).
- <kbd>Windows</kbd> + <kbd>S</kbd>: Cambia la ventana actual a modo flotante.
- <kbd>Windows</kbd> + <kbd>Shift</kbd> + <kbd>(1,2,3,4,5,6,7,8,9,0)</kbd>: Mover la ventana actual a otro espacio de trabajo.
- <kbd>Windows</kbd> + <kbd>Alt</kbd> + <kbd>(⬆⬅⬇➡)</kbd>: Redimensiona la ventana actual (sólo funciona si está en modo flotante).
- <kbd>Windows</kbd> + <kbd>Ctrl</kbd> + <kbd>(⬆⬅⬆➡)</kbd>: Cambia la posición de la ventana actual (sólo funciona si está en modo flotante).
- <kbd>Windows</kbd> + <kbd>Shift</kbd> + <kbd>F</kbd>: Abrir Firefox.
- <kbd>Windows</kbd> + <kbd>Shift</kbd> + <kbd>B</kbd>: Abrir Burpsuite.
- <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>L</kbd>: Bloquear la pantalla.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>⬆⬇</kbd>: Subir/bajar el volumen.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>M</kbd>: Silenciar/activar el volumen.
- <kbd>Windows</kbd> + <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>(⬆⬅⬇➡)</kbd>: Muestre una preselección y, a continuación, abra una ventana (kitty, Firefox, Gestor de archivos, etc.). 
   - <kbd>Windows</kbd> + <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>Space</kbd>: Deshacer la preselección.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Enter</kbd>: Abrir una subventana en una ventana normal.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Z</kbd>: Hacer zoom en la subventana actual.
- <kbd>Ctrl</kbd> + <kbd>(⬆⬅⬇➡)</kbd>: Navega entre las subventanas de la ventana actual.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>R</kbd>: Redimensiona la subventana actual. Después, utilice:
   - <kbd>W</kbd> for 'Más ancho'
   - <kbd>N</kbd> for 'Más fino'
   - <kbd>T</kbd> for 'Más alto'
   - <kbd>S</kbd> for 'Más corto'
   - <kbd>R</kbd> for 'Resetear'
   - <kbd>Esc</kbd> salir del modo configuración de tamaño.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>L</kbd>: Alternar la disposición de las subventanas.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>W</kbd>: Cerrar la pestaña o sunventana actual.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>T</kbd>: Abrir una pestaña en la ventana actual.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Alt</kbd> + <kbd>T</kbd>: Renombrar el título de la ventna actual.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>(⬅➡)</kbd>: Navegar entre las pestañas actuales.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>C</kbd>: Copiar al portapapeles.
- <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>V</kbd>: Copiar desde el portapapeles.
- <kbd>F1</kbd>: Copiar al búfer A.
- <kbd>F2</kbd>: Pegar al búfer A.
- <kbd>F3</kbd>: Copiar al búfer B.
- <kbd>F4</kbd>: Pegar al búfer B.

## Software
Esta configuración utiliza el siguiente software:
- **WM**: [bspwm](https://github.com/baskerville/bspwm)
- **Hotkey**: [sxhkd](https://github.com/baskerville/sxhkd)
- **Locker**: [i3lock-fancy](https://github.com/meskarune/i3lock-fancy)
- **Shell**: [zsh](https://www.zsh.org/)
- **Shell Theme**: [powerlevel10k](https://github.com/romkatv/powerlevel10k)
- **Shell configuration manager**: [ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)
- **Bars**: [polybar](https://github.com/polybar/polybar)
- **Bars Theme**: [polybar-themes](https://github.com/adi1090x/polybar-themes)
- **Compositor**: [picom](https://github.com/yshui/picom)
- **File Manager**: [thunar](https://docs.xfce.org/xfce/thunar/start)
- **Fonts**: [iosevka](https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/Iosevka) and [hack](https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/Hack)
- **Application Launcher**: [rofi](https://github.com/davatorium/rofi)
- **Browsers**: [firefox](https://www.mozilla.org/en-US/firefox/new/)
- **Terminals**: [kitty](https://sw.kovidgoyal.net/kitty/) and [qterminal](https://github.com/lxqt/qterminal)
- **Static Wallpaper**: [feh](https://github.com/derf/feh)
- **Color Scheme**: [pywal](https://github.com/dylanaraps/pywal)
- **Screenshot**: [flameshot](https://flameshot.org/)

## Credits
- Este entorno se ha inspirado en las funcionalidades del entorno [S4vitar's](https://github.com/s4vitar).
- Gracias a [Cube](https://github.com/ZLCube) por su contribución a la creación del fondo de pantalla `archkali.png`.
