Seems like the unix filesystem could provide a nice way to 
organize files with symbolic links perhaps even including metadata.

Structure
=========

Keep all the files in a directory called STORAGE.
Create topic directories such as:

 - Articles
 - Books
 - MyContent
 - PythonCode
 - HTML5
 - FORTRAN
 - Ccode
 - Demos
 - Combustion
 - Networks
 - NeuronStuff
 
Then add files to the topics using symbolic links::

  STORAGE/ $ ln -s ~/STORAGE/Flaming Combustion
  STORAGE/ $ ln -s ~/STORAGE/Flaming MyContent
  STORAGE/ $ ln -s ~/STORAGE/Flaming FORTRAN
  
Now the Flaming files are available in 3 easier to find places.

Questions
=========

**Q:** How does this comapre in performance and ease to keeping all
files in a single directory and using find, locate and grep to find them?
  
MetaData
========

Could a specific file be kept in each directory of STORAGE with metadata 
on the files in that directory? I think of the metadata as being created
by the user. But I supose it could be automated too. Comments on pdf paper,
citations related to the material, webpages retrived from, webpages with 
related work or images/video. Sort of a oneNote approach to collecting
comments on the material in that directory.
