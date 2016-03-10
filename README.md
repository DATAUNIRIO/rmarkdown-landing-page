## R Markdown UdS Landing Page

This repository illustrates one way to create a simple landing page made up of multiple R Markdown documents for resources located in the UdS CLARIN-D repository.

Original materials were taken from <https://github.com/rstudio/rmarkdown-website> and adapted to follow CLARIN-
D Corporate Design <http://de.clarin.eu/mwiki/index.php/CLARIN_Corporate_Design>.

Features of the simple website include:

1. Multiple Rmd files are accessible from a global navigation bar (defined in `_navbar.html`)

2. The Rmd files share common output settings (including the directory where dependent libraries are written) defined in `_output.yaml`.

3. The Rmd files share also a common header (`_header.html` devoted to the corpus banner and other logos) and a common footer (`_footer.html` devoted to information about the license).

3. The site can be built using the included `Makefile`. An RStudio Project that binds building the Makefile to `Cmd+Shift+B` is also included.

4. Folder `libs/uds/` contains corpus banner, logos (CLARIN-D, BMBF, CLARIN B Center, UdS), and CSS file overriding theme styles.
