## Summary

This repository is intended to download the mp3 songs from a given playlist to later transfer the music to an iPod nano. Other devices can be also used, but these need to be tested as only this has been tested with the afore mentioned iPod.
Please follow the instructions to replicate the transferral of music to the device.

## Instructions

The playlist can be downloaded in csv file format from the following web-site:

'https://www.tunemymusic.com/de/home'

To be able to do so, one would need to create an account on this web-site and have an spotify account to be linked. 
After logging in select the playlist from spotify that one would like to transfer to the iPod in csv format.

# Create Music folder

'mkdir ~/Music'

# Create folder to store csv file.

'mkdir ~/include'

# Clone the spotiplay

'cd ~'

'git clone https://www.tunemymusic.com/de/home'

# Give execution permissions

'chmod +x ~/spotiplay'

# Access the music directory

'cd ~/Music'

# Execute the command

'~/spotiplay <spotify-playlist-link>

Then the music will be downloaded into the Music directory.

## Transfer the music to the iPod

# Update apt database 

'sudo apt update'

# Install gtkpod

'sudo apt -y install gtkpod'

## Connect iPod to Computer

# Create mounting point for iPod

'sudo mkdir -p /media/ipod'

# Mount iPod

'sudo mount /dev/sdb2 /media/ipod'

# Open gtkpod

- type <super> key on keyboard.
- type gtkpod
- type <Enter> key on keyboard.
- select the correct version of your iPod on the prompt window.

## Add downloaded music to gtkpod

- Click on the 'Music' tab
- Click on 'Add Folder'
- Select the '~/Music' directory

## Transfer the music to your iPod

- Select your playlist directory on the left panel.
- Select a song from the list found in center of the window.
- type 'ctr-A'.
- Click on the 'Music' tab
- Click on Normalize

## Notes

If there are bugs please write them in the comments so these can be attended.
