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

The manipulation of text is central to the operation of computer
systems and so a huge number of text editors are available. One of
these is *GNU Emacs*. Emacs is a powerful text editor characterised by
its flexibility. The manual describes it as &ldquo;the extensible,
customisable, self-documenting, real-time display editor&rdquo;. Emacs is
Free Software<sup><a id="fnr.2" class="footref" href="#fn.2">2</a></sup>, meaning the user has the four freedoms: the
freedom to *run* the program, to *study* the source code, to
*redistribute* copies and to *improve* the program. It is therefore
not tied to a single company, computer architecture or operating
system. Emacs supports most Unix-like systems (GNU/Linux, the BSDs
etc), Microsoft Windows and Mac OS X and it supports the editing of
text written in many languages. Development of the first Emacs began
in the 1970s and continues actively as of 2016.

Primarily created for computer programmers, Emacs is perceived to have
a steep learning curve. Emacs has over 2,000 built-in commands and
allows the user to combine these commands into macros to automate
work. This makes Emacs incredibly adaptable to the users workflow.
However Emacs can be a powerful tool in the hands of a writer equipped
with just a handful of basic commands. This guide aims to show that
writing a novel or a dissertation in Emacs can be a simple and
pleasurable experience.

### Org Markup (and Emacs Org-mode)<a id="orgheadline3"></a>

Having discussed the weaknesses of *what you see is what you get*, we
now examine *what you see is what you mean*<sup><a id="fnr.3" class="footref" href="#fn.3">3</a></sup>. In this model the
writer marks text as the title of the document, the name of a section,
or the name of an author. This allows one element, such as section
headings, to be rendered as large bold text in one output format, but
as red centre justified text in another without further
intervention. This is the key advantage of markup languages:
separation of the structure and appearance of a document. In a markup
language, the user writes the document in a structured way, marking
the content according to its significance in the document. The writer
can outline, write and edit the text largely without concern
for the presentation, leaving the final appearance to a separate
process, the export system.

*Org* is a powerful yet simple plain-text markup language, which allows
the writer to describe complex documents easily. One of the most
elegant markup languages, Org is more powerful than simple Markdown,
yet more readable and accessible than LaTeX or the XML based Docbook
or DITA. Org can be used to produce quite complex documents. This
guide was itself written entirely in Org. Furthermore, Org is designed
for project planning, running an agenda and taking notes and so can be
incredibly useful to a writer for far more than simply writing.

*Org-mode*, a major mode in Emacs, provides front end tools to outline,
write and edit an Org document and back end export functions to
produce output for high quality typesetting. Org-mode export uses
LaTeX to produce professionally typeset PDF output. Org-mode can also
export to HTML for web publishing, to Docbook or simply to plain ASCII
text. In this way, Org-mode provides a system for exporting structured
content to generate the document&rsquo;s final format leaving the writer
free to… *write*.

# Emacs<a id="orgheadline30"></a>

## Getting Started<a id="orgheadline5"></a>

This chapter is an introduction to the basics of editing text in
Emacs for the novice. It also serves as a handy reference, with tables 
summarising the commands covered. To start, a look at installing and
running Emacs.

Emacs installation on GNU/Linux is simple<sup><a id="fnr.4" class="footref" href="#fn.4">4</a></sup>. At a terminal, enter
`sudo apt-get install emacs`. Emacs can be run in the terminal or the
GUI, the graphical user interface. The GUI offers menus, which can be
helpful to a beginner, and also integrates with the system clipboard.
The display can be customised more extensively that can the
terminal version. The GUI version runs from the system menu or
launcher and when the `emacs` command is entered in the
terminal.  To use the terminal version, type `emacs -nw` at the terminal
prompt.

## Vocabulary<a id="orgheadline6"></a>

Emacs uses different vocabulary than might be expected.  An early
mention of some of the non-standard terms is helpful when reading
this guide and other Emacs documentation and tutorials.

To *kill* is to remove text. Usually called cut in other applications.
The *kill ring* is the Emacs clipboard. To *yank* is to insert or
paste previously removed text. An open file resides in a memory
*buffer*. When saved the buffer is written to that file. The *point*
is the cursor position. Selected text, between the *mark* and the
point, is called the *region*. The function of *filling* is similar to
word-wrap: to format a paragraph of text, Emacs inserts a return
character at the end of every line.

An Emacs *frame* is what any other program would call a window. A
frame can be merely another view of the same document or show
different documents. Finally, an Emacs *window* divides the Emacs
frame into sections, each of which can view a different buffer or
different parts of the same buffer. The following sections will cover
these terms and other Emacs basics, starting with how to enter 
commands and key sequences.

