# watchfile
very simple tool to turn any terminal into a IDE.
```
watchfile [file to look at] [command]
```
The file to look at could be anything. The same is for the command (for piped command use quotation marks).

for example:

```
watchfile script_im_writing.py python script_im_writing.py
#will run the script everytime it is saved
```
There are more complicated stuff that can be used with.
```
watchfile script_im_writing.py python script_im_writing.py input_file.txt
#will run as before but giving command line agruments
```
```
watchfile script_im_writing.py "python script_im_writing.py input_file.txt | head"
#will run as before but giving command line agruments and only show the top 10 lines of output
```
```
watchfile input_file.txt "python script_im_writing.py input_file.txt | head"
#will run when the input_file.txt gets updated
```


##install
Make sure the script folder is in your path.
