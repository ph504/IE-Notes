<!-- ================================================== a heading here ================================================ -->
<h1><u><b>
		Internet Engineering
		Shahid Beheshti University, <br/>
		Computer Science and Engineering Faculty
		Instructed By: Parham Alvani
		Author: Arya Parvizi
	</b></u>
	
</h1>

## __TAGS USED:__

- LSS = LONG STORY SHORT
- OOL = OUT OF LESSON
- PSD = PREVIOUS SESSION DISCUSSION
- BYD = BY DEFAULT
- DFW = DIFFERENCE WITH
- ATST = AT THE SAME TIME
- MQUESTION = MY QUESTION
- OQUESTION = OTHER'S QUESTION
- E.G. = FOR EXAMPLE
- OPT = OPTIONAL
- AMAP = AS MUCH AS POSSIBLE
- IMP = IMPORTANT
- TBRL = TO BE REVIEWED LATER
</b>

# <u><b>7th Session : HTML</b></u>


## **INTRODUCTION**

<p>
	<b>PSD: </b>HTTP was the process of how to get a resource.
	HTML is one of the most important resources --&gt; from the concept of documents and papers published until now to share.
	the beginning of the story was the idea for sharing documents (WWW).
</p>
<b>Ouestion:</b>
HOW TO DEFINE STRUCTURES OF DOCUMENTS?
a document includes different parts (e.g. tables, figures and images, links and etc.)
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>BINARY FORMATS : USELESS</b>
</h3>
not readable formats.
old days: there was nothing
there was hardly ever graphical popular binary formats: PDF, Doc, ...
different architectures little-endian and big-endian issue. makes the reading from binary formats much harder.

<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>TEXT format</b>
</h3>
ASCII text
open and edit and readable and available in every machine. also no little-endian and big-endian issue.

<b>Question:</b>
how to format the doc though?
(header, footer, paragraph, table, etc.) (e.g. LaTeX, Word, etc.)
<b>Solution:</b>
MARK UPS!

<!-- ================================================== a heading here ================================================ -->
<b>Hyper Text Markup Language.</b>
<b>The main purpose and goal :</b> defines the structure. we do it with tags. (predefined markups)
HTML defined with SGML 
not a programming language (no calculation can be done with it, it is a description language.)
CSS is used for presentation specification, HTML is only responsible for the structure (not the font, color, style, etc.)
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>Standardizing HTML</b>
</h3>
<b>HTML 1</b> <b>(OOL: </b>(Berners-Lee, 1989), basic, limited)
<b>HTML 2.0</b> <b>(OOL: </b>(IETF, 1994): tried standardizing and adding some features)
<b>HTML 3.2</b> (W3C 1996) tried: unifying to a single standard
<b>HTML 4.0</b> (W3C 1997) tried: map of future.
<b>XHTML 1.0</b> (W3C 2000)(adding more structures to the html files to limit the formats and templates.) modified to confirm <b>XML</b> standards.
<b>HTML 5</b> added many more features which was combined with javascript.
<!-- ================================================== a heading here ================================================ -->
<h2>
	<b>Tags:</b>
</h2>
<b>XHTML = HTML in this lecture, which is a set of elements.</b>
<b>element : </b> a pair of tags(open/close) + content in between (content is <b>OPT</b>) e.g. &lt;h1&gt;This is header&lt;/h1&gt;

&lt;tagname&gt; : open
&lt;/tagname&gt; : close
&lt;tagname/&gt; : self-closing tag (usuallly for tags that have no content)
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>ATTRIBUTES</b>
</h3>
<b>format : </b>
attname = "value in double quote"
<b>example : </b>
&lt;tagname attrib1="setting" attrib2="setting" ...&gt;
...
&lt;/tagname&gt;
no att for closing tags.
some <b>core attribs</b> that most tags have:
<b>id: </b> a unique identifying thing starting with character, for the element, have different other uses too.
browsers want to show the content <b>AMAP</b>, they're responsible for rendering html too. so they ignore html's issues <b>AMAP</b>. to give user the best exp. because the user isn't an omniscient to know if the html file of the server has problems.
<b>class: </b> assign a/some class(es) to the element 
(uniqeness of the id might come with issues later because of browsers mechanisms (in case the id is not unique for example.))
<b title="for example this thing you're seeing is a title. :)">title: </b> give more info about the element, hover on <b title="for example this thing you're seeing is a title. :)">"title" </b> to see what I mean.
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>general structure of tags</b>
</h3>
&lt;tag attribute = "attribute value"&gt;content&lt;/tag&gt; 
<b>example : </b>
&lt;h1 class="primary"&gt;Example Heading&lt;/h1&gt;
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>HTML PROCESSING</b>
</h3>
main discussion.
different goal of html (not limited to browser rendering) --> 
<b>
	search engines, browsers rendering, pdf, etc.
