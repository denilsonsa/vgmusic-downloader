# VGMusic Downloader

Scrape, download and save all songs from VGMusic, neatly organized in folders.

It has several neat features:

* Organizes the files into folders: `Company/System/Game/Song {Author}.mid`
* Replaces special characters, keeping only filename-safe characters.
* Skips songs already downloaded (based on their file sizes).
* Re-downloads songs if their file sizes don't match.
* Nice progress bars.
* Uses HTTP Keep-Alive to reuse the same TCP connection, reducing the overhead.

## How to use

Tested on Linux, should work on most systems with a recent Python 3 version.

```sh
# Downloading the code
git clone https://github.com/denilsonsa/vgmusic-downloader.git
cd vgmusic-downloader

# Creating and activating a Python virtual environment
python3 -m venv venv
source venv/bin/activate

# Installing the dependencies
pip install -r requirements.txt

# Running Jupyter Lab
jupyter lab VGMusic-downloader.ipynb
```

Then, change the `DESTINATION` under the **Configuration** section, according to your needs.

If you want to customize the filename and folder organization, change it at the **File Handling** section.

Then, **Run → Run All Cells**. And wait one hour or two.
