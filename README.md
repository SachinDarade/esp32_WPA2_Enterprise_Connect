# WPA2 Enterprise Example

This example shows how ESP32 connects to AP with wpa2 enterprise encryption to University of Auckloand (UoA) Wifi which uses the CA certificate for verification. Follow the following steps:

1. Replace the file wpa2_ca.pem with your own Certificate from QuVadis_Root_CA_2_G3.crt or any other certificate of similar format which you have.
2. Use your UPI/Username in both the fields of EAP_ID, EAP_USERNAME. Enter your password. This can also be done through the Configuration Menu. 
3. Use method as PEAP in the configuration menu.
4. Connect to AP using the steps from: https://docs.espressif.com/projects/esp-idf/en/latest/get-started/index.html#step-4-set-up-the-environment-variables



### Example output

Here is an example of wpa2 enterprise(PEAP method) console output.

I (1352) example: Setting WiFi configuration SSID wpa2_test...
I (1362) wpa: WPA2 ENTERPRISE VERSION: [v2.0] enable

I (1362) wifi: rx_ba=1 tx_ba=1

I (1372) wifi: mode : sta (24:0a:c4:03:b8:dc)
I (3002) wifi: n:11 0, o:1 0, ap:255 255, sta:11 0, prof:11
I (3642) wifi: state: init -> auth (b0)
I (3642) wifi: state: auth -> assoc (0)
I (3652) wifi: state: assoc -> run (10)
I (3652) wpa: wpa2_task prio:24, stack:6144

I (3972) wpa: >>>>>wpa2 FINISH

I (3982) wpa: wpa2 task delete

I (3992) wifi: connected with wpa2_test, channel 11
I (5372) example: ~~~~~~~~~~~
I (5372) example: IP:0.0.0.0
I (5372) example: MASK:0.0.0.0
I (5372) example: GW:0.0.0.0
I (5372) example: ~~~~~~~~~~~
I (6832) event: ip: 192.168.1.112, mask: 255.255.255.0, gw: 192.168.1.1
I (7372) example: ~~~~~~~~~~~
I (7372) example: IP:192.168.1.112
I (7372) example: MASK:255.255.255.0
I (7372) example: GW:192.168.1.1
I (7372) example: ~~~~~~~~~~~
I (9372) example: ~~~~~~~~~~~
I (9372) example: IP:192.168.1.112
I (9372) example: MASK:255.255.255.0
I (9372) example: GW:192.168.1.1
I (9372) example: ~~~~~~~~~~~
