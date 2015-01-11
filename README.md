## About

A little photo management helper in Ruby.

For now, it just takes a directory with your images and sorts out contained photos according to the date when they got shot. If a file doesn't contain EXIF or contains wrong EXIF information, it's being ignored, new log entry created (pixd.log in the source directory).

### Usage

I wrote this little helper to use it my photo workflow. This consits today of:

a) automatic sync of pictures from my Smartphones and Tablets (by using BitTorrent Sync on my iOS and Android devices) into a local folder (on my network HDD connected to Raspberry PI)

b) Sorting out picutres from a) into a time line folder structure (/year/month/day). While sorting out the program also renames the files so they are sortable by time taken


  pixd SOURCE DESTINATION

#### Example

pixd . /mnt/myhdd/martin/pictures/library
=> Fotos from current directory will be sorted out to your external hardrive.

## TODO

* provide option to remove files from SOURCE (when successfuly copied)
* provide option to put problematic files to "Karantene" folder
* include movies, not only photographs