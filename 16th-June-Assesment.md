to read - https://stackoverflow.com/questions/5641997/is-it-necessary-to-write-head-body-and-html-tags
task:-
 1.  create a simple html file containing of elements that helps to build a rough portfolio
 2. ** doc for the difference between <div>, <article>, <section> tag?**
Answer - Both the tags are semantics tag in HTML 5. Both the <article> and <section> tags are represented in a similar way but used for some meaning, that meaning is for the browsers and the developers. Both tags can replace each other as there will be no changes to the outputs, but it will be difficult to understand by the developers and the browsers to act on those content.
 
<div> Tag : The div tag is known as Division tag. The div tag is used in HTML to make divisions of content in the web page like (text, images, header, footer, navigation bar, etc). Div tag has both open(<div>) and closing (</div>) tag and it is mandatory to close the tag. The Div is the most usable tag in web development because it helps us to separate out data in the web page and we can create a particular section for particular data or function in the web pages.

Div tag is Block level tag
It is a generic container tag
It is used to the group of various tags of HTML so that sections can be created and style can be applied to them.
As we know Div tag is block-level tag
 
<article> Tag: This tag contains independent content that doesn’t require any other context. So the <article> tag can be placed inside the main content. But each of the articles will contain independent content within it. Like YouTube use to contain different kinds of videos on a single page, each video is independent .
Feature:
An article can have nested articles and that should refer to parent article.
Article tags are perfect for Microdata information.
 
<section> Tag: This tag is used to split a page into sections like Introduction, Contact Information, Details, etc and each of these sections can be in a different <section> tag. The <section> tag is introduced to wrap-up the things in a particular section. The <section> tag divides the content into sections and subsections. The section tag is used when requirements of two headers or footers or any other section of documents needed. Section tag grouped the generic block of related content.
Feature:
A section can have nested sections
Note: Placing <article> tag inside of <section> tag is good practice, like section basically defines the types and the articles will contain the specific contents in that type of section.
 3.    write a doc for the following below
        typeof(1)            - number
        typeof(1.1)          - number 
        typeof('1.1')        - string
        typeof(true)         - boolean  
        typeof(null)         - object
        typeof(undefined)    - undefined
        typeof([])           - object
        typeof({})           - object
        typeof(NaN)          - number
 4.   read what is prototype
 Answer:- https://www.geeksforgeeks.org/prototype-in-javascript/
