<p align="center">
  <img src="https://github.com/P-404/stuff/raw/master/dump/umai.png" />
</p>

A project that shouldn't have existed by the laws of the internet and yet it does; we present you Project 404, just like the Schrödinger's cat!

 # Project 404
Error 404: Bugs not found!

 ### Instructions
 1. Make sure you have a build environment setup.
 2. Run the following commands to sync Project-404 source

 	```bash
         mkdir p-404 && cd p-404
         repo init -u https://github.com/P-404/android_manifest -b umai
         repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
 	```

 3. Once the source is downloaded prepare your trees.
 	```bash
         # Inherit from Project 404 vendor config
         $(call inherit-product, vendor/404/configs/common.mk)
 	``` 
      - for adopting trees you can visit https://github.com/P404-Devices and check bringup stuffs needed from any other device trees.
      - remove pathmaps from your hals and clone it in respective directories
        - Display  : hardware/qcom/display
        - Media : hardware/qcom/media
        - Audio : vendor/qcom/opensource/audio-hal/primary-hal

4. Building
 	```bash
         source build/envsetup.sh;
         lunch p404_$devicecodename-userdebug;
         make bacon;
 	```
  ### Reporting compilation issues
 - For common porting related errors, visit [**Android Building Help**](https://t.me/AndroidBuildingHelp)

 ### Adding Support
 - For adding your device to the list of supported devices, please raise a issue [**here**](https://github.com/P-404/stuff) with your device tree and previous experience in building roms.

 ### Follow  us for more
 * [**Telegram Group**](https://t.me/project_404)
 * [**Telegram Channel**](https://t.me/project404channel)
 * [**Twitter**](https://twitter.com/Project404x)

 ### Happy Building :)
