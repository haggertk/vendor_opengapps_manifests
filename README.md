# OpenGapps Mirror Manifest

Usage: `repo init -u https://github.com/haggertk/vendor_opengapps_manifests -b mirror --mirror`

Once the mirror is synced you can then run `repo init -u /path/to/opengapps/mirror/manifests.git -b $BRANCHNAME` and sync normally.

If you want to sync the source quickly but want it to be up-to-date without syncing the mirror every time, then run `repo init -u http://www.github.com/haggertk/vendor_opengapps_manifests -b $BRANCHNAME --reference=/path/to/opengapps/mirror/`. This will init the new repo and fetch all the (available) data from the mirror, but will fallback to GitHub if something is missing in the mirror.
