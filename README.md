# How to host a resume on GitHub Pages
Welcome! We will learn how to host a resume on GitHub Pages!
- [Purpose](#purpose)
- [Audience](#audience)
- [Prerequisites](#prerequisites)
- [Instructions](#instructions)
  - [Convert your resume to Markdown format](#convert-your-resume-to-markdown-format)
  - [Add your resume to GitHub](#add-your-resume-to-github)
  - [Customize the theme of your resume page](#customize-the-theme-of-your-resume-page)
- [More Resources](#more-resources)
    - [GitHub Pages](#github-pages)
    - [Markdown](#markdown)
    - [Jekyll](#jekyll)
    - [Technical Writing](#technical-writing)
- [Authors and Acknowledgments](#authors-and-acknowledgments)
- [FAQs](#faqs)
     
   

## Purpose
This tutorial will guide you how to create a markdown formatted resume by markdown editor. After that, you will learn how to build a repository on GitHub and how to add your resume to the repository. Further, you will learn how to change the theme of your resume. Through this tutorial, you will gain an in-depth understanding of the methods introduced by Andrew Etter in his book *"Modern Technical Writing: An Introduction to Software Documentation"*. This lightweight, flexible technical writing approach will benefit you a lot.

## Audience

## Prerequisites
1. A Markdown editor.
   + There are several excellent editors to choose from. Please check [The 10 Best Markdown Editors of 2020](https://www.shopify.com/partners/blog/10-of-the-best-markdown-editors).
   + I use [visual studio code](https://code.visualstudio.com/) with [Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced) to write this tutorial.
2. A GitHub account.
   + You can visit [Github](https://github.com/) to sign up an account.
3. An up-to-date resume.


## Instructions
### Convert your resume to Markdown format

1. Open the Markdown editor (e.g. Visual Studio Code ), then create a new file and save it as `resume.md`.
   
2. Put the name and contact information on the top of the resume.
   ```
    # Your name

    + Your address
    + Your phone number
    + Your email

   ```
   Note: # and a space indicate  the biggest header. You can use 1-6 # to indicate  all levels of headers, and 6 # is the smallest header.
   
3. Add second level subheadings, for example:
   
   ```
    ## Education

    ## Soft Skills

    ## Technical Skills

    ## Volunteer Experience

    ## Work experience

    ## Projects

   ```

4. Fill in the details under the second level subheadings, for example:

   ```
    ## Education
    + Bachelor of Science in Computer Science / **University of Manitoba**
     &nbsp; *September 2016-Present* 

    ## Soft Skills
    + Good communication skills

    ## Technical Skills
    ### Languages
     Java, JavaScript, C++, C, Python
    ### Tools
    Eclipse, Visual Studio Code, JUnit, Processing

    ## Work experience
    + Book Editor / **China Industry Press**
    &nbsp; *March 2010-November 2015* 

   ```

  ### Add your resume to GitHub
  1. Sign up and log in your GitHub account.

  2. Create a new repository on Github.
     * Click "strat a project" on your GitHub home page.
     * Enter "*YourUsername*.github.io" in the blank space of Repository name.
     * Choose "Public".
     * Click "Create repository". Then it will jump to a new page.
  3. Click on the "Creating a new file" link in "Quick setup" section.
  4. Name the file as `index.md`. 
   **Note**: *This name is very important! If the name is not `index.md`, your resume will not be displayed on GitHub page.*
  5. Open your existing Markdown formatted resume `resume.md` and copy its contents.
  6. Paste your resume into "Edit new file" area of `index.md` in Github.
  7. Click the "Commit new file" button at the bottom.
   Now, your resume is hosted on Github pages. If you want to see it, go to `https://YourUsername.github.io`. For example, my resume is hosted on `https://mrzhengzhi.github.io`.

   ### Customize the theme of your resume page
At present, our resume page is only the basic version. Fortunately, we can use the some Jekyll template that comes with GitHub pages to change the appearance and style of our resume pages.
  1. Click  "Settings" in your repository.
  2. Scroll to the "GitHub Pages" section and click "Choose a theme" button.
  3. Select one of those themes that you like and click "Select theme" button.
  4. Select "code" and you will find that there is a new file "_config.yml" in your repository. This file can be used to set the theme of your resume page. Now you can go to `https://YourUsername.github.io` to see your new theme.
  
 ![image]（https://github.com/mrzhengzhi/mrzhengzhi.github.io/blob/main/resume.gif）
   
## More Resources
#### GitHub Pages
+ [GitHub Pages](https://pages.github.com/)
+ [Working with GitHub Pages](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages)
#### Markdown
+ [Markdown Quick Tutorial](https://helloacm.com/markdown-markup-language-quick-tutorial/)
+ [Markdown Guide](https://www.markdownguide.org/getting-started)
+ [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet)
#### Jekyll
+ [Jekyll Video Tutorial](https://www.youtube.com/playlist?list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB)
#### Technical Writing
+ [Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)

## Authors and Acknowledgments
This Tutorial was written by [Zhi Zheng](https://github.com/mrzhengzhi).

## FAQs

**1. How do I update my resume ?**
First, go to your resume repository. Second, click `index.md` file. Third, click the pencil icon on the right (i.e."Edit this file"). After that, you can edit your resume. You can view changes through the "Preview changes". After you finish editing, you need to click the green button "commit changes" at the bottom. Now you have finished updating your resume! Very easy, right?

**2. What should I do if I don't want my resume to be seen?**
There are several ways we can do it. First, we can make the `index.md` file blank by editing it. Second, after clicking `index.md`, we can click the trash can icon （"Delete this file"）to delete the file directly. Third, we can click the Settings tab in the repository, then scroll to the bottom "Danger zone", and then click "Change repository visibility" to change visibility to private. Be sure to use the third method carefully! Because it's a potentially destructive act.
