# ziemannlab
Ziemann lab website

# Instructions

To make a new post, edit the files under content/post

The content folder also has static sites like about and team.

These files can be index.Rmd or index.md.

In the projects base directory, run the following R command:

```
blogdown::build_site(build_rmd = TRUE,local=TRUE,run_hugo=TRUE)
```

then copy the contents to the html directory.

```
sudo cp -r public/* /var/www/html
```

Do it carefully as you don't want to share any files outside the
public folder.

Once it looks okay, be sure to add the source files (Rmd, md, jpg) to the github.
