# clean_maven_repos
A bash script to clean the maven repositories in the home file of the user

After some time using maven for projects, the local repository directory can get really huge.
This tiny bash script traverses through these local repositories and removes all the version folders. You can pass an amount of versions, which should be left out. This number defaults to 3.

## Installation
Just copy the file somewhere on your hard drive and make it executable via chmod +x.

## Usage
Assuming you are either in the folder, where the script is in or otherwise the script is somewhere, where it's globally available you can just run
```
clean_repository [number_of_versions_to_be_excluded]
```
  
This will find all the version subfolders under ~/.m2/repository and removes all of them except for the given amount of last versions.
