# Add publication/news post
## No-code in-browser approach

1. Navigate to the folder "_publications" or "_news"

![Navigate to folder publications](/assets/images/add_publication_1.jpg)

2. Click on any publication or news file (.md) in that folder and copy it (top-right corner)

![Copy any publication file](assets/images/add_publication_2.jpg)

3. Navigate back to the folder "_publicaitons" or "_news" and add a new file (top-right corner)

![Add a file to publications](assets/images/add_publication_3.jpg)

4. Paste the copied publication into the contents of the newly created file and name it. File name: naming convention is optional (YYYY-MM-DD-paper-name) but it should be a .md file. 

5. Adjust all the fields accordingly.
IMPORTANT: the value in the field date must be in the YYYY-MM-DD format.
The field author should contain all authors of this paper (possible authors listed on people.md).
The last three fields (author_profile, collection and classes) should not be changed.
Change the link to the paper pdf at the bottom of the file in the brackets after "Access paper here" or remove it if there is no pdf availible (yet).

![Adjust fields](assets/images/add_publication_4.jpg)

6. Commit the changes (top-right corner).

### Additional info
1. Escaping special characters
If special characters are present in title, abstract or authors you can do the following.  
When a string scalar is surrounded by single quotes '....' the only escaping within that string that can be done is inserting a double single quote to indicate a single quote:
```
 the user''s behavior
```
When string scalar is surrounded by double quotes, "....", you use backslash for escaping.
```
 \"user behavior\"
```
