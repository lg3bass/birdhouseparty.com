# birdhouseparty.com


### Steps to to publish
1. open the /BW_PUBLISH/birdhouseparty.com in terminal
2. update the post .md file
3. check the post using hugo server D
4. commands:
	1. git status -s
	2. git add -A
	3. git commit -m "add message"
	4. git push

### Create a new post
1. hugo new --kind post-bundle post/20181115_snowyBoots
	* NOTE: camelCase DOESN'T work. 
	* This will create a folder called 20181115_snowyBoots and a post called work_new.md  This also creates a folder called work_new which contains a template.jpg file. 
2. You can change the name of the folder, post, images folder.  Note the images folder needs to be the same name as the post.
3. place your cover image in the images folder and update the <post>.md file with 

