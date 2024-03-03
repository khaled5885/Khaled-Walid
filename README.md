# <h1>
  Hey there
  <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px"/>
</h1>
#Python programmer
AI Developer
<div align="center">
  <img src="https://github.com/khaled5885/Khaled-Walid/blob/main/Well-paying-Tech-Jobs.jpg" width="600" height="300"/>
</div>


<picture>
  <source
    media="(prefers-color-scheme: dark)"
    srcset="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg"
  />
  <source
    media="(prefers-color-scheme: light)"
    srcset="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake.svg"
  />
  <img
    alt="github contribution grid snake animation"
    src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake.svg"
  />
</picture>




### :man_technologist: About Me :
I am  AI Developer <img src="https://media.giphy.com/media/WUlplcMpOCEmTGBtBW/giphy.gif" width="30"> from Egypt.

---

### :hammer_and_wrench: Languages and Tools :

Computing
How to Create an Impressive GitHub Profile README
Career Advancement
Developer Tools
Nida Khan
Nida Khan
January 26, 2022
Share





If you visit my profile on GitHub, you’ll notice that it contains images, social network links, some GitHub statistics and links to my blogs, which makes the GitHub profile stand out. This is possible through the GitHub profile README feature. In this article, we’ll learn how to create a GitHub profile README.

We’ll cover the following:

what a GitHub profile README is
how to create a GitHub profile README
adding social badges, skills and descriptions about oneself
adding GitHub stats
creating a GitHub workflow to pull latest published blogs
To follow along with the tutorial, you’ll need to have a basic understanding of HTML and Markdown. If you’d like an introduction to Markdown, check out this Markdown introduction. Also, you should have a GitHub account. If you don’t have one yet, sign up at GitHub.

The code for this tutorial is available on GitHub.
What a GitHub Profile README Actually Is
Build Your Own Developer Portfolio
A GitHub profile README is a feature of GitHub that allows users to use a Markdown file named README to write details about themselves such as their skills, interests, GitHub stats and showcase it to the GitHub community. It’s shown at the top of your GitHub home page, above the pinned repositories. This is a fancy way to showcase one’s skills and stats on GitHub.

Pictured below is the final look of the GitHub profile that we’ll create for this article.

GitHub profile readme GIF
We’ll divide this into multiple sections and add contents for each section incrementally. The background color will change based on the GitHub theme settings of the user.

In the next section, we’ll look at the steps for creating the README file.

Creating a GitHub Profile README
The README file resides in a GitHub repository, the name of which is the same as the username of your GitHub account. To create the repository, follow these steps:

Log in to GitHub.
Click on + icon at top right of the page and select New Repository.
GitHub Create Repository
A Create a new repository page opens. In the Repository name field, enter the username of your GitHub account. After entering the username, GitHub displays a message describing that you’re about to create a GitHub special repository.
Repository name input field
Check the Public checkbox under repository type to make the GitHub profile README visible to everyone who visits the GitHub profile page. If you don’t want users to see your GitHub profile README while it’s still in development, you can choose Private. Once you’re done with the complete development of your README, make sure to change the visibility to Public.
Check the Add a README file checkbox. This will add a README.md file where we’ll add the profile contents. The field values should look similar to thepicture below.
Create repository form fields
Click on the Create repository button. A special repository is created successfully. Go to the repository you just created and you’ll see a README.md file added to the repository.
Special repository created
In the next few sections, we’ll add contents to our README.md file. We’ll use GitHub’s file editor to write and preview the changes. You can use any other text editor you’re comfortable with.

To use the GitHub file editor, open README.md and click on the Edit this file icon (a pencil icon) on the top right of the page. You can read more about editing GitHub files at the official GitHub documentation on editing files.

Build Your Own Developer Portfolio
Adding GIFs and Badges to Your GitHub Profile README
Here’s an image of the content that will be added in this section:

Header section
The GIF used in this section can be found here. I found this GIF on Giphy, which is full of free GIFs to use.

Go to the GIF Link and click on the Share button and then Copy GIF Link. We’ll add this copied link to an HTML img tag to display it in the Markdown file. We’re using the img tag as it’ll help us specify the width of the image.

In the GitHub file editor, replace the README.md file content with the following code:

<div id="header" align="center">
  <img src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" width="100"/>
