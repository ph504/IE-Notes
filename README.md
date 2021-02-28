<!DOCTYPE HTML>
<!--lang="en"-->
<html>
<head>
	<title>IE HTML NOTES</title>
</head>
<body>
	<meta charset="utf-8">
<!-- ================================================== a heading here ================================================ -->
<h1>
	<u><b>
		Internet Engineering<br/>
		Shahid Beheshti University, Computer Science and Engineering Faculty<br/>
		Instructed By: Parham Alvani<br/>
		Author: Arya Parvizi<br/>
	</b></u>
	
</h1><br/>
<h2><b>TAGS USED:<br/></h2>
LSS = LONG STORY SHORT<br/>
OOL = OUT OF LESSON<br/>
PSD = PREVIOUS SESSION DISCUSSION<br/>
BYD = BY DEFAULT<br/>
DFW = DIFFERENCE WITH<br/>
ATST = AT THE SAME TIME<br/>
MQUESTION = MY QUESTION<br/>
OQUESTION = OTHER'S QUESTION<br/>
E.G. = FOR EXAMPLE<br/>
OPT = OPTIONAL<br/>
AMAP = AS MUCH AS POSSIBLE<br/>
IMP = IMPORTANT<br/>
TBRL = TO BE REVIEWED LATER
</b><br/><br/>

<h1><u><b>7th Session : <br/>HTML</b></u></h1>

<h2>
	<b>INTRODUCTION</b>
</h2>
<p>
	<b>PSD: </b>HTTP was the process of how to get a resource.<br/>
	HTML is one of the most important resources --&gt; from the concept of documents and papers published until now to share.<br/>
	the beginning of the story was the idea for sharing documents (WWW).<br/>
</p>
<b>Ouestion:</b><br/>
HOW TO DEFINE STRUCTURES OF DOCUMENTS?<br/>
a document includes different parts (e.g. tables, figures and images, links and etc.)
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>BINARY FORMATS : USELESS</b>
</h3>
not readable formats.<br/>
old days: there was nothing<br/>
there was hardly ever graphical popular binary formats: PDF, Doc, ...<br/>
different architectures little-endian and big-endian issue. makes the reading from binary formats much harder.

<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>TEXT format</b>
</h3>
ASCII text<br/>
open and edit and readable and available in every machine. also no little-endian and big-endian issue.<br/><br/>

<b>Question:<br/></b>
how to format the doc though?
(header, footer, paragraph, table, etc.) (e.g. LaTeX, Word, etc.)<br/>
<b>Solution:<br/></b>
MARK UPS!

<!-- ================================================== a heading here ================================================ -->
<b>Hyper Text Markup Language.</b><br/>
<b>The main purpose and goal :</b> defines the structure. we do it with tags. (predefined markups)<br/>
HTML defined with SGML <br/>
not a programming language (no calculation can be done with it, it is a description language.)<br/>
CSS is used for presentation specification, HTML is only responsible for the structure (not the font, color, style, etc.)<br/><br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>Standardizing HTML</b>
</h3>
<b>HTML 1</b> <b>(OOL: </b>(Berners-Lee, 1989), basic, limited)<br/>
<b>HTML 2.0</b> <b>(OOL: </b>(IETF, 1994): tried standardizing and adding some features)<br/>
<b>HTML 3.2</b> (W3C 1996) tried: unifying to a single standard<br/>
<b>HTML 4.0</b> (W3C 1997) tried: map of future.<br/>
<b>XHTML 1.0</b> (W3C 2000)(adding more structures to the html files to limit the formats and templates.) modified to confirm <b>XML</b> standards.<br/>
<b>HTML 5</b> added many more features which was combined with javascript.<br/><br/>
<!-- ================================================== a heading here ================================================ -->
<h2>
	<b>Tags:</b>
