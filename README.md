# WARNING
Use only at your discretion.

While this has nothing to do with cheating, you may be banned from online games if anti-cheat systems doesn't like it.
The repository's name contains the word 'hack' only because the author didn't think of its association to cheating.

## What?
Originally started as hacky solution for shader compilation stutter in dxvk. Similar solution was later added to dxvk itself and promptly
removed. This patch restores it again.

Not enabled by default

### Games tested

* Path of Exile: seems fine. Disabling state cache (`DXVK_STATE_CACHE=0`) is recommended, though.

### Instructions

* Set environment variable `DXVK_ASYNC=1`

### Installation instruction

* Clone the repository
* Enter folder and copy pipeline.patch
* Put `pipeline.patch` in the dxvk folder where `package-release.sh` is located
* Run `patch -Np1 -i ./pipeline.patch` ready patch applied
* After patch applied build dxvk normally