</b>

<b>search engines : </b> doesn't use your html to render, they just get information and analyze the structure and prioritize and rank the websites (<b>E.G.</b> using "fish farm" phrase in your title has more priorty than a website that just mentioned a "fish farm" in a relevant topic).
<b>browsers : </b> just render.
not all tags are rendered. (<b>E.G.</b> &lt;head&gt;) 
some tags are for render but themselves aren't rendered, <b>E.G.</b> &lt;h1&gt; is not rendered itself, the browser just renders the content
note : each tag has a default render presentation (<b>E.G.</b> headings have bold and bigger fonts.)


<b>LSS:</b> some tags have content but are not rendered, <b>E.G.</b> &lt;head&gt;
some have contents and are also rendered 

<h4>
	<b>&lt;em&gt;</b> tag
</h4>
<b>E.G.</b> &lt;em&gt;italic, this tag is for emphasis&lt;/em&gt; 
<b>RESULT</b>= <em>italic, this tag is for emphasis</em>

<h4>
	<b>&lt;br&gt; OR &lt;br/&gt;</b> tag
</h4>
some tags don't have content but are rendered. <b>E.G.</b> &lt;br/&gt;
line&lt;br/&gt;newline 
<b>RESULT</b>= is below!
linenewline
<h4>
	<b>&lt;h1&gt;</b> tag
</h4>
&lt;h1&gt;the tag and the purpose of the tag won't be rendered.&lt;/h1&gt;
<b>RESULT</b>= is below! <h1>the tag and the purpose of the tag won't be rendered.</h1> 

<!-- ================================================== a heading here ================================================ -->
<h2>
	<b>HTML RENDERING</b>
