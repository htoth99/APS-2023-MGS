# APS-2023-MGS
Welcome! If you've made it to this site, it means you're enrolled in the pre-meeting metagenomics workshop held at APS 2023. This page will serve as your one-stop shop for this workshop. Here, you will find links to download programs, lines of code that you will copy, and much more. 

You should have recieved an email from the Ohio Supercomputer (OSC) about signing up for an account. Please follow those instructions and gain access to an account as soon as you can, since that link expires. Almost all of the workshop will take place on the OSC, so it is crucial for you to sign up for an account. 

Lastly, it is incredibly important for you to bring your computer to the workshop, as this workshop relies on indivudal computers. 

## Things to download on your computer
Most of this workshop will take place on the OSC, but there are a few times you will need to use a program downloaded to your computer. 

### R and Rstudio
We will use Rstudio for part of the course. You can download them at: https://cran.rstudio.com and https://posit.co

This guide is a comprehensive walk-through of downloading both: https://teacherscollege.screenstepslive.com/a/1108074-install-r-and-r-studio-for-windows

### Mauve
Mauve is a genome alignment viewer, and can be a super cool tool to compare similar genomes! You may have the opportunity to work with it during this course. You can download it here: https://darlinglab.org/mauve/mauve.html

## During the course


You will need the following lines of code for Pavian. 

This line installs Pavian into your Rstudio
```bash
if (!require(remotes)) { install.packages("remotes") }
remotes::install_github("fbreitwieser/pavian")
```
This line will open the Pavian interface
```bash
pavian::runApp(port=5000)
```