</div>
The src attribute points to the URL we copied in the previous step. Since all the contents in this section are center-aligned, we’ve wrapped the image in an HTML div tag with the align="center" attribute.

Note: GitHub converts the README Markdown to HTML and renders it on GitHub. After conversion, the HTML is sanitized, and for security reasons, it ignores certain HTML tags and attributes such as <script>, <style>, style etc. For this reason, we’ve used an align attribute instead of CSS.

Now go to the preview tab. Pictured below is the output we get.

Build Your Own Developer Portfolio
GIF preview
Next, we’ll add social network badges. On clicking the badge, it will redirect to the respective social networking sites. You can add social badges of various websites like Instagram, Facebook, Twitter, etc. For this tutorial, we’ll add three: Twitter, YouTube and LinkedIn.

To get the respective badges for each social network, we’ll use Shields.io, which provides various endpoints letting users create and customize social badges. We’ll use the https://img.shields.io/badge/ URL and pass additional parameters to this URL to get the respective social badges.

The first parameter we’ll pass is of the following format:

Label-Color
Label is the social network site name shown on the badge.
Color is the color of the badge.

For the three social networks, the values for this parameter will be:

LinkedIn: LinkedIn-blue
Twitter: Twitter-blue
YouTube: YouTube-red
When combined with https://img.shields.io/badge/, the following URL is created for LinkedIn:

https://img.shields.io/badge/LinkedIn-blue
Build Your Own Developer Portfolio
After entering the above URL in the browser, we get the following output:

Linkedin badge with no styling
Note that we don’t have the icon for the badge added yet. To add it, we’ll use two query parameters in the following format:

logo={your social network icon name}
logoColor={color of the icon}
We’ll add both the parameters to the URL as below:

https://img.shields.io/badge/LinkedIn-blue?logo=linkedin&logoColor=white
We’ll also add a style parameter to the above URL. There are various styling options available, the details of which you can find at Shields.io. We’ll use for-the-badge styling.

The final URL for LinkedIn will be:

https://img.shields.io/badge/LinkedIn-blue?logo=linkedin&logoColor=white&style=for-the-badge
Now, when we hit this URL in the browser, we get the output pictured below.

Build Your Own Developer Portfolio
Linkedin badge with styling
Similarly, we create URLs for other badges:

https://img.shields.io/badge/YouTube-red?style=for-the-badge&logo=youtube&logoColor=white
https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white
We’ll wrap each URL in img tag like so:

<div id="badges">
  <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
  <img src="https://img.shields.io/badge/YouTube-red?style=for-the-badge&logo=youtube&logoColor=white" alt="Youtube Badge"/>
  <img src="https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter Badge"/>
</div>
We’ve wrapped the images in <div> tags to make sure all badges come on a single line. The above code will only display the image generated from the URL. To add hyperlinks for each of the badges, we’ll wrap each image with an <a> tag.

Add the below code inside the <div> tag with id="header" and after the GIF <img> tag. Make sure to change the href attribute to point to your social profiles:

<div id="badges">
  <a href="your-linkedin-URL">
    <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
  </a>
  <a href="your-youtube-URL">
    <img src="https://img.shields.io/badge/YouTube-red?style=for-the-badge&logo=youtube&logoColor=white" alt="Youtube Badge"/>
  </a>
  <a href="your-twitter-URL">
    <img src="https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter Badge"/>
  </a>
</div>
Pictured below is the output we get.

Badges preview
Build Your Own Developer Portfolio
Next in this section, we have a profile views counter. It counts the number of visits your GitHub profile gets. We’ll use an open-source project that offers the view-counter badge, the documentation of which is available at GitHub Profile Views Counter. We use it in a similar way we used the social badges. Below is the endpoint for the same. We’ll also added some styling parameters to this URL:

https://komarev.com/ghpvc/?username=your-github-username
Add the below code after the <div> tag with id="badges". Make sure to replace your-github-username with your username:

<img src="https://komarev.com/ghpvc/?username=your-github-username&style=flat-square&color=blue" alt=""/>
Pictured below is the output we get.

Profile counter preview
The last part of this sections is text with a wave (:wave:) GIF. The GIF is taken from Giphy and can be found here.

Add the below code after the profile view counter <img> tag:

