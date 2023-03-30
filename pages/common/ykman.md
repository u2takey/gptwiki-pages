# ykman 
## chatgpt 
The command "ykman" stands for "YubiKey manager" and is a command-line tool used to manage YubiKeys. 

A YubiKey is a hardware security key that can be used for two-factor authentication, password management, and secure login. With YubiKey, users can protect their online accounts from phishing attacks and other cyber threats. 

The "ykman" command allows users to perform various functions related to their YubiKeys. Some of the common functions include:

1. Listing the connected YubiKeys: This command displays all the YubiKeys currently connected to the system.

2. Configuring YubiKeys: Users can configure their YubiKeys for various purposes, such as enabling or disabling certain features, setting a PIN, and programming the YubiKey.

3. Generating OTPs: This command generates one-time passwords (OTP) that can be used for two-factor authentication.

4. Managing applications: YubiKeys can support multiple applications, and users can manage these applications using the "ykman" command.

Overall, the "ykman" command is a powerful tool for managing YubiKeys and keeping your online accounts secure. 

## tldr 
 
> The YubiKey Manager can be used to configure all aspects of the YubiKey.
> More information: <https://docs.yubico.com/software/yubikey/tools/ykman/index.html>.

- Get information from YubiKey:

`ykman info`

- Get information for a given application from YubiKey:

`ykman {{fido|oath|openpgp|otp|piv}} info`

- Get a list of enabled applications over NFC from YubiKey:

`ykman config nfc --list`

- Enable application over USB on YubiKey:

`ykman config usb --enable {{OTP|U2F|FIDO2|OATH|PIV|OPENPGP|HSMAUTH}}`
