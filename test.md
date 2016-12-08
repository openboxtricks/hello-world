<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#orgheadline4">1. Introduction</a></li>
<li><a href="#orgheadline30">2. Emacs</a>
<ul>
<li><a href="#orgheadline5">2.1. Getting Started</a></li>
<li><a href="#orgheadline6">2.2. Vocabulary</a></li>
<li><a href="#orgheadline8">2.3. Commands and Modifiers</a></li>
<li><a href="#orgheadline9">2.4. Help Commands</a></li>
<li><a href="#orgheadline7">2.5. Undo</a></li>
<li><a href="#orgheadline10">2.6. Files and Buffers</a></li>
<li><a href="#orgheadline12">2.7. The Mode Line, Modes and Configuration</a></li>
<li><a href="#orgheadline13">2.8. Navigation</a></li>
<li><a href="#orgheadline14">2.9. Searching</a></li>
<li><a href="#orgheadline15">2.10. The Region &#x2013; Selecting Text</a></li>
<li><a href="#orgheadline16">2.11. Kill and Yank &#x2013; Cut and Paste</a></li>
<li><a href="#orgheadline17">2.12. Buffers, Windows and Frames</a></li>
<li><a href="#orgheadline22">2.13. Formatting text</a></li>
<li><a href="#orgheadline27">2.14. Other Writing Tools</a></li>
<li><a href="#orgheadline29">2.15. Learning More</a></li>
</ul>
</li>
<li><a href="#orgheadline47">3. Org</a>
<ul>
<li><a href="#orgheadline31">3.1. A First Look at Org</a></li>
<li><a href="#orgheadline32">3.2. Getting Started</a></li>
<li><a href="#orgheadline34">3.3. Headlines</a></li>
<li><a href="#orgheadline36">3.4. Paragraphs</a></li>
<li><a href="#orgheadline37">3.5. Structure Navigation</a></li>
<li><a href="#orgheadline38">3.6. Plain Lists</a></li>
<li><a href="#orgheadline39">3.7. Formatting</a></li>
<li><a href="#orgheadline35">3.8. Special Blocks</a></li>
<li><a href="#orgheadline42">3.9. Hyperlinks</a></li>
<li><a href="#orgheadline43">3.10. Footnote Markers</a></li>
<li><a href="#orgheadline40">3.11. Tables</a></li>
<li><a href="#orgheadline41">3.12. Figures</a></li>
<li><a href="#orgheadline44">3.13. Document Metadata</a></li>
<li><a href="#orgheadline45">3.14. Macros</a></li>
<li><a href="#orgheadline46">3.15. Comments</a></li>
</ul>
</li>
<li><a href="#orgheadline54">4. Export</a>
<ul>
<li><a href="#orgheadline48">4.1. Write Once and Export Many</a></li>
<li><a href="#orgheadline49">4.2. Export Commands</a></li>
<li><a href="#orgheadline51">4.3. Export Settings</a></li>
<li><a href="#orgheadline52">4.4. Inline LaTeX</a></li>
<li><a href="#orgheadline53">4.5. HTML Export</a></li>
</ul>
</li>
<li><a href="#orgheadline11">5. Customisation</a>
<ul>
<li><a href="#orgheadline59">5.1. Emacs Customisation</a></li>
<li><a href="#orgheadline33">5.2. Org Customisation</a></li>
<li><a href="#orgheadline50">5.3. Export Customisation</a></li>
</ul>
</li>
<li><a href="#orgheadline28">6. Resources</a></li>
<li><a href="#orgheadline66">7. Acknowledgements</a></li>
<li><a href="#orgheadline79">8. GNU Free Documentation License</a></li>
</ul>
</div>
</div>

<div class="abstract">
 This is a guide to using the GNU Emacs text editor and Org markup to
produce beautiful typeset documents. This guide covers the basic
knowledge needed from the starting point as an Emacs and Org novice.  
  
  
  
Copyright © 2016 Dr Jason Beard.  
  
Permission is granted to &ldquo;copy&rdquo;, distribute and/or modify this document
under the terms of the GNU Free Documentation License, Version 1.3 or
any later version published by the Free Software Foundation; with no
Invariant Sections, no Front-Cover Texts, and no Back-Cover Texts. A
copy of the license is included in the section entitled &ldquo;GNU Free
Documentation License&rdquo;.

</div>

# Introduction<a id="orgheadline4"></a>

### A Word On Word Processors<a id="orgheadline1"></a>

Most modern word processors use a *what you see is what you
get*<sup><a id="fnr.1" class="footref" href="#fn.1">1</a></sup> display. This makes it easy to write short documents
quickly and easily. However, long, structured documents can be
difficult to plan, write and edit in such an environment. Word
processors often involve the writer with unnecessary details and the
display can be distracting. The writer should not worry about things
such as page breaks or text re-flowing and figures being moved around
upon edits. These matters should be dealt with without interrupting
the writing process rather than as part of it. Therefore word
processors are simply not the right tool for the job for many kinds of
documents. Word processors, as a rule, focus too much on the
appearance of a document, too little on the structure, and usually
distract from what should be the main task: *writing*.

### GNU Emacs<a id="orgheadline2"></a>

The writer of documents such as manuals or novels may be better served
by writing in plain text in a text editor. Plain text is less
distracting than any other format. It can be easier on the eye, with a
font and colour scheme chosen for the screen rather than for the
page. However the advantages go far beyond the visual. Plain text is
superior when it comes to ensuring future access to documents. A text
file will be readable in twenty years time since the format is an open
standard. A proprietary word processor file may be a different
matter. Plain text also assures compatibility between systems. Text
files may be edited on all computers, even the most ancient of
hardware, and on all operating systems.