</h2>
browsers top-bottom, left to right reading to render.
<b>in-line</b> and <b>block-level</b> elements 
<b>block-level: </b>take one line for each element.(<b>E.G.</b> heading tag)
<b>in-line: </b>don't take the whole line they are put together in a single line.(<b>E.G.</b> bold tag)
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>ignored by browsers:</b>
</h3>
&lt;!-- which is comment (like // and /**/ in C) --&gt;
&lt;not recognizable tags&gt;
&lt;more than single whitespaces&gt; (spaces + newlines + tabs = single space)
&lt;br&gt; tag is more useful for poems rather than seperating paragraphs. other purposes such as the latter is done by css rather than html. if you want to fit a paragraph css itself will break as much as it needs, so be aware of what you're doing.
<b> OQUESTION by A. BOHLOOLI : </b> <b>ANSWER :</b> other reasons and issues: 
1. different sizes in three scales (responsive design which is more discussed in css).
2. makes developement so hard and conflicts are many more.

<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>
		hello world Example:
	</b>
</h3>
&lt;html&gt;
 &lt;head&gt;
&lt;title&gt; shown in the window or tab (used by search engines and browsers)&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
shown to the user
&lt;p&gt; Hello World! &lt;/p&gt;
&lt;/body&gt;
&lt;/html&gt;
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>
		description for example above
	</b>
</h3>
<h4>
	<b>&lt;html&gt;</b> tag
</h4>
every content in html file is between these two tags.(open-close html tag)
has only two children (Nothing More) : head and body
<h4>
	<b>&lt;head&gt;</b> tag
</h4>
not shown to the user.
used by search engines.
page descriptions, page keywords.
<h4>
	<b>&lt;body&gt;</b> tag
</h4>
shown to the user.
<!-- ================================================== a heading here ================================================ -->
<h3>
	NESTED TAGS
</h3>
a tree relation between the tags which is really <b>IMP</b>
root -&gt; head&body --&gt; (sth CHILD FOR HEAD)&(sth CHILD FOR BODY) etc.

<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>SPECIAL CHARACTERS</b>
</h3>
special characters as a symbol encoded in html can be used.
parsing issues characters.
although today these can be rendered normally, it is best to still the codes rather than the character itself, like below:
<!-- table to be added here. -->
<b>&lt;</b> ::: &amp;lt; ::: ASCII : &amp#60;
<b>&gt;</b> ::: &amp;gt; ::: ASCII : &amp#62;
<b>&amp;</b> ::: &amp;amp; ::: ASCII : &amp#38;
<b>'&nbsp; this was a forced whitespace'</b> ::: &amp;nbsp; ::: ASCII : &amp#160;
or characters which are not accessible from keyboard (E.G. UTF-8 characters) : 
<b>&copy;</b> ::: &amp;copy; ::: ASCII : &amp#160;
<b>&lambda;</b> ::: &amp;lambda; ::: ASCII : &amp#955;
but nowadays!!! --&gt; utf-8 characters are allowed.
<h4>
	other characters by my interest:
</h4>
<b>
&Omega;, &omega;, &Theta;, &theta;, &Alpha;, &alpha;, &Beta;, &beta;, &Gamma;, &gamma;, &Zeta;, &zeta;, &Sigma;, &sigma;, &Phi;, &phi;
こんなやり過ぎは申し絵分けございませんでした。&#128513;&#128517;😅
</b>

<!-- ================================================== a heading here ================================================ -->
<h2>
	<b>XHTML</b>
</h2>
HTML is a subset of <b>SGML</b> = Standard General Markup Language.
XHTML application of <b>XML</b> = Extensible Markup Language.

XML <b>DFW</b> SGML
XML is more restricted than SGML
XHTML is more restricted than HTML
XHTML is more well-defined.

<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>XHTML RESTRICTIONS:</b>
</h3>
<h4>
	forced self-closing.
</h4>
&lt;br/&gt; (forced self-closing)(endings are mandatory so there should be no open tag without content or end tag)
<h4>
	no tag overlap
</h4>
<b>E.G.</b> 
&lt;strong&gt;&lt;em&gt;test&lt;/strong&gt;&lt;/em&gt;
<b>because</b> the child or parent aren't determinant
<h4>
	all tags lower case.
</h4>
<h4>
	attributes values must be in double quote.
</h4>
<h4>
	browsers should ignore unknown tags/attributes.
</h4>
<h4>
	layout(=style) should be seperated from markup.
</h4>
markup should only be used to indicate the <b>semantic</b> and the <b>structure</b>.

<h4>
	removing some tags
</h4>
<b>&lt;big&gt;</b> tag was to show the font size is big.
<b>E.G.</b> = &lt;big&gt;this&lt;/big&gt; is in big font size.
<b>RESULT</b> = <big>this</big> is in big font size.

<b>&lt;center&gt;</b> tag which was to put the content in the center of page.
<b>E.G.</b> = &lt;center&gt;put it in center&lt;/center&gt;
<b>RESULT</b> = <center>put it in center</center>

these are implemented by <b>CSS</b> so it is not needed anymore.
<!-- ================================================== a heading here ================================================ -->
<h3>
	Bigger Example of HTML:
</h3>
&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
&lt;head&gt;
&lt;meta charset="utf-8"&gt;
&lt;title&gt;
My test page
&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
&lt;img src="pathname..." alt="My example image"&gt;
&lt;/body&gt;
&lt;/html&gt;
<!-- ================================================== a heading here ================================================ -->
<h3>
	discription for above example:
</h3>
<h4>
	&lt;!DOCTYPE html&gt; tag
</h4>
it had meaning in the past but it is nothing special anymore.
ATT: <b>lang</b> telling the language of the website. if your document is multi-lang you have to change the attrbute.
<h4>
	&lt;title&gt; tag
</h4>
it's the titr of the website.
<h4>
	&lt;meta&gt; tag
</h4>
meta data tag for the website.
ATT: <b>charset</b> telling that we are using a "utf-8"encoding in our website.
<h4>
	&lt;img&gt; tag
</h4>
loading an image in the body.
ATT: <b>src</b> is the source/path of the file.

##	&lt;!DOCTYPE HTML&gt;

for error checking purposes of html and announcing the html version and etc. and it would check the rules that should be asserted.
<b>in todays : </b> for after versions of xhtml (html 5) everyone is using html 5 so we don't really need this one anymore. __BYD__

## HTML ELEMENTS
<ol>
	<li>
		<h4>
			Main root (html tag) 
		</h4>
	</li>
	<li>
		<h4>
			Document metadata  
		</h4>
		<p>
			(things we see in head tag)
		</p>
	</li>


#### __these belows are used in body tag:__
<li>
	<h4>
		Sectioning root (<b>I.E.</b> body tag)
	</h4>
	<p>
		each html doc can have only <b>one</b>body
	</p>
</li>
<li>
	<h4>
		Content sectioning
	</h4>
	<p>
		these tags may not change the appearance, but they're greatly impacting the contents.
	</p>
<p>

`<h1>` tag represents the highest section level. the strongest and most impacting heading.

`<section>` a bunch of independant sections.

</p>
</li>
	<li>
		<h4>
			Text content	
		</h4>
	</li>
	<li>
		<h4>
			Inline text semantics	
		</h4>
	</li>
	<li>
		<h4>
			Image and multimedia
		</h4>
	</li>
	<li>
		<h4>
			Embedded content
		</h4>
	</li>
	<li>
		<h4>
			Scripting	
		</h4>
	</li>
</ol>

### <b>content</b> sectioning 
(logically and contently partition the document.)
titrs (h1-h6)

#### &lt;section&gt; tag 
when to use: to seperate parts which don't have semantic load (e.g. seperate slides and gmail tabs. later we can apply different styles to different sections using css.)

example :

&lt;footer&gt;this is a section&lt;/section&gt;

RESULT = <section>this is a section</section>

#### &lt;footer&gt; and &lt;header&gt; tag 
<b>has semantic </b> this footer of the nearest section/content (e.g. copy right)

'&lt;footer&gt;this is a footer example.&lt;/footer&gt;'

RESULT = <footer>this is a footer example.</footer>

as you can see there is no default rendering for footer/header in the browser.


#### &lt;nav&gt; tag 
<strong>has semantic </strong>

for guiding the map of website.
e.g. home, shop.

#### &lt;p&gt; tag 
put the content in this tag

#### &lt;pre&gt; tag 
<strong>exactly as written</strong> e.g. for codes (e.g. python)

<pre>
	// this is a java code.
	public class HelloWorld{
		public static void main(main(String[] args){
			System.out.println("hello world!");
		}
	}
</pre>


### lists:
__`<ol>`__ tag ordered lists (`#` render <strong>BYD</strong>)

__`<ul>`__ tag unordered lists (bullet render <b>BYD</b>)

__`<li>`__ tag the elements of the list. (list item) (ordered/unordered)

__`<dl>`__ tag a list which has description. (the items of this list have two members {dt 
and dd})

__`<dt>`__ tag list term

__`<dd>`__ tag description

__E.G.__ dictionry

Example:
```html
<dl>
	<dt>大切</dt>
	<dd>means important</dd>
	<dt>平日</dt>
	<dd>means weekdays</dd>
</dl>
```
RESULT = 

<dl>
	<dt>大切</dt>
	<dd>means important</dd>
	<dt>平日</dt>
	<dd>means weekdays</dd>
</dl>

__`<div>`__ tag (content division, <b>DFW</b> `<section>`, `section` has different parts of the content which can have no semantical relation. but `div` can no semantic partition purpose at all, generic container to apply different styles and javascript to this divisions.)

- 	__E.G.__ different lists in the gmail have different styles. (--> `<div>`)
- 	__E.G.__ different slides have no different styles but they have different semantics.(--> `<section>`)

you can write HTML however you want, it is easy and the lesson has no computation (taarifi). / is conceptual.


# <u><b>8th Session : HTML</b></u> 

__inline semantics__

__`<span>`__ tag __DFW__ `div` 
- `div` has a line dedicated.
- `span` has a word dedicated. (__E.G.__ style, has no semantic meaning for search engines.)


__`<q>`__ tag quote. (no style but has meaning)

__`<cite>`__ tag to cite. (no style but has meaning)

__`<a>`__ tag __IMP__ used for linking.

- `<a href="">`	 attribute.
- href Attribute --> a URL.

if href URL has `http://...` means we wan to open another website. (__I.E.__ scheme is included.)

if no `/` or no scheme (`http://...`) we want to open a file here.

#### Examples:
```html
<a href="https://sbu-ce.github.io/IE-lecture/slides/lecture-3/#/">
	this is the link to the main lecture website.
</a>
```
RESULT = 
<a href="https://sbu-ce.github.io/IE-lecture/slides/lecture-3/#/">
	this is the link to the main lecture website.
</a>



