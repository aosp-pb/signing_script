## Disclaimer
This script only works for password-less keys (DO NOT SET A PASSWORD) *This is due to building inline, other steps are necessary for a password*

*Works with lineage19.1+*

## How to use

1. Run this script in your root build directory

```bash
bash <(curl -s https://raw.githubusercontent.com/aosp-pb/signing_script/15/gen.sh)
```

2. Enter info for certificate subject line and confirm

3. Hit enter to set no password for each certificate. **Cannot set a password to build inline with this method!**

### Prep device tree (for other ROMs)
In your device tree (or common device tree) add:

`-include vendor/aospb-priv/keys/keys.mk`

Start building..
