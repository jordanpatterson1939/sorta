#! /usr/bin/env python3


import os
import re
import shutil

home = os.path.expanduser('~')
downloads = home+'/Downloads'
documents = home+'/Documents'
desktop = home+'/Desktop'

document_patterns = []
picture_patterns = []
audio_patterns = []
video_patterns = []
coding_patterns = []

class Group:
    def __init__(self,filetypes,target_directory):
        self.filetypes = filetypes
        self.target_directory = target_directory

    def match(self,filename):
        pass
    
    def save(self,filename):
        pass

def getfiles(directory):
    files = []
    li = os.listdir(directory)
    for f in li:
        if os.path.isfile(os.path.join(directory,f)):
            files.append(f)
    return files

def cleanup(groups,directories):
    for d in directories:
        files = getfiles(d)
        for f in files:
            for g in groups:
                if g.match(f):
                    g.save(f)
                    break

def main():
    # document_group = Group(document_patterns,'Documents')
    # picture_group = Group(picture_patterns,'Pictures')
    # audio_group = Group(audio_patterns,'Audio')
    # video_group = Group(video_patterns,'Video')
    # coding_group = Group(coding_patterns,'Code')

    # groups = [document_group, picture_group, audio_group,video_group,coding_group]
    
    directories = [downloads,desktop,documents]
    

    for d in directories:
        print(getfiles(d))

if __name__=='__main__':
    main()