<h1>
  hey there
  <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px"/>
</h1>
The output is pictured below.

Build Your Own Developer Portfolio
Hey there text preview
Save the changes by clicking on the Commit changes button. This completes the first section of the GitHub profile README. Let’s move to adding more content to our README.md file.

Adding a Banner GIF and About Me Section
Here’s what we’ll be adding to our profile page in this section:

About me section
In this section, we’ll add GIF and some words describing details about ourself. You can find the GIF here.

To add the GIF, we’ll use an <img> tag, specify a height and width and wrap it inside a <div> to center the GIF using align="center". Add the following code to your README.md file:

<div align="center">
  <img src="https://media.giphy.com/media/dWesBcTLavkZuG35MI/giphy.gif" width="600" height="300"/>
</div>
The output of this is shown below.

GIF banner preview
Build Your Own Developer Portfolio
Next, we’ll add the contents for the About Me section. For the description text we’ll use Markdown syntax, as we don’t need any sort of alignments. Append the below code in README.md:

---

### :woman_technologist: About Me :
--- is to add a horizontal rule before a new section. A horizontal rule in Markdown should be surrounded by blank lines. :woman_technologist: is the shortcode for the emoji used. For a male version, you can use :man_technologist:. For others, you can use :technologist:. You can find a list of emojis and the corresponding shortcodes in the GitHub repo.

Next, we’ll add a personal one-line introduction and use a wave (:wave:) GIF. Append the below code to README.md:

I am a Full Stack Developer <img src="https://media.giphy.com/media/WUlplcMpOCEmTGBtBW/giphy.gif" width="30"> from India.
Next is a list of points about yourself. To display a list, we’ll use - Markdown syntax. We’ll also prefix each line with an emoji. Add the following code to README.md and make changes according to your profile. Also, change your-linkedin-url to your profile URL:

- :telescope: I’m working as a Software Engineer and contributing to frontend and backend for building web applications.

- :seedling: Exploring Technical Content Writing.

- :zap: In my free time, I solve problems on GeeksforGeeks and read tech articles.

- :mailbox:How to reach me: [![Linkedin Badge](https://img.shields.io/badge/-kakbar-blue?style=flat&logo=Linkedin&logoColor=white)](your-linkedin-url)
Note that in the last line, the inner ![]() syntax is to display the LinkedIn badge image. The outer []() is Markdown hyperlink syntax to make the badge point to the LinkedIn profile URL. We’ve used Shields.io here for displaying a customized LinkedIn badge. You can also add any other links where people can reach out to you.

See the output in the picture below.

About yourself description preview
Build Your Own Developer Portfolio
Adding Languages and Tools
Here’s a picture of the content that we’ll add in this section.

Languages and tools section
For the heading, add the following code to README.md:

---

### :hammer_and_wrench: Languages and Tools :
We’ll add images representing technologies and skills one holds. You can find several free logos for many languages and tools in the DevIcons GitHub Repository.

Go to the icons folder and search and open the react folder. You’ll find images in SVG and EPS format. Click on any image and copy the URL shown in the browser’s address bar.

DevIcons react logo
We’ll use this URL in the <img> tag and specify the height and width attribute accordingly. Similarly, you can search for other skills and add them in separate <img> tags.

Append the below code to README.md. Add/remove the necessary skills you want in your profile:

Build Your Own Developer Portfolio
<div>
  <img src="https://github.com/devicons/devicon/blob/master/icons/python/python-original.svg" title="Python" alt="Python" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/anaconda/anaconda-original.svg" title="Anaconda" alt="Anaconda" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/linux/linux-original.svg" title="Linux" alt="Linux" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/microsoftsqlserver/microsoftsqlserver-original-wordmark.svg" title="microsoftsqlserver" alt="microsoftsqlserver" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/mysql/mysql-original-wordmark.svg" title="mysql" alt="mysql" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/vscode/vscode-original.svg" title="vscode" alt="vscode " width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/css3/css3-plain-wordmark.svg"  title="CSS3" alt="CSS" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/html5/html5-original.svg" title="HTML5" alt="HTML" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/javascript/javascript-original.svg" title="JavaScript" alt="JavaScript" width="40" height="40"/>&nbsp;
</div>


---

### :writing_hand: Blog Posts :

