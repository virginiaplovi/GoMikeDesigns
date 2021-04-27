# GoMikeDesigns
## Optimize an Existing Website, Project 4 - Optimization report 
Screenshot of the Lighthouse report before optimization:
![Before Pic](https://user-images.githubusercontent.com/76953217/116173175-06292680-a704-11eb-9d6c-a27ad6260579.png)

### PERFORMANCE 
 
The website was presenting many issues affecting the performance of the pages.  

In order to optimize it and improve the loading speed I've moved the script from the top of the page to the bottom and reduce the impact of these render-blocking URLs by inlining critical resources, deferring non-critical resources. 

Important resources are now preloaded. 

The analytics tag has been added so the pages performance can now be tracked on both Google Analytics and Google Search Console. 

To ensure text remains during web font load I've added the font-display:swap CSS property to @font-face. 

To improve the loading speed unused code should be removed. All the CSS and JavaScript files have been minified to reduce the files sizes. 

The images are now appropriately-sized, format and compressed (compressor.io), by doing this you will save mobile data and improve load time. Explicit width and height have been added to img elements. 
 

### ACCESSIBILITY 

 
The web pages were not fully accessible. 

The html element does not have a valid value for its [lang] attribute, the “en” value has been set to allow screen readers to read with the correct pronunciation.  

Div tags have been replaced with semantic tags where necessary to give structure to the pages and to allow users to navigate the page. 

Background and foreground colours do not have a sufficient contrast ratio. Headings colour and contact buttons background-color have been changed to comply with WCAG Level AAA requirement. 

Images of text have been removed and replace it with actual text (headings and blockquote). Avoid the use of images of text, assistive technologies and Search Engines cannot read text that’s contained inside an image causing a bad experience for users and problems to index content. 

The alt attribute provides alternative information for an image if a user for some reason cannot view it and it should be descriptive and specific.  
Alt text will as well provide greater relevance to search engines about your content and help drive traffic to your site 

ARIA attribute current page and aria-label have been added to navigation to be read by screen readers for interface elements. 
Labels have been associated to form elements. Labels ensure that form controls are announced properly by assistive technologies, like screen readers. 
 
Headings structure was not present in Contact Page and more than one h1 element has been used in the home page.  
h1 tag has been added at the top of the page content in Contact page and additional h1 tags have been replaced with h2 tags from the home page. 
 

### BEST PRACTICE 

 
Browser errors were logged to the console for Contact.html 
This was due to the incorrect name used to link style sheets and scripts. By correcting this error, navigation and forms are now working correctly. 

Html and CSS validator was used to identify code errors and correct them. 
Deprecated media feature has been replaced, value errors and success-msg/ fail-msg attributes have been removed. 
 

### SEO 

 
Meta keyword has been removed as it is no longer in use by Search Engines to rank websites. 

The title of both pages has been changed to suit the content and now contains the keyword. 
 
Keyword stuffing is considered a black hat technique so the meta description of the home page and contact page, where there was no any content, have been rewritten describing the page content and integrating the keywords in a natural way. 

Content should be visible to both the user and the search engine to avoid being penalized by Google and a terrible experience for screen reader visitors so hidden content has been removed. 

Unnatural backlinks, from low-quality or spam websites, have been removed from the footer. 

Screenshot of the Lighthouse report after optimization:
![After Pic](https://user-images.githubusercontent.com/76953217/116173432-7cc62400-a704-11eb-8942-f133a1c786ac.png)
