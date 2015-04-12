slimlp_manifest
================

Local Manifest to build CyanogenMod 12.1 for the Huawei Y300/G510/G330/C8812E

Build Instructions
-----------------------------------------------------------------------------

1. Initialize repo using the SlimLP manifest (CAF branch)
    
        repo init -u git://github.com/CyanogenMod/android.git -b cm-12.1

2. Add my local manifest

        mkdir .repo/local_manifests
        Copy cm_huawei.xml to .repo/local_manifests

3. Then sync up the repositories
 
        repo sync

4. Initialize the build environment

        source build/envsetup.sh
    
5. Build the ROM

        For Y300:
            brunch u8833
        For G510:
            brunch u8951
        For G330:
            brunch u8825
	For C8812E:
	    brunch c8812e

Credits
-----------------------------------------------------------------------------
fonz93 chil360 dazzozo
