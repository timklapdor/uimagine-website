## Resources

- Date: https://learn.cloudcannon.com/jekyll/date-formatting/
- ICS format: https://gist.github.com/woodworker/6725728
- Colours: https://alistapart.com/article/mixing-color-for-the-web-with-sass
- Responsive needs - ```<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">```
- Maps - https://learn.cloudcannon.com/jekyll/google-maps/

## Links

- For internal links - images and links to other pages and posts - please prepend the link with ```{{ site.baseurl }}```. This will ensure that links and images load correctly. 

## Includes
- To include youtube videos use ```{% include youtube.html id="KWvd8rjqPlg" %}```.
- To include slide share slides use ```{% include slideshare.html code="PASTE EMBED CODE HERE" %}``` To get the Embed Code copy the embed code snippet from Slide Share and grab the last part of the address in the iframe e.g In this case ``` <iframe src="//www.slideshare.net/slideshow/embed_code/key/xIXB1w2y8ncGat" ``` the code is ```xIXB1w2y8ncGat```
- To style APA references put text into a list then directly below on a new line add ```{: .apa }```
