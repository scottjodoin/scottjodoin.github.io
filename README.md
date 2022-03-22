# Resume

## Purpose

This guide will walk you through the steps to upload a resume to your Github repository using Markdown, Jekyll theming, and Github pages. This guide will also make references to the suggestions as outlined in Etter's book, **Modern Technical Writing**. 

## Prerequesites

* A resume formatted in Markdown.
* A Github account and dedicated respository

## Instructions

### 1. **According to Etter: Use a lightweight markup language**

The first thing to do is to create a Markdown file `index.md`. This is the file that will be used to create your resume. See below for a link to the **Markdown Cheatsheet** in case this is your first time using Markdown. See **[Why is Markdown better than a word processor?](https://github.com/scottjodoin/scottjodoin.github.io#faq)** for more information on why you should use Markdown.

Here is a template you are free to use to structure your resume in Markdown. Add any extra sections as you need.

```
# YOUR NAME

## Your Role

## TECHNICAL SKILLS

* Technical skills

## RELEVANT WORK EXPERIENCE

### Work Experience Title
Work location, date range

* Description of work

## EDUCATION

### School Name
School location, date range

* Description of achievements

## VOLUNTEER EXPERIENCE

Volunteer location, date range

* Description of work

```

### 2. **According to Etter: Share / host documents on a distributed version control system**

Etter recommends that you use a version control system to manage your documents. This is a good way to ensure that your documents are always up-to-date. We recommend using Github.

Now that you have your resume in Markdown, you need to upload it to a Github repository
#### 1. Create a Github repository for your resume in the following format: `username.github.io`.

#### 2. Grab the link to your repository from the Github page

#### 3. Download the repository in VS Code

Open up a new instance of VS Code and click **Clone a Git Repository**. Copy the link from the Github page and paste it into the **Repository URL** field. Click **Clone** and wait for the repository to download. You should see a new folder in your workspace.

#### 4. Add your resume to the directory as `index.md` and commit your changes.

#### 5. Push your changes to your repository

In VS Code, click the **Git** tab and click **Push**. You should see a message that your changes have been pushed to your repository.

#### 6. Open your Github repository in your browser and see that your file has successfully been uploaded

If you can't see your file, you may need to refresh the page.

### 3. **According to Etter: Format a document with a static site generator**

While styling with html and css can be fun, it also be time consuming and detract from the actual work of writing. Etter recommends using a static site generator to create a website that is easy to read and navigate from the beautiful markdown you produced in an earlier step.

Jekyll is our tool of choice that will convert a Markdown document into a static site. While is is possible to run Jekyll on your own machine, we will let Github pages take care of this for us.

#### 1. Set up Github Pages for your repository
* From your Github repository go to the **Settings** then **Pages** section.
* Choose the   **Main** or **Master** branch and **Save**.
* Choose a Jekyll theme that suits your fancy and commit the changes.

When you go back to your repository, you will find a new file called `_config.yml`. This file contains the configuration for your Jekyll site. So far the file only contains the `theme:` setting.

#### 2. Choose a more specific theme for your resume

If you want to see more Jekyll themes than the default ones that Github provides, you can visit the [Jekyll themes page](https://jekyllrb.com/docs/themes/) to see more. Each theme has a unique name, so when you find one you like, you can replace the `theme:` setting in `_config.yml` with the name of the theme you want and Github will take care of the rest.

#### 3. Configure your Jekyll site
  
The `_config.yml` file contains a lot of settings that can be configured to your liking. Here are a few of the most important ones:

  * `title`: The title of your site that shows up in the tab of your browser.
  * `name`: The text that appears at the top of your site.
  * `theme`: This is the theme that you selected earlier.

Jekyll has a lot of other settings that you can configure as well. The settings that you can configure will depend on the theme you choose, and these settings are usually listed on the Github repository of the theme.

#### 4. Continually update your site

Now that you have set up version control, whenever you want to update your resume you can simply update the `index.md` file and commit your changes.


### More Resources

* [Markdown Tutorial](https://www.markdowntutorial.com/)
* [Markdown Cheatsheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)
* [Andrew Etter's Book, Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
* [COMP 3040 course guide at the University of Manitoba](https://aurora.umanitoba.ca/banprod/bwckctlg.p_disp_course_detail?cat_term_in=202210&subj_code_in=COMP&crse_numb_in=3040) 

## Authors and Acknolwedgements

This resume and README was created by myself, Scott Jodoin in fulfillment of Assignment 2 from COMP 3040. The Jekyll theme {{jekyll theme}} used by this resume was created by {{jekyll author}}. My group members include: Kyle Calinisan, Raven Mico Carencia, Tahmidul Hasnain Zidaan, and Hao Qin. 


## FAQ

### Why is Markdown better than a word processor?

Markdown is simple and clean text content language designed for the web; it is all that it needs to be and nothing more. Did I mention that it is free? Markdown's bare-bones syntax makes it easy for writers to write, collaborate, and use version control. In contrast, word processors filled with print-formatting tools distract from the hard work of writing and restrict authors to use proprietary software, file formats, and collaboration tools. 

### Why is my resume not showing up?
  
Your resume could be not showing for a couple reasons. Did you forget to push your index.md file or _config.yml file? If you just pushed your code, try waiting a little bit: GitHub pages can take up to 20 minutes to deploy. You can view the deployment progress by following the **github-pages** under the Environments section on your respository's main page. 