## Commands and Modifiers<a id="orgheadline8"></a>

Emacs is driven by commands and key sequences. This can take time to
adjust to for a user used to menus and icons, however once mastered it
is far more efficient. Commands are usually performed by using key
sequences. For example `C-x C-s` which runs the command named
`save-buffer`. This command can also be called by name with `M-x
save-buffer`. These commands are entered using modifiers. This section
details what these modifiers are, how to read the key sequences and
how to perform them.

There are two main modifiers in Emacs commands. These keys are pressed
along with another key. First is `C-` which is the **Control** or **ctrl**
key. In Emacs documentation `C-x` means to press and hold control,
press `x` and release both keys. The longer command, `C-x C-s` means
`C-x` followed by `C-s`. Commonly used commands tend to begin with
`C-x` whilst many others that are specific to particular modes start
with `C-c`. Another common combination is `C-h` for help. The other
modifier is `M-` which means **Meta** which is on modern keyboards is
the **Alt** key. The command `M-x save-buffer` means press `Alt` and
`x`, release and then type `save-buffer`. Tab complete is available to
help with entering the command name and will prompt if more characters
are needed to uniquely identify a command. Sometimes `ESC` is
used instead of `M-` (usually when working remotely) here `ESC` is
pressed before the other key, so `M-a` becomes `ESC a`. The backspace
key is written `DEL` (not to be confused with the key marked Delete)
and `RET` means the **Enter** key.

