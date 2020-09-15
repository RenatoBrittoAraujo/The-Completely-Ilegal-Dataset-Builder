# The completely illegal dataset builder 

If you don't strictly care about being on the right side of the law and likes to build datasets, this is the place for you!

### What the f@#! is this?????

A simple to use tool for downloading stuff off the internet given any keyword and filetype you want to. 

### Versions

##### Alpha

v0.1 - Downloads images in a very manual fashion, you can clear a folder off the images of the images you don't want, rename them accordingly and resize them to a standard size.

### Dependencies

Paste this on your terminal (debian based systems. For others, do your magic):

```
sudo apt-get install python3
sudo apt-get install imagemagick
```

### Building up a dataset of images

- Go to google and type what you want the dataset to be about. 
- Go to images, scroll down the page until you think it's enough then save the .html file.
- Run `pyhton3 utils/link_parser.py` and input the file name and the folder you want the .jpg pictures to download to.
- (OPTIONAL: if you want images of the same size) Run `./utils/imageSizeConverter.sh` to resize images to a standard width-height format.
- (OPTIONAL: if you want to clean the dataset) Run `python3 utils/renamer.py` to rename the files in increasing order from [1..n].

