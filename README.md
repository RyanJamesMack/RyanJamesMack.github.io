# 1. README
## 2. Purpose
This README provides a reference of how to host markdown files as a static site. This is accomplished by referencing concepts from Andrew Etters book *Modern Technical Writing.*
## 3. Prerequisites
- Basic knowledge of the Markdown language
- A resume in the form of a Markdown file (.md) that can be hosted. 
## 4. Instructions
1. Log in to your Github account. If you have not created one, you can follow this guide to create one: https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github. Github is one option for a version control software that Etter recommends in his book *Modern Technical Writing.* 
2. Create a public repository with a name of the form *account_name*.github.io. This format is necessary to be able to host your resume on Github pages because Github will not recognise it otherwise. Once complete you should be able to see the new repository in the list of your current repositories.
3. Upload your Markdown resume to your Github repository. This can be done by clicking the add file button once you are inside your repository. The file should be in the markdown language so that it is easy modify if changes ever need to be made.
4. Change the name of your resume to **index.md**. This is also necessary for Github to host your site as Github will not recognize it otherwise.
5. Create a new file name _config.yml. This file will be responsible for converting your Markdown resume into a website that Github can use. From this _config.yml file you are able to configure all the necessary Jekyll settings to generate your website.
6. Now that all the necessary files have been created you can host your website! Open a new tab and type *account_name*.github.io into the search bar. The static website that you just hosted should appear! Congratulations, you just hosted your first website.
## 5. More Resources
- A reference for basic Markdown syntax https://www.markdownguide.org/basic-syntax/
- The official Github guide to hosting a website:https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- A guide for how to get started with using Github: https://docs.github.com/en/get-started/start-your-journey/hello-world
- For a guide on how to personalize your _config.yml file to make the website unique: https://www.educative.io/blog/yaml-tutorial
## 6. Authors and Acknowledgments 
- Thanks to tsudere for creating the resume theme. Link to the resume them page: (https://github.com/pages-themes/slate)
- Thanks to Barbara and Eric for reviewing this README and resume
## 7. FAQs 
### Why is Markdown better than a word processor?
One advantage of Markdown is that it is very simple to pick up and learn. It is also very versatile and can be used to format almost anything!
### Why is my resume not showing up?
There are many possible reasons for this to occur. Some common issues are:
- Github takes some time to build your website after your changes are commited. Simply waiting for 5 minutes after commiting your work could give Github fix the issue
- Ensure that the name of your respository is *account_name*.github.io. Github will not show your website otherwise
