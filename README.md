ILLUMINATION website.

#### Relevant files and folders for editing or adding content:

1. home page: index.html
2. project page: project.md
3. team page: team.md
4. relevant images for the website: assets(folder) 

#### Adding new pages:

1. Please refer to random.md as an example
2. To create a new page, simply create a new markdown file (e.g. your_newpage.md) file in the root directory and add the following code block to the top of the file. 
        
        ---
        layout: page
        title: <your_newpage>  
        permalink: /<your_newpage>/  
        main_nav: True  
        ---  
        
3. Setting main_nav to True displays a clickable link to that tab/webpage in the navigation pane on top of the website.

4. Rename title and permalink to the name of the tab/webpage. Then you can continue to use HTML to create content for your webpage.

#### Note
Most other files and folders are generated during website building and should not be altered (hardcoded) . If you wish to change color schemes/background images of the website; this can be changed in `_sass/layout.scss`.