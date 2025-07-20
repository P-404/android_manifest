A project that shouldn't have existed by the laws of the internet and yet it does; we present you Project 404, just like the Schrödinger's cat!

 # Project 404 AOSP Experiments
Error 404: Bugs not found!

 ### Instructions
 1. Make sure you have a build environment setup.
 2. Run the following commands to sync Project-404 source

 	```bash
    repo init -u https://github.com/P-404/android_manifest -b bijin_q2
    repo sync -c --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
 	```

 3. Once the source is downloaded prepare your trees.
 	```bash
    # Inherit from Project 404 vendor config
    $(call inherit-product, vendor/404/config/common_full_phone.mk)
 	```
 4. Building (Details Soon)  
  
 ### Follow  us for more
 * [**Telegram Group**](https://t.me/project_404)
 * [**Telegram Channel**](https://t.me/project404channel)
 * [**Twitter**](https://twitter.com/Project404x)

 ### Happy Building :)