# sorty
Get rid of clutter in your directories. Sorty organizes your files by moving them to different folders based on their filetype and extensions.

## Installation
```bash
$ pip install sorty
```


### Usage
**Basic(Organizes your Desktop, Documents and Downloads directories)**
```bash
$ sorty
```
<br>
**Clean up a single directory**
```bash
$ sorty -d
Enter directory:
```
<br>

**Run sorty in the background(note that you have to run daemon or your system's equivalent with sorty as the specidied command). Here is an example of running sorty iallowing it to update periodically every 15 minutes.**
```bash
$ sorty -b -i 15
```




