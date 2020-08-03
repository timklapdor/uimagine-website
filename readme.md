My work has ended at CSU so I'm keeping this domain going based on an older version of the website I created. 

## Resources

- Date: https://learn.cloudcannon.com/jekyll/date-formatting/
- ICS format: https://gist.github.com/woodworker/6725728
- Colours: https://alistapart.com/article/mixing-color-for-the-web-with-sass
- Responsive needs - ```<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">```
- Maps - https://learn.cloudcannon.com/jekyll/google-maps/
- htaccess Testing - https://htaccess.madewithlove.be

## Links

- For internal links - images and links to other pages and posts - please prepend the link with ```{{ site.baseurl }}```. This will ensure that links and images load correctly.
- File Names can't have spaces. So before uploading please check.

## Includes
- To include youtube videos use ```{% include youtube.html id="KWvd8rjqPlg" %}```.
- To include slide share slides use ```{% include slideshare.html code="PASTE EMBED CODE HERE" %}``` To get the Embed Code copy the embed code snippet from Slide Share and grab the last part of the address in the iframe e.g In this case ``` <iframe src="//www.slideshare.net/slideshow/embed_code/key/xIXB1w2y8ncGat" ``` the code is ```xIXB1w2y8ncGat```
- To style APA references put text into a list then directly below on a new line add ```{: .apa }```
- For Images with captions use the Figure Inclclude: ```{% include figure.html filename="Bart-lecture-Bathurst_March2018.jpg" caption="From left to right: Tim KLapdor, Lyn Hay, Cass Colvin, Bart Rienties, Sandra Wills" %}``` Filename = just the file name - not directory. Caption = can only be plain text.
