# 👨‍💻 DeauthX 👨‍💻
## **⚠️️Disclaimer**
This tool is for educational purposes only and should be used for legitimate penetration testing or security research on devices you own or have permission to test. Unauthorized or illegal use can lead to legal consequences. The author is not responsible for any damages or liabilities. Use the tool responsibly and ensure compliance with laws and obtain necessary permissions.

## **📘Introduction**
DeauthX is a command-line utility designed for educational purposes, allowing you to perform various actions related to Wi-Fi networks. This tool is intended for legitimate penetration testing, security research purposes, and network devices that you own or have permission to test.

## **📋Pre-requisites**
- Linux Environment
- [Python 3](https://www.python.org/downloads/)
- [Aircrack-ng](https://www.aircrack-ng.org/downloads.html)

## **🛠️Installation**
1. Clone the repository
```
git clone https://github.com/prashant-sagar-shakya/DeauthX.git
```
2. Move the repository
```
sudo mv DeauthX /opt
```
3. Create a symbolic link
```
sudo ln -s /opt/DeauthX/DeauthX /usr/local/bin/DeauthX
```
4. Make the tool executable
```
sudo chmod +x /opt/DeauthX/DeauthX
```

## **⚙️Options**
| Option                          | Description                                     |
| ------------------------------- | ----------------------------------------------- |
| `-h` or `--help`                | Show help message and exit                      |
| `--mode=<mode> `                | Specify the mode to use                         |
| `--interface=<interface>`       | Specify the Wi-Fi interface                     |
| `--time=<time>`                 | Specify the time you want to scan               |
| `--channel=<channel>`           | Specify the channel number of the Wi-Fi network |
| `--access-point=<access-point>` | Specify the access point MAC to use             |
| `--client=<client>`             | Specify the client MAC to use                   |
| `--number=<number>`             | Specify the number to packets to send           |

## **🔄Modes of Operation**
| Mode            | Description                                           |
| --------------- | ----------------------------------------------------- |
| `scan_wns`      | Scan for Wi-Fi networks                               |
| `list_aps`      | List available Wi-Fi networks                         |
| `scan_ap`       | Scan for clients connected to a Wi-Fi network         |
| `list_clients`  | List clients connected to a Wi-Fi network             |
| `deauth_all`    | Deauthenticate all clients from a Wi-Fi network       |
| `deauth_client` | Deauthenticate a specific client from a Wi-Fi network |

## **🖥️ Usage**
### Scan Wi-Fi networks
```
sudo DeauthX --mode=scan_wns --interface=wlan0 --time=120
```
### List available Wi-Fi networks
```
sudo DeauthX --mode=list_aps
```
### Scan a Wi-Fi network for clients
```
sudo DeauthX --mode=scan_ap --interface=wlan0 --channel=6 --access-point=FF:FF:FF:FF:FF:FF --time=120
```
### List clients connected to a Wi-Fi network
```
sudo DeauthX --mode=list_clients
```
### Deauthenticate all clients from a Wi-Fi network
```
sudo DeauthX --mode=deauth_all --interface=wlan0 --access-point=FF:FF:FF:FF:FF:FF --number=10000
```
### Deauthenticate a specific client from a Wi-Fi network
```
sudo DeauthX --mode=deauth_client --interface=wlan0 --access-point=FF:FF:FF:FF:FF:FF --client=FF:FF:FF:FF:FF:FF --number=10000
```

## **📞Connect With Me**
For questions, suggestions, or just to say hi:
- **GitHub:** [prashant-sagar-shakya](https://github.com/prashant-sagar-shakya)
- **Email:** [prashant.sagar.shakya@gmail.com](mailto:prashant.sagar.shakya@gmail.com)
