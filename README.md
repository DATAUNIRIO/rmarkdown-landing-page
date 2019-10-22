## R Markdown UdS Landing Page

This repository illustrates one way to create a simple landing page made up of multiple R Markdown documents for resources located in the UdS CLARIN-D repository.

Original materials were taken from <https://github.com/rstudio/rmarkdown-website> and adapted to follow CLARIN-
D Corporate Design <http://de.clarin.eu/mwiki/index.php/CLARIN_Corporate_Design>.

Learn how to adapt this example to your needs with the RMarkdown documentation <http://rmarkdown.rstudio.com/html_document_format.html>.

Features of the simple website include:

1. Multiple Rmd files are accessible from a global navigation bar (defined in `_navbar.html`)

2. The Rmd files share common output settings (including the directory where dependent libraries are written) defined in `_output.yaml`.

3. The Rmd files share also a common header (`_header.html` devoted to the corpus banner and other logos) and a common footer (`_footer.html` devoted to information about the license).

3. The site can be built using the included `Makefile`. An RStudio Project that binds building the Makefile to `Cmd+Shift+B` is also included.

4. Folder `libs/uds/` contains corpus banner, logos (CLARIN-D, BMBF, CLARIN B Center, UdS), and CSS file overriding theme styles `styles.css`.


----------------------------------------------------------------------------------------------------------------------------------------------------------------

Get started in 5 steps

Open RStudio and create a new project.
Run the following commands in RStudio to bootstrap your new project website with Project Kickstart-R:

```{r}
install.packages("blogdown")
install.packages("hugo")
blogdown::new_site(theme = "gcushen/hugo-academic", sample = FALSE, theme_example = FALSE)
download.file( url = "https://github.com/sourcethemes/project-kickstart-r/archive/master.zip", destfile="project-kickstart-r.zip")
unzip( zipfile = "project-kickstart-r.zip", junkpaths = TRUE )
```

Customise your new site and deploy it.
Fonte:https://georgecushen.com/talk/2018/build-website-with-rmarkdown/
      https://sourcethemes.com/academic/docs/install/#install-with-rstudio