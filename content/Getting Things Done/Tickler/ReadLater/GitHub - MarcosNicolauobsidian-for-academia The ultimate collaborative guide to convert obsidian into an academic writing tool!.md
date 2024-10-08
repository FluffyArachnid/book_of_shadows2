[[ReadItLater]] [[Article]]

# [GitHub - MarcosNicolau/obsidian-for-academia: The ultimate collaborative guide to convert obsidian into an academic writing tool!](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#reference-manager-integration)

## Obsidian for Academia

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#obsidian-for-academia)

This repository attempts to create a collaborative documentation explaining all the forms to convert obsidian into an academic writing tool.

There is no single or definite form of achieving this. So here you will find all the possible setups with their benefits and drawbacks.

To see this workflow in action, watch this [video](https://youtu.be/ZKQEgf2ktWE).

## Table of Contents

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#table-of-contents)

-   [How to setup](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#how-to-setup)
    -   [Reference Manager integration](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#reference-manager-integration)
        -   [Integrating Zotero](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#integrating-zotero)
            -   [Importing your annotations](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#importing-your-annotations)
        -   [Integrating another Reference manager](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#integrating-another-reference-manager)
            -   [Importing your annotations](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#importing-your-annotations-1)
    -   [Citations](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#citations)
        -   [Zotero Integration](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#zotero-integration)
        -   [Pandoc](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#pandoc)
    -   [Creating bibliography](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#creating-bibliography)
        -   [Zotero Integration](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#zotero-integration-1)
        -   [Pandoc Reference List](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#pandoc-reference-list)
        -   [Pandoc](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#pandoc-1)
    -   [Exporting](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#exporting)
        -   [Native](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#native)
            -   [Caveats](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#caveats)
            -   [Styling](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#styling)
        -   [Pandoc](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#pandoc-2)
            -   [Caveats](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#caveats-1)
            -   [Exporting](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#exporting-1)
            -   [Other formats](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#other-formats)
            -   [Internal links](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#internal-links)
    -   [Other](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#other)
        -   [Combine notes](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#combine-notes)
        -   [Improving Math writing](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#improving-math-writing)
            -   [Numerating equations](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#numerating-equations)
            -   [Aligning equations](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#aligning-equations)
        -   [Page breaks](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#page-breaks)
-   [Contributing](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#contributing)
-   [Reference](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#reference)

## How to setup

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#how-to-setup)

### Reference Manager integration

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#reference-manager-integration)

For the reference manager software, there are two alternatives. Either use [Zotero](https://zotero.org/) or any other of your preference and use the [obsidian-citations](https://github.com/hans/obsidian-citation-plugin) plugin which uses the .bib file.

Zotero is really well integrated into obsidian, so preferably you should go with that.

#### Integrating Zotero

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#integrating-zotero)

Here is what you need to install:

-   [Zotero 6 and Zotero Browser Connector](https://www.zotero.org/download/)
-   [Better Bibtex for Zotero](https://retorque.re/zotero-better-bibtex/) - Zotero plugin
-   [Zotero Integration](https://github.com/mgmeyers/obsidian-zotero-integration) - Obsidian plugin

Note: We are skipping the installation of Zotero and its plugins here, as well as the basics of Zotero, since these instructions are widely available on the web.

##### Importing your annotations

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#importing-your-annotations)

We'll use Zotero Integration to create notes that contain the full metadata, link to Zotero, as well as PDF annotations and notes.

For that, the plugin requires a template. We provide a standard one [here](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/templates/zotero). You can extend it to your needs following their [docs](https://github.com/mgmeyers/obsidian-zotero-integration/blob/main/docs/Templating.md).

The setup will look like:

[![1](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/1.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/1.png)

Note: It is important that you call the citations as @{{citekeys}}, you'll see why in [citations](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#Citations).

After that, you would create a note by entering the command "Zotero Integration: Create Note" in the command palette.

[![2](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/2.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/2.png)

And this is how your notes will look like:

[![17](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/17.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/17.png)

#### Integrating another Reference manager

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#integrating-another-reference-manager)

As explained before you need to install the following:

-   [Obsidian Citations](https://github.com/hans/obsidian-citation-plugin) - Obsidian plugin

And then you have to export your library in .bib format. Then, you tell the plugin to use that file in the configuration.

##### Importing your annotations

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#importing-your-annotations-1)

For obvious reasons, this plugin lacks the features of the Zotero-Integration. So importing your notes won't be as rich as with Zotero. Anyways, here you have a nice template:

\---
title: { { title } }
authors: { { authorString } }
year: { { year } }
\---

\# {{title}}

\## {{authorString}}

\## Abstract

{{abstract}}

\## Note

{{note}}

There are probably other plugins that can improve this workflow, if you know one, don't hesitate to open a PR and improve this section!

### Citations

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#citations)

Citations are pretty straightforward. You have two options, do it manually through the Zotero Integration or by setting up pandoc. The latter is the preferred one since it allows to change between different citation styles easily and automatically.

Regardless of what you choose, we want to create the citation and at the same time link it to the note that has its annotations (in case we have created it). This way, we don't lose the graph view and some other features that Obsidian offers.

#### Zotero Integration

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#zotero-integration)

Citations can be added using the Zotero Integration plugin by configuring a certain citation style and then selecting that option in the command palette.

For example:

[![1](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/1.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/1.png)

[![3](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/3.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/3.png)

And then you could also connect the citation to its respective note:

\[CITATION\_CREATED\_BY\_ZOTERO\_INTEGRATION\](/link\_to\_annotation)

#### Pandoc

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#pandoc)

You'll need to install:

-   [Pandoc](https://pandoc.orgl/)
-   [Pandoc Reference List](https://github.com/mgmeyers/obsidian-pandoc-reference-list) - Obsidian plugin

Note: If you want to export your documents using pandoc, then you must use this form. Since pandoc will automatically create the citations for you.

Then you need to tell the plugin where the .bib file exported by your reference manager is located in the configuration.

Once you have configurated everything, you would cite following the pandoc format: `[@CITE_KEY]`. Though, you should use the wikilink format `[@CITE_KEY](@CITE_KEY)`, this way you would be citing the source as well as connecting the note with the annotations (in case you created one). For this reason, you must import your annotations following the format `@{{citekey}}`.

By the way, you should activate the option "*Show citekey suggestions*" in the plugin to have auto-completion. Furthermore, you can set the Zotero Integration to cite in the pandoc style:

[![4](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/4.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/4.png)

The great thing about this plugin is that it keeps all citations made through the note:

[![5](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/5.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/5.png)

To view it, enter the command *"Pandoc Reference List: Show reference list"* in the command palette.

### Creating bibliography

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#creating-bibliography)

To create a bibliography, you have three options:

-   Manually doing it yourself with Zotero Integration
-   Use the Pandoc Reference List
-   Let pandoc create it for you automatically.

Let's see:

#### Zotero Integration

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#zotero-integration-1)

Create a configuration for citating bibliography on your desired style in the plugin settings. For example:

[![6](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/6.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/6.png)

And then you introduce it by entering the command *"Zotero Integration: Add Bibliography APA"* in the command palette.

#### Pandoc Reference List

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#pandoc-reference-list)

You have to open the reference list and then press the copy button.

[![9](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/9.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/9.png)

Then you would insert it wherever you want. If you change the citation style in the plugin settings or add new citations, then you have to do this again.

It is still kinda manual but it is still much faster than the previous method. This is the preferred method if you are not exporting the note with pandoc.

#### Pandoc

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#pandoc-1)

You can use this method if and only if you will **export the note using pandoc**. You need to provide the flags `--citeproc --bibliography --csl` when exporting. Refer to the [Exporting section](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#exporting) where this is explained.

This way, your bibliography will be automatically inserted at the bottom when exporting the note.

### Exporting

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#exporting)

You should know that there are two ways *\-maybe there are other forms, but these are the most popular among the community-* of exporting your documents: Through **Pandoc** or using the Obsidian **native** functions. If you choose the former, you should know that you must forfeit many obsidian features explained in [here](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#caveats-1).

#### Native

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#native)

##### Caveats

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#caveats)

There are two caveats to this approach:

1.  Internal links don't work (this is [quite a requested feature in the obsidian community](https://forum.obsidian.md/t/pdf-export-make-links-within-same-document-functional/16384), maybe we'll get it soon).
2.  Can't add a header and a footer.

##### Styling

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#styling)

We want to make the document look as closely as possible to latex, which is the standard when doing academic documents. For that, add this [css snippet](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/.obsidian/snippets/academic.css) and activate it. Check the [official guide](https://help.obsidian.md/Extending+Obsidian/CSS+snippets) for help.

Then you need to provide the property `cssclass: academic` or

In the note, you want to export. This will activate the academic style when exporting the note.

For example:

| Source | Exported |
| --- | --- |
| [![14](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/14.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/14.png) | [![10](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/10.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/10.png) |

Additionally, you can also provide the class `twocolumn` so that it renders the document in two columns. This way, your properties should look like:

cssclasess:
  - academic
  - twocolumn

See the style in action:

[![11](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/11.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/11.png)

Feel free to extend this snippet to suit your needs better and send a PR if you think it can be improved(surely you do).

#### Pandoc

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#pandoc-2)

##### Caveats

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#caveats-1)

If you choose to export using pandoc then you must forfeit features like DataView tables, callouts, and Templater. Any feature that relies on markdown processing. Though you can find workarounds through plugins, lua scripts, etc we won't cover them here.

##### Exporting

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#exporting-1)

You need to install:

-   [Pandoc](https://pandoc.org/installing.html)
-   [A Latex engine](https://www.tug.org/texlive/)
-   [Obsidian Pandoc](https://github.com/OliverBalfour/obsidian-pandoc) (optional) - Obsidian plugin
-   [Link Converter](https://github.com/ozntel/obsidian-link-converter) (optional) - Obsidian Plugin
-   [Templater](https://github.com/SilentVoid13/Templater) - Obsidian Plugin

If you've been reading the readme, you should know that if you are using pandoc export, then the citations and the bibliography are created by this tool.

To export the document you can do it through the Obsidian Pandoc plugin or via the CLI. They actually are the same thing, only that the former is a wrapper of the latter.

We provide you with a [template](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/templates/academic.md) that includes all the properties and metadata commonly used. They are all read by pandoc when exporting. You can see what each one does [here](https://pandoc.org/MANUAL.htmls).

Note: You could create a header file which you would then provide to pandoc with the `-H` flag, instead of declaring everything in the note properties. See more [here](https://pandoc.org/MANUAL.html#general-writer-options)

Then when you want to create a note that you will later export with pandoc you should enter the command "*Templater: Create new note from template*" and select the one for pandoc.

Note: We are not using the native template functions because it fails to insert the template.

As said before Wikilinks don't work with pandoc . Still, you can use them and, before exporting the note, you can run the command "*Obsidian Link Converter: Active file: Links to Markdown*" which will convert all the links in the wikilink format to the general markdown format.

Finally, you need to provide the `--citeproc` flag.

If you are using the Obsidian Pandoc Plugin, then you need to configure the command arguments:

[![13](https://github.com/MarcosNicolau/obsidian-for-academia/raw/main/assets/13.png)](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/assets/13.png)

And to export enter the command "*Pandoc Plugin: Export as PDF*".

If you want to go with the CLI style, then enter

pandoc <PATH\_TO\_NOTE\>.md -o ./output.pdf --from=markdown+wikilinks\_title\_after\_pipe --citeproc

Note: we are not passing the common flags you will see in other guides because they are all passed through the document properties. For example, you could provide the bibliography, and csl flags in the extra arguments field in the Obsidian Pandoc settings.

To see an example see

| Source | Exported |
| --- | --- |
| [markdown](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/example-note.md) | [pdf](https://github.com/MarcosNicolau/obsidian-for-academia/blob/main/example-note.pdf) |

##### Other formats

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#other-formats)

The great thing about pandoc is that not only can you export your documents as PDFs but to any other format you can think of, such as docx, epub, html, and many more. Check their [docs](https://hackage.haskell.org/package/pandoc) to see how.

##### Internal links

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#internal-links)

The great thing about pandoc is that you can make internal links work. See more [here](https://pandoc.org/chunkedhtml-demo/7.2-headings-and-sections.html) and [here](https://pandoc.org/chunkedhtml-demo/8.3-headings.html#heading-identifiers).

But basically, pandoc assigns an identifier to every header which is its name in undercaps. So to link to a header you would do `[click here](#header-name-in-undercaps-and-separated-by-hyphens)`. The problem is that it might not work with Obsidian out of the box.

You can assign identifiers to your headers by adding {#id} next to it. See below.

\# A header {#my\_id}

...

\### Later in the note

\[see here\](#my\_id)

Though, it won't work with Obsidian.

### Other

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#other)

#### Combine notes

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#combine-notes)

If you are writing a long document, chances are you are writing each section in a separate file. To merge all the content into a single file when exporting all the files you can do it through pandoc or obsidian.

**pandoc**

`pandoc ./note_1.md ./note_2.md ... ./note_n.md -o output.pdf`

or if everything is inside a folder:

`pandoc ./folder/*.md -o output.pdf`

**obsidian**

With obsidian, you just simply call all the notes into one

!\[note\_1\](note\_1)
!\[note\_2\](note\_2)
!\[note\_3\](note\_3)
.
.
.
!\[note\_n\](note\_n)

#### Improving Math writing

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#improving-math-writing)

##### Numerating equations

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#numerating-equations)

Many styles, such as the IEEE Style, that requires the author numerates their "math blocks" and refers to them as equations. To do this in Obsidian all you have to do is add `\tag{n}` to your math block where `n` is the figure/equation number.

An example would be: `$\tag{4} 1+1=2$` [![image](https://private-user-images.githubusercontent.com/95967108/326645100-d733c915-df7f-4495-b0ad-e1996dc7020e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjU5OTkzNzMsIm5iZiI6MTcyNTk5OTA3MywicGF0aCI6Ii85NTk2NzEwOC8zMjY2NDUxMDAtZDczM2M5MTUtZGY3Zi00NDk1LWIwYWQtZTE5OTZkYzcwMjBlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTEwVDIwMTExM1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTkwZWE3NjQ1MGQ2MjJjMzNiMTJiZGYyM2YyZjExNzU2MjY0ODE2MmFlMmVmZWQ4YmE2NDllNjllNjdlNWIwN2YmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.rRNIfQysrcd8oPPN2_Wjb6t_K9KZYHbnWyvHQqEXIqQ)](https://private-user-images.githubusercontent.com/95967108/326645100-d733c915-df7f-4495-b0ad-e1996dc7020e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjU5OTkzNzMsIm5iZiI6MTcyNTk5OTA3MywicGF0aCI6Ii85NTk2NzEwOC8zMjY2NDUxMDAtZDczM2M5MTUtZGY3Zi00NDk1LWIwYWQtZTE5OTZkYzcwMjBlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTEwVDIwMTExM1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTkwZWE3NjQ1MGQ2MjJjMzNiMTJiZGYyM2YyZjExNzU2MjY0ODE2MmFlMmVmZWQ4YmE2NDllNjllNjdlNWIwN2YmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.rRNIfQysrcd8oPPN2_Wjb6t_K9KZYHbnWyvHQqEXIqQ)

##### Aligning equations

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#aligning-equations)

Sometimes you will want to show your readers how you are reducing an expression. For this, the IEEE style requires that you align your equations properly.

To do this Obsidian you need to write the expressions inside the begin/end aligned tags: `$\begin{aligned}2x - 4 &= 6 \\ 2x &= 10 \\ x &= 5\end{aligned}`. Now you may be wondering what some of the other symbols mean so let me explain:

-   **\\\\** is for marking a new line.
-   **&** is for marking which character you want to align. One is needed in each line. So here, it'll align all the "=", as each line's "=" has an "&" symbol in front of it.

[![image](https://private-user-images.githubusercontent.com/95967108/326671281-87855a5e-5a9c-4617-bc80-d933d604e192.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjU5OTkzNzMsIm5iZiI6MTcyNTk5OTA3MywicGF0aCI6Ii85NTk2NzEwOC8zMjY2NzEyODEtODc4NTVhNWUtNWE5Yy00NjE3LWJjODAtZDkzM2Q2MDRlMTkyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTEwVDIwMTExM1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTUyZDE0YWY5ZGI0ZWFhZGY3MDBkMGJkMzAxYzg4MWQxODk1NmFmMmJjY2Y1ZTBmMWI3MWEyMTE1ZTBjNTliNWQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.M8L3brqzd7FDH8XeSF-sJNG0ZEHpkCBxL2JD_yhkufI)](https://private-user-images.githubusercontent.com/95967108/326671281-87855a5e-5a9c-4617-bc80-d933d604e192.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjU5OTkzNzMsIm5iZiI6MTcyNTk5OTA3MywicGF0aCI6Ii85NTk2NzEwOC8zMjY2NzEyODEtODc4NTVhNWUtNWE5Yy00NjE3LWJjODAtZDkzM2Q2MDRlMTkyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA5MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwOTEwVDIwMTExM1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTUyZDE0YWY5ZGI0ZWFhZGY3MDBkMGJkMzAxYzg4MWQxODk1NmFmMmJjY2Y1ZTBmMWI3MWEyMTE1ZTBjNTliNWQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.M8L3brqzd7FDH8XeSF-sJNG0ZEHpkCBxL2JD_yhkufI)

(MORE\_TO\_BE\_ADDED)

#### Page breaks

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#page-breaks)

Page breaks is a widely used tool, avaiable in everything from LaTex to Microsoft Word. It's especially useful if you want a seperate front page, or just dont like how a paragraph is split up it between two pages.

To make a page break in obsidian, all you have to do is paste this HTML:

`<div style="page-break-after: always;"></div>`

It is **important to note** that you should always have a line break before and after this HTML tag, to make sure it works properly. Another note is that it's going to appear invisible in live-editor mode, unless you move your cursor to it with your arrow keys.

---

## Contributing

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#contributing)

As said before, this repository tries to be the ultimate guide on how to setup Obsidian for academia, and for that, it'll be nice if you could contribute with your experience, workarounds, and workflows. If you know of any form of improvements(from the clarity and redaction of the documentation to new ways of configuring Obsidian), or if you encounter an issue, please don't hesitate to open an issue or, better still, create a PR. We'll surely review it and accept it. Thanks in advance :).

## Reference

[](https://github.com/MarcosNicolau/obsidian-for-academia?tab=readme-ov-file#reference)

[https://publish.obsidian.md/hub/04+-+Guides%2C+Workflows%2C+%26+Courses/for+Academic+Writing](https://publish.obsidian.md/hub/04+-+Guides%2C+Workflows%2C+%26+Courses/for+Academic+Writing)