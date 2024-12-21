# MAC Address Changer

This Python script is a simple tool to change the MAC address of a network interface on a Linux system. It can be useful for testing network setups, enhancing privacy, or bypassing MAC address-based filters.

## Features
- Retrieve the current MAC address of a network interface.
- Change the MAC address to a specified value.
- Verify if the MAC address was successfully changed.

## Requirements
- Python 3
- Root permissions to execute system commands
- A Linux-based operating system

## How to Use
1. Clone this repository or copy the script to your local machine.
2. Ensure you have the necessary permissions to execute the script.  
3. Run the script with the following options:
   ```bash
   python mac_changer.py -i <interface> -m <new_mac_address>
   ```
   Replace `<interface>` with the name of your network interface (e.g., `eth0`, `wlan0`) and `<new_mac_address>` with the desired MAC address (e.g., `00:11:22:33:44:55`).

### Example
```bash
sudo python mac_changer.py -i wlan0 -m 00:11:22:33:44:55
```

## Script Options
- `-i` or `--interface`: Specify the network interface whose MAC address you want to change.
- `-m` or `--mac`: Provide the new MAC address.

## Output
- The script will display the current MAC address of the specified interface.
- It will attempt to change the MAC address and then verify the change.
- Success or failure messages will be shown in the terminal.

### Example Output
```plaintext
Current MAC = 00:1a:2b:3c:4d:5e
[+] Changing MAC address for wlan0 to 00:11:22:33:44:55
[+] MAC address was successfully changed to 00:11:22:33:44:55
```

## Limitations
- This script is designed for Linux systems and may not work on other operating systems.
- Requires administrative privileges (`sudo`) to execute system commands.
- Does not validate the MAC address format. Ensure the provided address is valid.

## Disclaimer
This script is intended for educational and legal purposes only. Misuse of this tool is strictly prohibited. The author is not responsible for any damage or legal issues caused by using this script.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

