<div align="center">
	
# SpotDL-Syncer

A "ecosystem" of Python scripts to create and maintain multiple Spotify Playlists/Albums synchronized.

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
[![Licence](https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge)](./LICENSE)<br>
![](https://img.shields.io/github/stars/Rikiub/spotdl-syncer?style=social)

> Powered by [spotDL](https://github.com/spotDL/spotify-downloader)
	
</div>

## Dependencies

- [Python 3.8](https://www.python.org/downloads/)
	- [spotDL](https://github.com/spotDL/spotify-downloader)
	- [Rich (Included with spotDL)](https://pypi.org/project/rich/)

## Usage

It is important to mention that depending on where you run the script, all operations such as downloading and synchronizing playlists will take place. Additionally, keep in mind that this program works as an "ecosystem," so all Playlist folders must be stored in `main` or alongside the scripts.

**During this guide, please note that:**

-   "Playlist" also refers to "Playlist/Album"
-   `main` folder can be renamed to anything, but the scripts must be kept in the same folder.

### Sync New Playlist

1. Run `s-new-playlist.py`
2. Enter a valid Spotify URL (Playlist/Album) and follow the instructions. A folder with the name of the Playlist will be created in the same directory as the script.
3. To sync only this Playlist, enter its folder and run `s-sync-playlist`.

**WARNING**: Do not delete, rename or move the `data.spotdl` file from the created folder, or you will break the synchronization!

### Sync All Playlists

To sync all downloaded playlists:

1. In `main`, run `s-sync-all`.
2. Wait for the program to synchronize all downloaded playlists in all directories in `main`; it may take a while.

**WARNING**: The synchronization will remove any music files that are not in the Spotify Playlist, so do not store others music files in this folders.
