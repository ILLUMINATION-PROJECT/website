ILLUMINATION website.

#### Relevant files/folders for editing/adding content:

1. index.html: home page
2. project.md: project page
3. team.md: team page
4. assets(folder) : contains all relevant images for the website 

#### Adding new pages:

please refer to random.md:
1. To create a new page, simple create a new .md file in the root directory and add the code block below to the top of the file. 
        
        ---
        layout: page
        title: "newpage"  
        permalink: /newpage/  
        main_nav: True  
        ---  
        
2. Setting main_nav to True displays a clickable link to that page in the navigation pane on top of the website. Then you can continue to use HTML to create content for your webpage.

#### Final note
All other files and folders are generated during website building and should not be altered unless you wish to change color schemes/background images of the website (this can be changed in `_sass/layout.scss`).