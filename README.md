This manifest should be applied along with the v316 patches from the 'caosr' branch of treble-patches on gitlab:

    https://gitlab.com/eremitein/treble-patches/-/tree/caosr?ref_type=heads

Note that the last commit is dated 2022-03-21 so we need to sync the manifest packages to this date.

To use this manifest, checkout r48 version of Android 11.0.0 with

    repo init -u https://android.googlesource.com/platform/manifest -b android-11.0.0_r48

then cd into android-11.0.0_r48 and do:

    git clone --single-branch https://github.com/joshuarwood/treble_manifest_caos -b main .repo/local_manifests
