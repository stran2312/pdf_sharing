# QR Code Web Server

This Python project sets up an HTTP web server that generates a QR code to provide easy access to the server's content. The server displays the content of a specified directory on the user's desktop and generates a QR code containing the server's IP address and port number.

## Requirements
Ensure you have the following packages installed:
- `pyqrcode`
- `pypng`

You can install these via pip:
pip install pyqrcode
pip install pypng


## Usage
1. Run the Python script after installing the required packages.
2. Upon execution, the server will start and display the following information in the console:
    - "serving at port [PORT_NUMBER]"
    - "Type this in your Browser [IP_ADDRESS]"
    - "or Use the QRCode"
3. To access the server's content:
    - **Via IP Address:**
        - Open a web browser on your mobile device.
        - Type the displayed IP address and port number (e.g., `http://192.168.1.10:8010`) in the browser's address bar and press Enter.
    - **Via QR Code:**
        - Use a QR code scanner app on your mobile device.
        - Scan the QR code displayed in the script's output.
4. You should now see the content of the specified directory (typically the user's desktop) in your mobile browser.

## Functionality
- Utilizes `http.server`, `socket`, `socketserver`, and `webbrowser` modules.
- Generates a QR code containing the server's IP address and port.
- Displays the content of the specified directory on the user's desktop.
- Serves content on a designated port for easy access.

## Setup
1. Change the directory path in the code to the desired directory you want to serve.
2. Modify the port number if necessary.
3. Run the script and follow the instructions displayed in the console.

### Note
- Ensure proper permissions to access the directory specified.
- Modify the code as needed to fit your specific use case.
