Find possible duplicate images in EPU using the session metadata.  This issue seems to have been mostly corrected with the latest updates to EPU but I'd be very interested in if other people are seeing this phenomenon.  

Run the script on the top level directory of the EPU session.
For holey carbon it checkes to see if the same hole has been imaged multiple times, for lacy carbon it considers images suspect if they have more than 50% overlap of the illuminated area.

USAGE: ./EPU_duplicate_finder.py <EPU directory> <hole size (um)> <hole spacing (um)>

If hole size and spacing are left blank the grid is assumed to be lacy carbon 


clean_duplicates.py removes suspect images from a relion micrographs star file.  It prioritizes the image with the earliest aqusition date.

USAGE: ./clean_duplicates <micrographs ctf file>  
