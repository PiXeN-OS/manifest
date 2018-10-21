# PiXeN-OS #

### Sync ###

# Initialize local repository
repo init -u https://github.com/PiXeN-OS/manifest -b pie

# Sync
repo sync -c -j16 --force-sync --no-clone-bundle --no-tags



# Set up environment
. build/envsetup.sh

# Choose a target
lunch aosp_cheeseburger-userdebug

# Build the code
mka bacon -j16

