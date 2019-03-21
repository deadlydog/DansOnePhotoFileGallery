# Dan's One File Photo Gallery

## What Is Dan's One File Photo Gallery

Dan's One File Photo Gallery is a way for you to easily display all of your photos on your website. The only requirements are that you have a website which supports PHP 5. From there just put your photos and my file on your website and that's it. Just go to the file in your web browser and your pictures will be displayed.

For example, I have my own webserver so all I had to do was put my Photo Gallery file in my "My Pictures" folder and point my webserver to the Photo Gallery file, and presto. My entire "My Pictures" collection is available online. If you do this, you may want to make sure there aren't any "incriminating" pictures in there, since the Photo Gallery will display all pictures within that directory and all sub-directories :-)

## Features

- Automatic thumbnail creation
- Easily change the size of generated thumbnails and how many appear on each row
- Supports .jpg, .png, .gif, and .wbmp pictures
- Looks for pictures in all directories and sub-directories of the directory the file is put in
- Can maintain directory structure as an easy to navigate menu, or can simply display all pictures from all directories on one page
- Very configurable via global variables near the top of the file
- Easily change the look and feel of the photo gallery via the CSS style sheet within the file
- Easily specify a welcome message for viewers and explain what your site is about
- It's open source! If you feel like changing something go right ahead
- It's only one file!

## Installation

Installation instructions are also provided within the file itself at the very top.

### Prerequisites

- PHP 5 or greater installed on the webserver
- Pictures to display are of type .jpg, .png, .gif, or .wbmp

### Installation instructions

1. Drop this file into the directory containing your photos, then simply navigate to the file in your web browser. The file display any photos found in the directory, as well as any found in its subdirectories.
1. The GD Graphics Library must be enabled. This is a standard library included with PHP 5, but it is not enabled by default. Simply locate your php.ini file (usually in C:\PHP or C:\Windows) and uncomment the line ";extension=php_gd2.dll" (So it should read "extension=php_gd2.dll"). If you do not host your own website you may have to contact your hosting provider and ask them to do this for you if they have not already done it. If this is not enabled then no pictures will show up. So if everything else shows up except the pictures, this is likely the problem.

## Change log

Created in 2006, and last updated in 2009.

- v1.6
  - Fixed problem with directory paths having spaces in them when $THUMBNAILS_DIRECTORIES_CREATED_IN_PICTURE_DIRECTORIES is set to $No.
- v1.5
  - Added option to store thumbnails in the same directories as the pictures, or to store them in their own directory tree.
  - Removed the $THIS_FILENAME variable and replaced it with a php function to retrieve the name of this file automatically.
- v1.4
  - Added min-width of 800px so pictures aren't moved down below the menu when the window size is shrunk.
- v1.3
  - Fixed apostrophe and ampersand link problems by introducing 2 new functions, EncodeSpecialCharacters and DecodeSpecialCharacters.
- v1.2
  - Fixed apostrophe link problem with Apply button.
- v1.1
  - Fixed apostrophe link problem in the Pages section.
  - Updated Footer link to the proper address.