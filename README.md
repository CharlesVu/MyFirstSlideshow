# Yoti Technical Tests

### Document version 1.0.3

Please read this document carefully before continuing the exercise. In case you don't follow the rules described your test will be rejected.

**Do**:
- Clone and commit the project locally
- Send us a patch file
- Send comments either in a markdown formatted mail or a PDF (not both)
- Use when possible a monospaced font (Hack, Anonymous Pro, Menlo, Monaco, …)
- Reply in English

**Don't**:
- Fork the project
- Submit a Pull Request on the repo
- Comment on any of the issues or Existing Pull Requests
- Submit a solution made by someone else


## Exercise 1

This first exercise is rather simple and should take at most one hour.  
The README should tell you what the project is trying to achieve and what are the limitations.
You should send us a code review of the first pull request on the list. 

Each comment should have the one of following format :
```
<filename>:<linenumber> - “<your comment>”
e.g:
main.m:42 - “This ASCII art should be a cat”
```
```
<filename>:<start line>-<end line> - “<your comment>”
e.g:
main.m:42-922 - “This ASCII art needs more colour”
```
```
<feature> - “<your comment>”
e.g:
MyFeature - “Should be renamed to ASCIICat”
``` 

Don’t limit your PR review to “this is bad”, please ellaborate and provide a better solution (in pseudo code) as you would explain it to another developer.  
We are not looking for an (re)implementation of the presented code at this stage.

## Exercise 2

The second exercise is described in the issues tab on the github project. You need to read all the issued described in the Issues section of the repository and resolve them. 

- Re-implement the project as if the feature was given to you.  
- You are not requested to implement a completely different design unless you want to but the UI elements implemented should be flexible enough to be re-used (try to hardcode the least values as possible).  
- We don’t expect any bonuses.
- Don’t use any external frameworks (we know that most of what we asked can be solved by just importing one).  
- If you need more time, please email us.
- This is not a speed contest, we do prefer you taking the full allocated time and send us a better solution than rushing for a solution which is sub-optimal.  
- Send us your commit logs attached with your answer.


# MyFirstSlideshow

For people who browse random repositories (hello by the way), this is just a technical exercise that reflects how projects are developed in a lot of companies: Someone writes code based on some specifications, someone else reviews their code then it gets merged when everyone is happy. Then, the specifications changes, an issue is created and someone needs to fix that.

This "app" is a rather simple one.
It's only one screen divided into two areas. The app should display images represented by their URL in an array of 4 elements
``` 
["https://c1.staticflickr.com/6/5615/15570202337_0e64f5046e_k.jpg",
 "https://c1.staticflickr.com/4/3169/2846544061_cb7c04b46f_b.jpg",
 "https://i.redd.it/d8q1wkgu1awy.jpg",
 "http://www.kapstadt.de/webcam.jpg"]
 
  // Images under Creative Commons
  // Images attributed to (in order) https://www.flickr.com/photos/_torne/
  // https://www.flickr.com/photos/chrisyarzab/
  // https://www.reddit.com/user/lalien42/
  // http://www.kapstadt.de/
```
(PS. the last one is temporary as we will create new service which will help this exercise)

The two areas will work the same way. Each of them will have a button to cycle to the next image, an index indicator and a zone to display the image. 

The **branch** "slideshow" is currently respecting the above "specifications" but with some caveats.