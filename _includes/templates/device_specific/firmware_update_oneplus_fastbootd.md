{% include alerts/warning.html content="These instructions are NOT for carrier branded variants." %}

1. Download latest stock ROM from [oneplus.com](https://oneplus.com/support/softwareupgrade) or [Oxygen Updater](https://play.google.com/store/apps/details?id=com.arjanvlek.oxygenupdater).
   Oxygen Updater app usually happens to have newer releases available as OnePlus website tends to lag a bit.
2. Extract stock ROM using [payload-dumper-go](https://github.com/ssut/payload-dumper-go)
3. Boot up exTHmUI recovery
4. Go to "Advanced" -> "Enter fastboot"
   {% include alerts/warning.html content="The \"Enter fastboot\" option may not be present on older exTHmUI recovery builds and it cannot be substituted with \"Reboot to bootloader\"." %}
5. Execute following commands:
   ```
   {{- include.content -}}
   fastboot reboot
   ```
