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

