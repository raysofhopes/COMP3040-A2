# Hosting a Resume on GitHub Pages

## Purpose

This guide aims to explain how to host a website on GitHub Pages, focusing on hosting a resume. It also introduces the principles of Modern Technical Writing by Andrew Etter, demonstrating these principles through the process.

## Prerequisites

- A GitHub account
- A Markdown-formatted resume
- Basic knowledge of git commands
- (Optional) Download and install Jekyll

For a detailed Markdown tutorial, [click here](https://www.markdowntutorial.com/).

## Instructions

### Creating a Markdown Formatted Resume

1. **Install a Markdown Editor**: Download and install a Markdown editor like Visual Studio Code or use an online editor like [dillinger](https://dillinger.io).
2. **Write Your Resume**: Use Markdown syntax for formatting. For headers, use `#` for the main title, `##` for sections, `-` for bullet points.
3. **Save Your Resume**: Save the file as `resume.md`.
4. **From Etter's book**: Andrew Etter in their book emphasizes that Markdown is an incredibly versatile and widely used lightweight markup language, praised for its clean syntax that makes it accessible to many. 
    Despite its simplicity, Markdown's limited feature set and the lack of a single defined standard have led to the creation of numerous "flavors" like MultiMarkdown, Markdown Extra, GitHub Flavored Markdown, and CommonMark, each aiming to extend its capabilities.
    And thus creating your resume in md file format ensures a universally readable format that combines simplicity with the flexibility to showcase your professional profile effectively across various platforms.

### Downloading and Installing Jekyll

1. **Install Ruby**: Ensure Ruby is installed on your system. Use `ruby -v` to check the version.
2. **Install Jekyll and Bundler**: Run `gem install jekyll bundler`.
3. **Create a Jekyll Site**: Navigate to your project directory and run `jekyll new . --force`.
4. **Build and Serve Your Site Locally**: Execute `bundle exec jekyll serve`. Visit `http://localhost:4000` to see your site.
5. **From Etter's book**: Andrew Etter highlights the significant advantages of static websites, such as their speed, simplicity, portability, and security, making them an excellent choice for hosting on platforms like Amazon S3 and GitHub Pages. Among the tools for creating static sites, Jekyll stands out for its popularity and effectiveness, particularly for those who value a straightforward development process without compromising on the ability to produce complex, feature-rich sites.
    Jekyll's integration with GitHub Pages offers a seamless workflow for developers, allowing them to directly deploy their static websites from a GitHub repository. This synergy not only simplifies the deployment process but also leverages GitHub's robust platform for version control and collaboration, making website updates as easy as pushing a commit.

### Enabling GitHub Pages

1. **Push Your Site to GitHub**: Use `git init`, `git add .`, `git commit -m "Initial commit"`, and `git push -u origin main`.
2. **Enable GitHub Pages**: Go to your GitHub repository settings, find the GitHub Pages section, and select the `main` branch as the source.
3. **From Etter's book**: Andrew Etter advocates for the use of distributed version control systems (DVCS) like Git and Mercurial in documentation workflows, emphasizing their advantages over centralized systems. The primary benefits he outlines include improved performance, the ability to work offline, and superior handling of concurrent edits to the same file. However, the most compelling reason for technical writers to adopt DVCS is its preference among developers.

### Things to Keep in Mind

#### Repository Naming
**Required**: For your GitHub Pages site, ensure the repository is named `username.github.io`, replacing `username` with your GitHub username. This specific naming convention is crucial for GitHub to recognize the repository as a GitHub Pages site and automatically serve it at `http(s)://username.github.io`.

#### Content Organization
*Optional*: Keep your repository organized by using folders for different sections of your site (e.g., `/blog`, `/projects`) and maintain a clean root directory. Use a `README.md` file to provide an overview of your repository and instructions for visitors.

#### Custom Domain
*Optional*: If you prefer a custom domain over the default `github.io` domain, you can configure it in your repository's settings under the GitHub Pages section. Remember to update your DNS settings accordingly.


## Animated GIF

![myresumeGIF](https://i.makeagif.com/media/3-06-2024/tQWaxb.gif)

## More Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdowntutorial.com/)

## Authors and Acknowledgements

Thank you to Andrew Etter for his insightful book on Technical Writing.

Also a big thank you to my team members Jahidul and Shadib for helping with error checking and analysis.

## FAQs

1. **Why is Markdown better than a word processor?**
  Markdown is lightweight, portable, and can be easily converted to HTML, making it ideal for online hosting.

2. **Why is my resume not showing up?**
  Ensure you've enabled GitHub Pages in your repository settings and the file is named `index.md` or correctly linked in your `_config.yml`.

## Software Stack Used

- Markdown
- Visual Studio Code (or your preferred Markdown editor)
- GitHub Pages
- Jekyll
