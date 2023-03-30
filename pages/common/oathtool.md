# oathtool 
## chatgpt 
oathtool is a command-line utility for generating and validating Time-based One-Time Password (TOTP) and HMAC-based One-Time Password (HOTP) codes.

TOTP and HOTP are commonly used for two-factor authentication (2FA) systems, where a user must provide a code generated by their mobile device or another device in addition to their regular password.

The oathtool command can be used in the following ways:

1. Generating TOTP and HOTP codes: 
   oathtool <options> <secret>
   This command generates a one-time password code based on the specified secret and options. The secret can be a shared secret key provided by the 2FA system or a Base32-encoded string.

2. Verifying TOTP and HOTP codes:
  oathtool --verify <code> <secret>
  This command verifies a one-time password code against the specified secret. If the code matches, the command returns 0, and if there is a mismatch, it returns 1.

3. Converting a Base32-encoded string:
   oathtool --base32 <string>
   This command decodes a Base32-encoded string and outputs the resulting binary data.

Some common options for oathtool include:

- --totp: specifies that the code generated should be based on TOTP rather than HOTP.
- --digits=<num>: specifies the number of digits in the generated code (defaults to 6).
- --time-step-size=<num>: specifies the number of seconds per time step for TOTP codes (defaults to 30).
- --counter=<num>: specifies the counter value for HOTP codes (defaults to 0).

Overall, oathtool is a powerful utility for generating and verifying one-time password codes for use in 2FA systems. It is commonly used in shell scripts and other automation tools to incorporate 2FA functionality. 

## tldr 
 
> OATH one-time password tool.
> More information: <https://www.nongnu.org/oath-toolkit/oathtool.1.html>.

- Generate TOTP token (behaves like Google Authenticator):

`oathtool --totp --base32 "{{secret}}"`

- Generate a TOTP token for a specific time:

`oathtool --totp --now "{{2004-02-29 16:21:42}}" --base32 "{{secret}}"`

- Validate a TOTP token:

`oathtool --totp --base32 "{{secret}}" "{{token}}"`