</h2>
<b>XHTML = HTML in this lecture, which is a set of elements.</b><br/>
<b>element : </b> a pair of tags(open/close) + content in between (content is <b>OPT</b>)<br/> e.g. &lt;h1&gt;This is header&lt;/h1&gt;<br/>
<br/>
&lt;tagname&gt; : open
&lt;/tagname&gt; : close
&lt;tagname/&gt; : self-closing tag (usuallly for tags that have no content)
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>ATTRIBUTES</b>
</h3>
<b>format : </b><br/>
attname = "value in double quote"<br/>
<b>example : </b><br/>
&lt;tagname attrib1="setting" attrib2="setting" ...&gt;<br/>
...<br/>
&lt;/tagname&gt;<br/><br/>
no att for closing tags.<br/>
some <b>core attribs</b> that most tags have:<br/>
<b>id: </b> a unique identifying thing starting with character, for the element, have different other uses too.<br/>
browsers want to show the content <b>AMAP</b>, they're responsible for rendering html too. so they ignore html's issues <b>AMAP</b>. to give user the best exp. because the user isn't an omniscient to know if the html file of the server has problems.<br/>
<b>class: </b> assign a/some class(es) to the element <br/>
(uniqeness of the id might come with issues later because of browsers mechanisms (in case the id is not unique for example.))<br/>
<b title="for example this thing you're seeing is a title. :)">title: </b> give more info about the element, hover on <b title="for example this thing you're seeing is a title. :)">"title" </b> to see what I mean.<br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>general structure of tags</b>
</h3>
&lt;tag attribute = "attribute value"&gt;content&lt;/tag&gt; <br/>
<b>example : </b><br/>
&lt;h1 class="primary"&gt;Example Heading&lt;/h1&gt;<br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>HTML PROCESSING</b>
</h3>
main discussion.<br/>
different goal of html (not limited to browser rendering) --> 
<b>
	search engines, browsers rendering, pdf, etc.<br/>
</b>
<br/>
<b>search engines : </b> doesn't use your html to render, they just get information and analyze the structure and prioritize and rank the websites (<b>E.G.</b> using "fish farm" phrase in your title has more priorty than a website that just mentioned a "fish farm" in a relevant topic).<br/>
<b>browsers : </b> just render.<br/>
not all tags are rendered. (<b>E.G.</b> &lt;head&gt;) <br/>
some tags are for render but themselves aren't rendered, <b>E.G.</b> &lt;h1&gt; is not rendered itself, the browser just renders the content<br/>
note : each tag has a default render presentation (<b>E.G.</b> headings have bold and bigger fonts.)<br/>
<br/>

<b>LSS:</b> some tags have content but are not rendered, <b>E.G.</b> &lt;head&gt;<br/><br/>
some have contents and are also rendered <br/>

<h4>
	<b>&lt;em&gt;</b> tag
</h4>
<b>E.G.</b> &lt;em&gt;italic, this tag is for emphasis&lt;/em&gt; <br/>
<b>RESULT</b>= <em>italic, this tag is for emphasis</em><br/><br/>

<h4>
	<b>&lt;br&gt; OR &lt;br/&gt;</b> tag
</h4>
some tags don't have content but are rendered. <b>E.G.</b> &lt;br/&gt;<br/>
line&lt;br/&gt;newline <br/>
<b>RESULT</b>= is below!<br/>
line<br/>newline
<h4>
	<b>&lt;h1&gt;</b> tag
</h4>
&lt;h1&gt;the tag and the purpose of the tag won't be rendered.&lt;/h1&gt;<br/>
<b>RESULT</b>= is below! <h1>the tag and the purpose of the tag won't be rendered.</h1> <br/>
<br/>
<!-- ================================================== a heading here ================================================ -->
<h2>
	<b>HTML RENDERING</b>
