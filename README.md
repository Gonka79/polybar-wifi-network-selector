# Polybar Wi-Fi Network Selector

This repository contains a customizable script and Rofi theme for displaying and managing Wi-Fi networks directly from Polybar. With this setup, you can easily view your current Wi-Fi connection and switch between available networks with just a few clicks.

## Features

- **Display Current Network**: The Polybar module shows the name of the currently connected Wi-Fi network, or indicates if no network is connected.
- **Network Selection with Rofi**: Clicking on the Polybar module launches a Rofi menu that lists all available Wi-Fi networks. Users can select a network to connect to, and if the network is password-protected, the script prompts for the password.
- **Seamless Integration**: Designed for easy integration with any Polybar setup, supporting various Linux distributions by leveraging environment variables.
- **Portable Configuration**: The script and configuration are fully portable, making it easy to adapt for different users and environments.

## Installation

1. **Clone this repository** and navigate to the directory:

   ```bash
   git clone https://github.com/yourusername/polybar-wifi-network-selector.git
   cd polybar-wifi-network-selector
   ```

   ## 2. Place the script in your Polybar scripts directory:
   ```
   cp wifi-menu.sh ~/.config/polybar/scripts/
   ```

   ## 3. Ensure the script is executable:
   ```
   chmod +x ~/.config/polybar/scripts/wifi-menu.sh
   ```

   ## 4. Place the Rofi theme in the appropriate directory:

    ```
    mkdir -p ~/.config/polybar/scripts/rofi
    cp wifi-menu.rasi ~/.config/polybar/scripts/rofi/
    ```
   ## 5. Edit your Polybar config (~/.config/polybar/config) to include the Wi-Fi module:
   ```
   [module/wifi]
   type = custom/script
   exec = ~/.config/polybar/scripts/wifi-menu.sh
   click-left = ~/.config/polybar/scripts/wifi-menu.sh --select
   interval = 10
   format-padding = 2
   ```

   ## 6. Restart Polybar to apply the changes:

   ```
   polybar-msg cmd restart

   ```
   
# Dependencies

    NetworkManager: The script relies on nmcli, which is part of NetworkManager.
    Rofi: Rofi is used to display the list of available Wi-Fi networks in a user-friendly menu.

Install these dependencies with:
```
sudo apt install network-manager rofi
```

# Customization

**Rofi Theme:** The theme is located at ~/.config/polybar/scripts/rofi/wifi-menu.rasi and can be customized to match your desktop environment.
    
 **Polybar Module Configuration:** Adjust the appearance and behavior of the Polybar module by editing parameters such as format-padding and content.

# Usage

**Display Current Network:** The Polybar module shows the SSID of the connected network.
    
**Select a Network:** Click on the module to open the Rofi menu and select a different Wi-Fi network. If the selected network is password-protected, you will be prompted to enter the password.

# Contribution

Feel free to fork the repository, submit pull requests, or open issues for any bugs or feature requests. Contributions are welcome!

# License

This project is licensed under the MIT License - see the LICENSE file for details.



# Documentación en Español 
# Selector de red Wi-Fi de Polybar

Este repositorio contiene un script personalizable y un tema Rofi para visualizar y administrar redes Wi-Fi directamente desde Polybar. Con esta configuración, puede ver fácilmente su conexión Wi-Fi actual y cambiar entre las redes disponibles con solo unos pocos clics.

## Características

- **Mostrar red actual**: el módulo Polybar muestra el nombre de la red Wi-Fi conectada actualmente o indica si no hay ninguna red conectada.
- **Selección de red con Rofi**: al hacer clic en el módulo Polybar, se inicia un menú Rofi que enumera todas las redes Wi-Fi disponibles. Los usuarios pueden seleccionar una red a la que conectarse y, si la red está protegida con contraseña, el script solicita la contraseña.
- **Integración perfecta**: diseñado para una fácil integración con cualquier configuración de Polybar, compatible con varias distribuciones de Linux aprovechando las variables del entorno.
- **Configuración portátil**: el script y la configuración son completamente portátiles, lo que facilita su adaptación para diferentes usuarios y entornos.

## Instalación

1. **Clonar este repositorio** y navegar al directorio:

```bash
git clone https://github.com/yourusername/polybar-wifi-network-selector.git
cd polybar-wifi-network-selector
```

## 2. Colocar el script en el directorio de scripts de Polybar:
```
cp wifi-menu.sh ~/.config/polybar/scripts/
```

## 3. Asegurarse de que el script sea ejecutable:
```
chmod +x ~/.config/polybar/scripts/wifi-menu.sh
```

## 4. Colocar el tema Rofi en el directorio apropiado:

```
mkdir -p ~/.config/polybar/scripts/rofi
cp wifi-menu.rasi ~/.config/polybar/scripts/rofi/
```
## 5. Edite la configuración de Polybar (~/.config/polybar/config) para incluir el módulo Wi-Fi:
```
[module/wifi]
type = custom/script
exec = ~/.config/polybar/scripts/wifi-menu.sh
click-left = ~/.config/polybar/scripts/wifi-menu.sh --select
interval = 10
format-padding = 2
```

## 6. Reinicie Polybar para aplicar los cambios:

```
polybar-msg cmd restart

```

# Dependencias

NetworkManager: el script se basa en nmcli, que es parte de NetworkManager.
Rofi: Rofi se utiliza para mostrar la lista de redes Wi-Fi disponibles en un menú fácil de usar.

Instale estas dependencias con:
```
sudo apt install network-manager rofi
```

# Personalización

**Tema Rofi:** El tema se encuentra en ~/.config/polybar/scripts/rofi/wifi-menu.rasi y se puede personalizar para que coincida con su entorno de escritorio.

**Configuración del módulo Polybar:** Ajuste la apariencia y el comportamiento del módulo Polybar editando parámetros como format-padding y content.

# Uso

**Mostrar red actual:** El módulo Polybar muestra el SSID de la red conectada.

**Seleccionar una red:** Haga clic en el módulo para abrir el menú Rofi y seleccionar una red Wi-Fi diferente. Si la red seleccionada está protegida con contraseña, se le solicitará que ingrese la contraseña.

# Contribución

Siéntase libre de crear un fork del repositorio, enviar solicitudes de incorporación de cambios o abrir problemas para cualquier error o solicitud de funciones. ¡Las contribuciones son bienvenidas!

# Licencia

Este proyecto está licenciado bajo la licencia MIT. Consulte el archivo de LICENCIA para obtener más detalles.




   

