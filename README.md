# Systemless User Certificates

Simple Magisk module to add self-signed user certificates to the system trust store without modifying the system partition.

After installation place your self-signed certificates in `/data/adb/modules/systemless-user-certificates/system/etc/security/cacerts` and reboot your device.

**ATTENTION!** The certificates must be compatible with Android. If you are unsure how to make a certificate Android compatible, import the certificate using the Settings app and then copy the converted certificate from `/data/misc/user/0/cacerts-added` into the Magisk module directory mentioned above. You can uninstall the imported certificate afterwards if you want, or keep both versions (system and user) installed at the same time.

## DISCLAIMER

**No support provided for this module whatsoever.** I'm using this mainly for development and testing (encrypted "localhost"). Don't import random certificates into your system trust store when you don't know what they are used for.
