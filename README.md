ILLUMINATION website.

#### Relevant files and folders for editing or adding content:

1. index.html: home page
2. project.md: project page
3. team.md: team page
4. assets(folder) : contains all relevant images for the website 

#### Adding new pages:

1. Please refer to random.md as an example
2. To create a new page, simple create a new .md (e.g. your_newpage.md) file in the root directory and add the following code block to the top of the file. 
        
        ---
        layout: page
        title: <your_newpage>  
        permalink: /<your_newpage>/  
        main_nav: True  
        ---  
        
3. Setting main_nav to True displays a clickable link to that page in the navigation pane on top of the website.

4. Rename title and permalink to the name of the tab/webpage. Then you can continue to use HTML to create content for your webpage.

#### Note
Most other files and folders are generated during website building and should not be altered (hardcoded) . If you wish to change color schemes/background images of the website (this can be changed in `_sass/layout.scss`).