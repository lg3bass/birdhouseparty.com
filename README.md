# birdhouseparty.com

This is my personal work blog where I keep track of projects.  

### Steps to to publish
1. open the /BW_PUBLISH/birdhouseparty.com in terminal
2. update the post .md file
3. check the post using:
		
		//"-D" mean w/drafts
		hugo server -D

4. publish commands:

		git status -s
		git add -A
		git commit -m "<use-folder-name-plus-date/time>"
		//eg. -m "20181115_snowyBoots-0125"
		
		git push

### Create a new post

		hugo new --kind post-bundle post/20181115_snowyBoots

- NOTE: camelCase DOESN'T work. 
- This will create a folder called "20181115\_snowyBoots" and a post called "work\_new.md"  This also creates a folder called "work\_new" which contains a template.jpg file. You can change the name of the folder, post, images folder.  Note the images folder needs to be the same name as the post. Place your cover image in the images folder and update the \<post\>.md file with 

### Clone birdhouseparty.com repo on new computer

1. Run this command to clone this repo with the theme.

		//pull down a fresh copy of the latest site with the submbodules(theme)		git clone --recurse-submodule https://github.com/lg3bass/birdhouseparty.com.git
		
2. To pull with the submodules use.

		git pull --recurse-submodules
		
### Notes/Issues
- Sometimes when you pull it donesn't pull all the content.  So you will need to download fresh on a computer.
		
	

