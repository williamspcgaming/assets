# Downloading Project Files
This repository uses Git LFS in order to manage working with the larger files in the Adobe production pipeline. However, Github does not use anywhere close to enough storage space for this use case for free and I have no interest in paying a monthly fee to make it happen. All files used for LFS are actually stored in a Google Drive but this workaround requires a bit of extra work to clone the repository properly. 

## Prerequisites

Install [Git LFS](https://git-lfs.github.com/), [lfs-folderstore](https://github.com/sinbad/lfs-folderstore), and [Backup and Sync](https://www.google.com/drive/download/). Configure Backup and Sync with the Williams PC Gaming google account and sync the folder titled williamspcgaming to your machine, noting the directory.

Follow the instructions on [lfs-folderstore](https://github.com/sinbad/lfs-folderstore) under "Cloning a repo" to reconfigure your repository.

# Recoloring Assets

# Animations and Layers

# Exporting
Animated assets for direct use in an overlay should be rendered in the `.webm` format using the default `VP8` codec because of its efficient, albeit lossy encoding. This is actually preferable to rendering in `.mp4` using `.H264` encoding as `.H264` does not include an alpha channel which is necessary for transparency. In theory, `.H265` should work but this encoding is still not yet widely supported. You could use other encoding formats that support alpha channels but that is on you