The commands are displayed below the mode line at the bottom of the
frame as they are entered. This area is called the *minibuffer*.
Commands appear here as they are entered. Emacs commands can be tricky
to get used to for a beginner. Some of the most important commands to
learn when starting with Emacs are the commands which cancel a
command, allow commands to be undone and windows to be closed, and the
command to quit Emacs. If a mistake is made when entering a command,
use `C-g` or three presses of `ESC` to cancel it. This will also stop
a running command if Emacs appears to have frozen. To revert a
completed command use `C-/` or `C-x u` to perform undo (explained in
more detail in Section [2.5](#orgheadline7)). If a command has opened a new window
return to a single window with `C-x 1` which closes all other windows.
Close a focused window with `C-x 0`. If the wrong window is closed,
switch back to the desired buffer using `C-x left` and `C-x right`. To
return the buffer to the point at which is was last saved use
`revert-buffer`. Finally, the command `C-x C-c` will quit Emacs and
query if changes should be saved. Whilst learning these basic
commands, remember they are also available from the Emacs menu.
Additionally, buffers can be switched using the mouse on the buffer
name, and windows closed using the empty area of the modeline.

Another difficulty with commands stems from the design of many modern
keyboards which are not ideal for the purpose. Using your little
fingers to press ctrl can lead to the infamous &ldquo;Emacs pinky&rdquo;<sup><a id="fnr.5" class="footref" href="#fn.5">5</a></sup>.
One useful trick is to use the pad of the little finger of the
opposite hand to press the ctrl key. However, if your control keys are
not in the corners or are otherwise awkwardly positioned, as on many
laptop keyboards, it may be desirable to remap Caps Lock to act as
ctrl. To do this on a GNU/Linux system, in the terminal enter
`setxkbmap -option ctrl:nocaps`. To set both shift keys together to
act as a replacement for Caps Lock use `setxkbmap -option
shift:both_capslock`. To unset all changes use `setxkbmap -option`

## Help Commands<a id="orgheadline9"></a>

Emacs is self-documenting and extensive help is available on the
commands. Get help on a key press with `C-h k <command>`, for example
`C-h k C-x C-c`. Or search for help with `C-h a <string>`, for example
`C-h a find file`. To list all the key sequences type `C-h b` and to
view all the help commands use `C-h ?`. Emacs has its own manual,
accessed with `C-h r` and also available online<sup><a id="fnr.6" class="footref" href="#fn.6">6</a></sup>, and an
interactive tutorial which is started with `C-h t`. Both are also
available from the splash screen. Table [1](#orgtable1) summarises
these help commands and the commands mentioned in the previous section
which help cancel a command and undo mistakes.

If the name of the desired command is known, or even partially known,
then Emacs can help here too. For example, if you want to centre a
line of text but do not know the command name or the key
sequence. Type `M-x center TAB TAB`. Emacs will make some
suggestions. Keep typing so you have `M-x center-line` and the line is
centred. Emacs will also tell you in the minibuffer that the key
sequence required is `M-o M-s`.

With the command names always available, and the help commands on
hand, it can be seen that there is no need to learn all the short
commands. Each user will know a different set of commands, and some
learn only the basics, but knowledge of a selection of frequently used
key sequences makes using Emacs much more efficient.

## Undo<a id="orgheadline7"></a>

The undo system in Emacs is different to that in many other programs.
Emacs can undo not just the previous command, but a long sequence of
commands even back through saves. Additionally, there is no separate
concept of undo and redo. There is a single undo command called with
`C-x U`, or more conveniently with `C-/`. Redo is simply &ldquo;undoing an
undo&rdquo;. Once understood, it may be seen that this allows Emacs to cycle
to all states in the history. In other programs if you undo and type a
character the undone steps may be lost.

When performing a sequence of undo commands any other command breaks
the sequence. The undo commands performed are then placed into the
undo record as a set of changes. To re-apply changes that have been
undone, type any command that silently breaks the undo sequence, such
as a cursor move or `C-f`, then type `C-/` to undo the undone steps.

## Files and Buffers<a id="orgheadline10"></a>

Once a file from disk is loaded into Emacs, it is referred to as a
buffer. If the file requested does not exist Emacs will create a new
file. So to create a new Org file hit `C-x C-f RET newfile.org`.
Inserting a file at the cursor is performed with `C-x i`. This can be
useful for inserting template material.

Emacs does not modify the file on disk until told to do so. For
example, by entering `C-x C-s` to save the buffer. However, it has two
useful save features set by default. When saving, Emacs also saves the
previous version of the file. If the file is named `foo`, the backup
will be called `foo~`. Emacs also has auto-save by default. The
auto-save file for a file named `foo` is `#foo#`. If Emacs, or the
system, were to crash before edits were saved, unsaved edits may be
recovered from this file. Auto-saving occurs every 300 characters.

<table id="orgtable1" border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
<caption class="t-above"><span class="table-number">Table 1:</span> Basic commands</caption>

<colgroup>
<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">Action</th>
<th scope="col" class="org-left">Key sequence</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">Cancel</td>
<td class="org-left">`C-g` or `ESC ESC ESC`</td>
</tr>


<tr>
<td class="org-left">Undo</td>
<td class="org-left">`C-/` or `C-x u`</td>
</tr>


<tr>
<td class="org-left">Close other windows</td>
<td class="org-left">`C-x 1`</td>
</tr>


<tr>
<td class="org-left">Close selected window</td>
<td class="org-left">`C-x 0`</td>
</tr>


<tr>
<td class="org-left">Switch buffers</td>
<td class="org-left">`C-x left/right`</td>
</tr>


<tr>
<td class="org-left">Revert buffer</td>
<td class="org-left">`M-x revert-buffer`</td>
</tr>


<tr>
<td class="org-left">Quit emacs</td>
<td class="org-left">`C-x C-c`</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="org-left">Find (open) a file</td>
<td class="org-left">`C-x C-f`</td>
</tr>


<tr>
<td class="org-left">Save</td>
<td class="org-left">`C-x C-s`</td>
</tr>


<tr>
<td class="org-left">Save as</td>
<td class="org-left">`C-x C-w`</td>
</tr>


<tr>
<td class="org-left">Insert file into current</td>
<td class="org-left">`C-x i`</td>
</tr>
</tbody>

<tbody>
<tr>
<td class="org-left">Help: help commands</td>
<td class="org-left">`C-h ?`</td>
</tr>


<tr>
<td class="org-left">Help: list key sequences</td>
<td class="org-left">`C-h b`</td>
</tr>


<tr>
<td class="org-left">Help: describe</td>
<td class="org-left">`C-h k <key sequence>`</td>
</tr>


<tr>
<td class="org-left">Help: apropos</td>
<td class="org-left">`C-h a <string>`</td>
</tr>


<tr>
<td class="org-left">Help: tutorial</td>
<td class="org-left">`C-h t`</td>
</tr>
</tbody>
</table>

## The Mode Line, Modes and Configuration<a id="orgheadline12"></a>

The mode line is at the bottom of the Emacs window just above the
minibuffer. It shows summary information about the buffer, including
its modification status, its name, the position in the buffer and
current modes. The status of the buffer is shown to the left. Two
dashes (`--`) indicate the buffer is not modified since the last save.
Two asterisks (`**`) show the buffer has been modified since the last
save. For read-only files, `%%` and `%*` indicate unmodified and 
modified buffers respectively. 