</h2>
browsers top-bottom, left to right reading to render.<br/><br/>
<b>in-line</b> and <b>block-level</b> elements <br/>
<b>block-level: </b>take one line for each element.(<b>E.G.</b> heading tag)<br/>
<b>in-line: </b>don't take the whole line they are put together in a single line.(<b>E.G.</b> bold tag)<br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>ignored by browsers:</b><br/>
</h3>
&lt;!-- which is comment (like // and /**/ in C) --&gt;<br/>
&lt;not recognizable tags&gt;<br/>
&lt;more than single whitespaces&gt; (spaces + newlines + tabs = single space)<br/>
&lt;br&gt; tag is more useful for poems rather than seperating paragraphs. other purposes such as the latter is done by css rather than html. if you want to fit a paragraph css itself will break as much as it needs, so be aware of what you're doing.<br/>
<b> OQUESTION by A. BOHLOOLI : </b> <b>ANSWER :</b> other reasons and issues: 
1. different sizes in three scales (responsive design which is more discussed in css).
2. makes developement so hard and conflicts are many more.
<br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>
		hello world Example:
	</b>
</h3>
&lt;html&gt;<br/>
 &lt;head&gt;<br/>
&lt;title&gt; shown in the window or tab (used by search engines and browsers)&lt;/title&gt;<br/>
&lt;/head&gt;<br/>
&lt;body&gt;<br/>
shown to the user<br/>
&lt;p&gt; Hello World! &lt;/p&gt;<br/>
&lt;/body&gt;<br/>
&lt;/html&gt;<br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>
		description for example above
	</b>
</h3>
<h4>
	<b>&lt;html&gt;</b> tag
</h4>
every content in html file is between these two tags.(open-close html tag)<br/>
has only two children (Nothing More) : head and body<br/>
<h4>
	<b>&lt;head&gt;</b> tag
</h4>
not shown to the user.<br/>
used by search engines.
page descriptions, page keywords.
<h4>
	<b>&lt;body&gt;</b> tag
</h4>
shown to the user.<br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	NESTED TAGS
</h3>
a tree relation between the tags which is really <b>IMP</b><br/>
root -&gt; head&body --&gt; (sth CHILD FOR HEAD)&(sth CHILD FOR BODY) etc.<br/>
<br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>SPECIAL CHARACTERS</b><br/>
</h3>
special characters as a symbol encoded in html can be used.<br/>
parsing issues characters.<br/>
although today these can be rendered normally, it is best to still the codes rather than the character itself, like below:<br/>
<!-- table to be added here. -->
<b>&lt;</b> ::: &amp;lt; ::: ASCII : &amp#60;<br/>
<b>&gt;</b> ::: &amp;gt; ::: ASCII : &amp#62;<br/>
<b>&amp;</b> ::: &amp;amp; ::: ASCII : &amp#38;<br/>
<b>'&nbsp; this was a forced whitespace'</b> ::: &amp;nbsp; ::: ASCII : &amp#160;<br/>
or characters which are not accessible from keyboard (E.G. UTF-8 characters) : <br/>
<b>&copy;</b> ::: &amp;copy; ::: ASCII : &amp#160;<br/>
<b>&lambda;</b> ::: &amp;lambda; ::: ASCII : &amp#955;<br/>
but nowadays!!! --&gt; utf-8 characters are allowed.<br/>
<h4>
	other characters by my interest:<br/>
</h4>
<b>
&Omega;, &omega;, &Theta;, &theta;, &Alpha;, &alpha;, &Beta;, &beta;, &Gamma;, &gamma;, &Zeta;, &zeta;, &Sigma;, &sigma;, &Phi;, &phi;<br/><br/>
こんなやり過ぎは申し絵分けございませんでした。&#128513;&#128517;😅
</b><br/>
<br/>
<!-- ================================================== a heading here ================================================ -->
<h2>
	<b>XHTML<br/></b>
</h2>
HTML is a subset of <b>SGML</b> = Standard General Markup Language.<br/>
XHTML application of <b>XML</b> = Extensible Markup Language.<br/>
<br/>
XML <b>DFW</b> SGML<br/>
XML is more restricted than SGML<br/>
XHTML is more restricted than HTML<br/>
XHTML is more well-defined.<br/>
<br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	<b>XHTML RESTRICTIONS:</b>
</h3>
<h4>
	forced self-closing.
</h4>
&lt;br/&gt; (forced self-closing)(endings are mandatory so there should be no open tag without content or end tag)<br/>
<h4>
	no tag overlap
</h4>
<b>E.G.</b> <br/>
&lt;strong&gt;&lt;em&gt;test&lt;/strong&gt;&lt;/em&gt;<br/>
<b>because</b> the child or parent aren't determinant<br/>
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
<br/>
<h4>
	removing some tags
</h4>
<b>&lt;big&gt;</b> tag was to show the font size is big.<br/>
<b>E.G.</b> = &lt;big&gt;this&lt;/big&gt; is in big font size.<br/>
<b>RESULT</b> = <big>this</big> is in big font size.<br/><br/>

<b>&lt;center&gt;</b> tag which was to put the content in the center of page.<br/>
<b>E.G.</b> = &lt;center&gt;put it in center&lt;/center&gt;<br/>
<b>RESULT</b> = <center>put it in center</center>
<br/>
these are implemented by <b>CSS</b> so it is not needed anymore.<br/><br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	Bigger Example of HTML:
</h3>
&lt;!DOCTYPE html&gt;<br/>
&lt;html lang="en"&gt;<br/>
&lt;head&gt;<br/>
&lt;meta charset="utf-8"&gt;<br/>
&lt;title&gt;
My test page
&lt;/title&gt;<br/>
&lt;/head&gt;<br/>
&lt;body&gt;<br/>
&lt;img src="pathname..." alt="My example image"&gt;<br/>
&lt;/body&gt;<br/>
&lt;/html&gt;<br/>
<!-- ================================================== a heading here ================================================ -->
<h3>
	discription for above example:
</h3>
<h4>
	&lt;!DOCTYPE html&gt; tag
</h4>
it had meaning in the past but it is nothing special anymore.<br/>
ATT: <b>lang</b> telling the language of the website. if your document is multi-lang you have to change the attrbute.<br/>
<h4>
	&lt;title&gt; tag
</h4>
it's the titr of the website.<br/>
<h4>
	&lt;meta&gt; tag
</h4>
meta data tag for the website.
ATT: <b>charset</b> telling that we are using a "utf-8"encoding in our website.<br/>
<h4>
	&lt;img&gt; tag
</h4>
loading an image in the body.<br/>
ATT: <b>src</b> is the source/path of the file.<br/>
<h2>
	&lt;!DOCTYPE HTML&gt;
</h2>
for error checking purposes of html and announcing the html version and etc. and it would check the rules that should be asserted.<br/>
<b>in todays : </b> for after versions of xhtml (html 5) everyone is using html 5 so we don't really need this one anymore.
<br/>
<h2>
	HTML ELEMENTS
</h2>
<h4>
	Main root (html tag)<br/> 
</h4>
<h4>
	Document metadata (things we see in head tag)<br/> 
</h4>
<h4>
	<b>these belows are used in body tag:</b>
<h4>
<h4>
	Sectioning root (<b>I.E.</b> body tag)
</h4>
each html doc can have only <b>one</b> body<br/><br/>
<h4>
	Content sectioning<br/>
</h4>
sectioning
<h4>
	Text content<br/>	
</h4>
<h4>
	Inline text semantics<br/>	
</h4>
<h4>
	Image and multimedia<br/>
</h4>
<h4>
	Embedded content<br/>
</h4>
<h4>
	Scripting<br/>	
</h4>


&lt;section&gt;<br/>
&lt;footer&gt; (semantical element)<br/>
&lt;header&gt; (semantical element)<br/>
&lt;nav&gt; (semantical element)<br/>
&lt;pre&gt;<br/>
<br/>
lists:<br/>
&lt;ol&gt; ordered lists<br/>
&lt;ul&gt; unordered lists (bullet render <b>BYD</b>)<br/>
&lt;li&gt; the elements of the list. (list item)<br/>
&lt;dt&gt;<br/>
&lt;dd&gt;<br/>
&lt;div&gt; (content division, <b>DFW</b> section)<br/>

<strong>STRONG</strong> <b>BOLD</b>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
</body>
</html>