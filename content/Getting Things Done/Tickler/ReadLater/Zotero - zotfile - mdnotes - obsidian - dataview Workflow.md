[[ReadItLater]] [[Article]]

# [Zotero -> zotfile -> mdnotes -> obsidian -> dataview Workflow](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536)

This is a workfrow about setting up a smooth(ish) transition from getting a pdf into [zotero](https://www.zotero.org/) (which is a reference manager), annotating it, extracting annotations (with or without color coding for that), pushing those into Obsidian using the [@argentum’s mdnotes plugin](https://github.com/argenos/zotero-mdnotes) - specifically, the latest alppha release at the time of this post: [0.2.0 alpha4](https://github.com/argenos/zotero-mdnotes/releases) and have those readily usable with [Michael Brenan’s Dataview plugin](https://github.com/blacksmithgu/obsidian-dataview).

2023 Update: there is a new plugin, the [Zotero Integration plugin](https://github.com/mgmeyers/obsidian-zotero-integration), that works well and simplifies the transfer of highlights from zotero to obsidian. There are still differences in operation; I still use zotfile because (1) zotero pdf reader doesn’t offer as many annotation options and (2) ZI isn’t always accurate at extracting highlights from some pdfs.

If you still wish to use this workflow, most of it has not changed for Zotero 6; the only issue is that you will need to use the older version of zotfile - version 5.0.16 ([available here](https://cdn.discordapp.com/attachments/722584061087842365/958273435887362048/zotfile-5.0.16-fx.xpi)) and disable updates on it.

Some Caveats:

1.  The mdnotes plugin I’m using is the current alpha build, that makes all of this really great. I am not sure how any of this will work for future versions of zotero. It does *not* work with earlier releases of mdnotes.
2.  I’m using a mac for this, and have not tested the workflow on windows.
3.  I’ve created a basic “Setting up Zotero” process, for those who want that. Feel free to skip anything irrelevant.
4.  I’m currently using [Juris-M](https://juris-m.github.io/), which is based on zotero with additional zotero fields for legal referencing. Other than the additional legal information added on to cases in my library, everything else should translate to zotero. The version I’m on is Juris-M 5.0.93m18. I have not tried the latest beta-builds of zotero as of this date. For this post and to avoid confusion, I’m going to say ‘zotero’, which means ‘the Juris-M build of zotero’. I do use Zotero (5.0.96.1) for the main sections #1 and #2, and Juris-M for everything from #3 onward.
5.  I’m using a test-book item in zotero, with a lorem ipsum text randomly highlighted.
6.  I’ve included screenshots and descriptions of what’s happening right before the screenshot.

## [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-1-setting-up-zotero-and-the-other-add-ons-1)1\. Setting up Zotero and the other add-ons

This is a list of one-time set-ups for this workflow in Zotero.

### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-11-zotero-installation-2)1.1 Zotero Installation

1.  Go to [zotero.org](https://www.zotero.org/).
2.  Download relevant installation file.
3.  Install zotero on your system.
4.  Get a zotero account.
5.  Open zotero. Once you open zotero, it should show you an Introduction pop-up. If you press Continue, it will take you to the plugin installation window. Here, it shows you the plugins available for the word processing applications you have (including Libre Office and MS Word). If you plan on using citations in any such program, select the appropriate plugins here and press “Continue”, which will install them.
6.  Once this is done, it will take you to an empty-looking window with “My Library” at the top left. This is your library, and if this is your first time using zotero, it’s probably empty. (Screenshot 01)
7.  Collections in Zotero look like sub-folders under “My Library” in the main zotero window, but function like tags, in that you can have the same item in more than one collection at the same time. You can create a new collection by selecting File → New Collection. Enter a name for your new collection (I enter “Open Access”). Press OK. It should show you the new collection under “My Library”. Screenshot 01-2 and 01-3).  
    01:  
    
    [![01 new zotero window](https://forum.obsidian.md/uploads/default/optimized/2X/f/f0a77470ff36888cba03c3413f2e95b0e369881a_2_690x411.png)](https://forum.obsidian.md/uploads/default/original/2X/f/f0a77470ff36888cba03c3413f2e95b0e369881a.png "01 new zotero window")
    

01-2  

[![01-2 New Collection](https://forum.obsidian.md/uploads/default/optimized/2X/f/fa8f5a8c649e1f5988a504cc9ae25a1749d18035_2_690x414.png)](https://forum.obsidian.md/uploads/default/original/2X/f/fa8f5a8c649e1f5988a504cc9ae25a1749d18035.png "01-2 New Collection")

01-3  

[![01-3 Open Access](https://forum.obsidian.md/uploads/default/optimized/2X/a/a39a57543a7844757b440b32c17907a12d45ec42_2_690x408.png)](https://forum.obsidian.md/uploads/default/original/2X/a/a39a57543a7844757b440b32c17907a12d45ec42.png "01-3 Open Access")

### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-12-zotero-sync-3)1.2 Zotero Sync

Before getting pdfs into zotero, you want to decide where you’d like to store these pdfs. If you’re not planning to use a zotero account to sync your library, then zotero will store your files locally on your computer at the [default location](https://www.zotero.org/support/zotero_data). If you are planning on intensive use of zotero for academic citation management, it’s probably best to get an account. If you plan on not syncing your library to any cloud, skip this step.

Zotero offers 300 MB of free storage, and [paid upgrades](https://www.zotero.org/settings/storage?ref=usb). Depending on your usage, this may or may not be enough. You can also choose to sync your library through a different cloud storage.

Steps.

1.  Open zotero
2.  Go to Preferences (Zotero → Preferences in Mac, Edit → Preferences on win)
3.  Go to the “Sync” tab.
4.  Input your zotero username and password, if you already have an account. Select “Create an account” if you didn’t do that in 1.1 (Screenshot 02)

![02 Sync](https://forum.obsidian.md/uploads/default/original/2X/9/949a5e4eba89eeddc01fcc19079b1a1f6c3e7f8b.png)

5.  Once you have an account, if you don’t plan on using zotero sync, unselect “Sync full-text context” as seen in the screenshot.
6.  You can use a webdav account for syncing instead, by choosing the “WebDAV” option in “Sync attachment files in My Library using” option.

If you’re not planning on using zotero file storage but want to use another cloud that isn’t WebDAV, go to the “Advanced” Tab, and then to the “Files and Folders” subtab (screenshot 04).

[![04 FilesandFolders](https://forum.obsidian.md/uploads/default/optimized/2X/e/e58c60c1eed7e92b4ad13c32dc72e7226d2df770_2_510x499.png)](https://forum.obsidian.md/uploads/default/original/2X/e/e58c60c1eed7e92b4ad13c32dc72e7226d2df770.png "04 FilesandFolders")

Zotero allows you to link files into your library (instead of attaching them) and uses the same cloud folder across different computers as long as their path to the “Base directory”. Here’s how to set that up:

1.  Select a base directory for your library under “Linked Attachment Base Directory”. This is where you want to store all your Zotero attachments. (eg. I created a folder in my locally-synced-cloud, and gave it a name, “ZoteroAttachments”) (Screenshot 05)

[![05 Base directory](https://forum.obsidian.md/uploads/default/optimized/2X/4/4136080ee579a108ea5df522ed8b6a8cd9ce574d_2_512x500.png)](https://forum.obsidian.md/uploads/default/original/2X/4/4136080ee579a108ea5df522ed8b6a8cd9ce574d.png "05 Base directory")

### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-13-install-the-browser-plugin-4)1.3 Install the Browser Plugin

Steps

1.  Install the zotero plugin on your preferred browser. For this, I’m going with Chrome.
2.  Go to [zotero.org/download](https://www.zotero.org/download)
3.  Select “Install Chrome Connector”, which should take you to the connector on the Chrome web store.
4.  Select “Add To Chrome” → “Add Extension”.
5.  The plugin should install, and then show you a pop-up that tells you how to use it.
6.  Once installed, click the menu button for the plugin and select Options.
7.  If you’re using sync, select the “Authorize” button under “Save to [Zotero.org](http://zotero.org/)” and log in to your zotero account when prompted. Once Logged in, accept defaults or change the key to your preference.
8.  The default settings under “Save to [Zotero.org](http://zotero.org/)” should have “Automatically take Snapshots…” and “Automatically download associated PDFs…” both enabled. I don’t use snapshots, so I have disabled that in mine, but that’s my preference. The defaults are usually fine here.

### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-14-install-zotfile-install-mdnotes-and-better-bibtex-for-steps-in-no-3-onward-5)1.4 Install Zotfile; Install Mdnotes and Better Bibtex for steps in No. 3 onward.

Here are the links to [Zotfile](http://zotfile.com/), [Zotero-mdnotes](https://github.com/argenos/zotero-mdnotes/releases), and [Better BibTex](https://retorque.re/zotero-better-bibtex/).

Steps:

1.  Save the .xpi files from the installation links onto your computer.
2.  In Zotero, go to Tools → Add-Ons
3.  Click on the settings button at the top-right corner, and select “Install Add-on From File” (Screenshot 06)

[![06 Addons](https://forum.obsidian.md/uploads/default/optimized/2X/8/84ceae244fefbc6e3250bb5346e53ca99c33000a_2_690x296.png)](https://forum.obsidian.md/uploads/default/original/2X/8/84ceae244fefbc6e3250bb5346e53ca99c33000a.png "06 Addons")

4.  Select the downloaded .xpi files and then click Install.
5.  Restart Zotero when prompted.

### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-15-zotfile-and-bibtex-basic-preferences-6)1.5 Zotfile and Bibtex: Basic Preferences

Zotfile can manage your pdfs, rename them, extract annotations and store them wherever you want it to do that.  
Zotero, Zotfile, and mdnotes also have hidden preferences, which I edit in part 3 of this workflow, with examples of different outputs for the various settings.

#### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-151-zotfile-preferences-7)1.5.1 Zotfile Preferences

Steps for setting up file organisation if you’re using a cloud to link files into zotero

1.  Go to Zotero → Tools → Zotfile Preferences
2.  In general settings, you can tell zotfile where to store your documents. For this, in “Location of Files”, choose Custom Location, and choose the folder you selected in 1.2 (in my case, “ZoteroAttachments”)
3.  You can choose to have zotfile sub-categorise your files in this folder, using [these wildcards](http://zotfile.com/#renaming-rules). Many people choose to categorise by Author (%a) or year (%y).
4.  I prefer organising my files by subject, so I pick %c, meaning collection. You can also combine different wildcards, like so: “/%c/%a” (Screenshot 07). The wildcards will create folders with the entirety of the field referred to. In my case, it will create a folder with the name of the collection in Storage (/ZoteroAttachments/CollectionName)

[![07 Folder organisation](https://forum.obsidian.md/uploads/default/optimized/2X/f/f35dd472166403a775b5b6d350ec65933ef95dea_2_453x500.png)](https://forum.obsidian.md/uploads/default/original/2X/f/f35dd472166403a775b5b6d350ec65933ef95dea.png "07 Folder organisation")

Steps for setting up zotfile renaming

1.  Go to Zotero → Tools → Zotfile Preferences
2.  Under the Renaming Rules Tab, using [these wildcards again](http://zotfile.com/#renaming-rules), decide how you want to name your files. This depends on what works best for you. The default settings can be fine if you like that. I use: “{%a} {(%y)} {%t}”, because I like the way that is visualised. (see screenshot 08)

[![08 Renaming](https://forum.obsidian.md/uploads/default/optimized/2X/0/09de187cec3890ae5e19edf30a6b16d3b5fd2474_2_452x499.png)](https://forum.obsidian.md/uploads/default/original/2X/0/09de187cec3890ae5e19edf30a6b16d3b5fd2474.png "08 Renaming")

3.  Next, go to advanced settings, and under “Other Advanced Settings”, select the “Always rename” option for “Automatically rename new attaktments”. Disable “Ask user when attaching new files”. (Screenshot 09).
4.  Close Preferences.

[![09 Renaming 2](https://forum.obsidian.md/uploads/default/optimized/2X/d/d9c2af2296980bcab6175ced2f1fc54c3687fbc1_2_451x500.png)](https://forum.obsidian.md/uploads/default/original/2X/d/d9c2af2296980bcab6175ced2f1fc54c3687fbc1.png "09 Renaming 2")

## [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-2-get-references-and-pdf-papers-into-zotero-extracting-annotations-basic-8)2\. Get References and PDF papers into Zotero, Extracting Annotations (basic)

Zotero has [browser plugins](https://www.zotero.org/download/) that allow you to directly add items to zotero. This works well with most journal databases (which, if accessible, sometimes allow you to download the pdf directly through the plugin). It also works well with google scholar, which I’m using for this demo.

For this, I’ve picked a random search for [“open access” in google scholar](https://scholar.google.com/scholar?q=open+access), picking one of the results that gave me access to the pdf (Open Access and global participation in science by James A Evans et al, Science, 20 Feb 2009: Vol. 323, Issue 5917, pp. 1025, DOI: 10.1126/science.1154562).

Steps to get reference and pdf into zotero:

1.  To use the zotero chrome connector, from the google scholar search page, click on the zotero plugin (it should look like a folder) (Screenshot 10)  
    
    [![10 chrome connector](https://forum.obsidian.md/uploads/default/optimized/2X/8/8f6cbbfb511a9b01211470f744fd2c052a49aded_2_690x401.png)](https://forum.obsidian.md/uploads/default/original/2X/8/8f6cbbfb511a9b01211470f744fd2c052a49aded.png "10 chrome connector")
    
2.  Once you click on it, it should open a po-pup that lists all the results on the page as selectable items.
    
3.  Select the one(s) you want. Then select “OK” (Screenshot 11)  
    
    [![11 Add to zotero](https://forum.obsidian.md/uploads/default/optimized/2X/e/e12e293231f59570eb20797fa21260e21b430a13_2_690x441.png)](https://forum.obsidian.md/uploads/default/original/2X/e/e12e293231f59570eb20797fa21260e21b430a13.png "11 Add to zotero")
    
4.  The plugin shows a pop-up saying that it is saving to My Library, with the name of the paper below that. It should also show a semi-transparent pdf icen with “Full Text” on it. This becomes opaque if zotero can access the file (which it can, in this case). If you click on the arrow on the right of “My Library”, you can select a different collection for the reference and the file. I select the “Open Access” Collection (Screenshot 12).  
    
    [![12 Save to Collection](https://forum.obsidian.md/uploads/default/optimized/2X/f/fd5983e91c2480f8fa26df653a0b47a0fa7a9d62_2_690x439.png)](https://forum.obsidian.md/uploads/default/original/2X/f/fd5983e91c2480f8fa26df653a0b47a0fa7a9d62.png "12 Save to Collection")
    
5.  Once Zotero has the PDF, zotfile renames it and transfers it to the folder you specified in zotfile settings. You get a pop-up confirming that zotfile has renamed the pdf (Screenshot 14).
    

[![14 Zotfile Confirmation](https://forum.obsidian.md/uploads/default/optimized/2X/5/5e65eb731f358691084e154df43c2053d4e1ec0e_2_690x428.png)](https://forum.obsidian.md/uploads/default/original/2X/5/5e65eb731f358691084e154df43c2053d4e1ec0e.png "14 Zotfile Confirmation")

6.  You can also add Tags, Clicking on done. Here, I’ve added two tags, Unread and Science (Screenshot 15).

[![15 Add tags](https://forum.obsidian.md/uploads/default/optimized/2X/4/45e8df56d3c38dd412ce45205959ab55a1948629_2_690x442.png)](https://forum.obsidian.md/uploads/default/original/2X/4/45e8df56d3c38dd412ce45205959ab55a1948629.png "15 Add tags")

7.  When you go to zotero, you can see the reference you’ve added, along with the snapshot and the link to the file (which is the pdf of the paper that was downloaded with the chrome plugin) (Screenshot 16)

[![16 zotero with PDF](https://forum.obsidian.md/uploads/default/optimized/2X/c/c7500c0cd4c635f4046a210927c65aef4e6c1628_2_690x410.png)](https://forum.obsidian.md/uploads/default/original/2X/c/c7500c0cd4c635f4046a210927c65aef4e6c1628.png "16 zotero with PDF")

8.  This PDF can be annotated in whatever pdf reader you choose (This does not include the new zotero pdf reader beta tool).
    
9.  For those who do not care about formatting annotations, Zotfile allows you to extract any annotations you’ve made on the PDF file. simply right-click on the pdf file in Zotero, hover on “Manage Attachments”, and Select “Extract Annotations” (Screenshot 17). This should create a new note for the Reference with any highlights you made in the PDF extracted as text into the note. (Screenshot 18)
    

Screenshots 17 and 18:

[![17 Extracting Annotations.](https://forum.obsidian.md/uploads/default/optimized/2X/4/4746b31f0cf2c7f793b4066dad25ccfa81d7a2d3_2_690x409.png)](https://forum.obsidian.md/uploads/default/original/2X/4/4746b31f0cf2c7f793b4066dad25ccfa81d7a2d3.png "17 Extracting Annotations.")

[![18 Extracted Annotations](https://forum.obsidian.md/uploads/default/optimized/2X/c/c8dba26d624dd6608e871ebefb32f34c44a3521e_2_690x411.png)](https://forum.obsidian.md/uploads/default/original/2X/c/c8dba26d624dd6608e871ebefb32f34c44a3521e.png "18 Extracted Annotations")

## [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-3-formatting-extracted-annotations-for-mdnotes-and-dataview-9)3\. Formatting Extracted Annotations for mdnotes and dataview

(I’m using Juris-M from here on, but everything I do here should work the same way on Zotero).

For those who do want to format annotations, Zotfile allows a number of edits to give you a lot of options. I’ll go through some of them here. This requires some comfort with fiddling with and editing the configuration files (or “hidden preferences”) in zotero. This assumes that you’re comfortable enough with step 9 in No. 2. I’m also not going to give screenshots for steps after this point, and instead reserving screenshots for displaying the export format.

Mdnotes has some different templates for the export; The [documentation for that is here](https://argentinaos.com/zotero-mdnotes/docs/templates/). Because This workflow involves changing the default and hidden settings for both zotfile and mdnotes, I’m first going to go through my edits in the mdnotes template and then go through the zotfile formatting, so I can display the output in obsidian for the different formats *after having edited the mdnotes template*

### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-31-mdnotes-default-template-10)3.1 Mdnotes default template:

The mdnotes plugin comes with a default template, saved in a .md file. You can find this file by checking Tools → Mdnotes Preferences. In the “Export Preferences” tab, the last section shows you the Template Folder path. There, the default template is called “Mdnotes Default Template.md”, and this is the file that I will be using.

In mdnotes preferences, my “Export Preferences” settings are:

-   enable “Use the item’s citekey as title” (this uses the Better BibTex citekey as the title of the .md export. That can be edited by going to Zotero → Preferences, to the “Better BibTex” tab, to the Citation keys sub-tab, and editing the “Citation key format” option. Details for formatting that are at [this link](https://retorque.re/zotero-better-bibtex/citing/). My own format reads: “\[auth\](\[year\])\[shorttitle3\_3\]”)
-   “Single file” for File organisation. (I prefer having all my notes on a particular reference in one single file in zotero. Choosing split files exports separate .md files for each note in the reference and a separate metadata note for the reference itself.)
-   A Folder in my Obsidian Vault for the Export Directory (Pick whatever folder works for your organisation of reference notes)
-   “Attach file links to zotero” is enabled

Here’s what the default mdnotes template looks like:

```
{{title}}

![[%(metadataFileName)#Metadata]]

Other files:
{{mdnotesFileName}}
{{metadataFileName}}

##  Zotero links
{{localLibrary}}
{{cloudLibrary}}

## Notes
```

This is the template that’s used when you use mdnotes to “Create full export note”. Other export formats are also available, if you want to export individual notes separately into markdown format for obsidian to read.

This includes {{placeholders}} and %(wildcards). Placeholders are the terms within curly brackets, like so: {{placeholder}}, and can be defined in the hidden preferences. Wildcards are the terms in regular brackets following a percentage symbol, like so: %(wildcard). Mdnotes has an option to “skip” placeholders that don’t exist, while this cannot be done for wildcards. If mdnotes encounters a wildcard that doesn’t exist, it exports the term “undefined” in its place. So for this workflow to be robust in exporting different kinds of references, we want to try to use placeholders instead of wildcards. Mdnotes can read custom placeholders, as long as they are defined with existing zotero fields.

#### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-311-adding-and-editing-mdnotes-placeholders-11)3.1.1 Adding and Editing Mdnotes Placeholders

Update: Since first writing this post, Dataview has been updated to include *inline* metadata, which works significantly better than plain YAML because it allows for the use of backlinks to other pages in your obsidian vault. While the process remains the same, there are some updates to the syntax. I’m changing this section to use inline tags, along with yaml tags for the alias, which still needs to be in YAML format, so you have samples of both. YAML placeholders in this section generally have the placeholder format {{yamlplaceholder}}, whereas the inline ones are just {{placeholder}}. I had to remove the old tags due to post-length limits.

First, we want to create placeholders to add to the YAML Metadata that the Dataview plugin in Obsidian can read. For this, we create custom placeholders that are formatted according to the YAML-dataview requirements, meaning strings need to be in quotes, anything with multiple references (such as a book with more than one author) needs to be formatted with newline bullets for each such item. I have a set of custom placeholders and formats here that can be used.

Steps to add a new Mdnotes Placeholder

1.  Go to Zotero → Preferences → Advanced (subtab) → click on “Config Editor”.
2.  Once inside, search for “mdnotes” (without quotes).
3.  This should show a bunch of settings, listed with “Preference Name”, “Status”, “Type”, and “Value”.
4.  To add a new placeholder, right-click on any preference. Hover over “New”, and Select the option “String”
5.  It opens a pop-up, “New String Value”, asking you to enter the preference name.
6.  Enter `extensions.mdnotes.placeholder.yamlauthorlist` (without the backticks, if they show up when you’re copy-pasting). This creates a new placeholder, {{yamlauthorlist}}. Press OK.
7.  Next, it asks you to enter string value.
8.  Enter `{"content":"Authors: \n- \"{{field_contents}}\"","zotero_field":"author","link_style":"no-links","list_separator": "\"\n- \""}` (again without the backticks). This points to the “author” field in zotero, and formats the output to first Tag the output with “Authors:”, and then have the authors each listed in new lines with a ‘-’ bullet and include quotation marks for all the Authors exported, without links on them.
9.  Repeat the process from 4 to 8 for each new placeholder you want to define.

Here are some of my placeholders, I’ve listed them in this format:

1.  {{placeholder}} (What the placeholder does)–> The term in {{}} is the name of the placeholder to be used in the final template
2.  `Preference name` → Use this in Step 6 above.
3.  `Value` → Use this in Step 8 above.

###### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#placeholders-12)Placeholders:

1.  {{DOI}} (outputs the DOI)
2.  `extensions.mdnotes.placeholder.DOI`
3.  `{"content":"\nDOI:: {{field_contents}}", "field_contents": "{{content}}", "link_style": "no-links"}`

.

1.  {{author}} (outputs list of author in wiki link style)
2.  `extensions.mdnotes.placeholder.author`
3.  `{"content":"Authors:: {{field_contents}}", "link_style": "wiki", "list_separator": ", "}`

.

1.  {{bookTitle}} (gives the title of the book)
2.  `extensions.mdnotes.placeholder.bookTitle`
3.  `{"content":"Book:: \"{{field_contents}}\"","zotero_field":"bookTitle","link_style":"no-links"}`

.

1.  {{book}} (outputs name of book, if edited volume)
2.  `extensions.mdnotes.placeholder.book`
3.  `{"content":"\nBook:: \"{{field_contents}}\"","zotero_field":"book","link_style":"no-links"}`

.

1.  {{date}} (outputs the date of the item)
2.  `extensions.mdnotes.placeholder.date`
3.  `{"content":"Year:: {{field_contents}}","zotero_field":"date","link_style":"wiki"}`

.

1.  {{collections}} (outputs collections as subjects)
2.  `extensions.mdnotes.placeholder.collections`
3.  `{"content":"\nSubjects:: {{field_contents}}", "field_contents": "{{content}}", "link_style": "wiki", "list_separator": ", "}`

.

1.  {{tags}} (outputs tags as wikilists)
2.  `extensions.mdnotes.placeholder.tags`
3.  `{"content":"{{field_contents}}", "field_contents": "{{content}}", "link_style": "wiki", "list_separator": ", "}`

(note: tags does not have a metadata field of its own and uses the field of collections. this is because dataview does not accept values of the first field entry of inline fields if there is more than one entry made, the latter field entries overwrite the previous ones. Since my collection and tag fields in zotero are both used to categorise subjects, I club them in the mdnotes template format).

1.  {{editor}} (outputs the list of editors)
2.  `extensions.mdnotes.placeholder.editor`
3.  `{"content":"\nEditors:: {{field_contents}}", "link_style": "wiki", "list_separator": ", "}`

.

1.  {{itemType}} (outputs the item type)
2.  `extensions.mdnotes.placeholder.itemType`
3.  `{"content":"Item_Type:: {{field_contents}}","zotero_field":"itemType","link_style":"wiki","list_separator": ", "}`

.

1.  {{yamlbooktitle}} (Outputs the title of the book)
2.  `extensions.mdnotes.placeholder.yamlbooktitle`
3.  `{"content":"BookTitle: \"{{field_contents}}\"","zotero_field":"bookTitle","link_style":"no-links"}`

.

1.  {{yamltitle}} (outputs the title of the reference)
2.  `extensions.mdnotes.placeholder.yamltitle`
3.  `{"content":"{{field_contents}}","zotero_field":"title","link_style":"no-links"}`

.

###### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#mdnotes-default-template-13)MDnotes default template:

```
---
aliases: ["{{yamltitle}}"]
Title: "{{yamltitle}}"
{{yamlbooktitle}}
---

# {{yamltitle}}

{{abstractNote}}

### Metadata
#zotero  #literature-notes  #reference

{{itemType}}
{{bookTitle}}
{{author}}
{{date}}
{{DOI}}
{{collections}}, {{tags}} 
{{book}}
{{editor}}

#### Links
{{pdfAttachments}}

#####  Zotero links
{{localLibrary}}
{{cloudLibrary}}
```

### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-32-formatting-extraction-of-notes-14)3.2 Formatting Extraction of Notes:

For this section, I’m going to describe zotfile hidden preferences for formatting, what they do to the zotfile Extract, and give you screenshots of the zotfile export and the corresponding obsidian export. I’ve created a sample reference item (A book section) for this, with Lorem Ipsum text as the attached PDF file. It has some annotations and highlights of different colors. I’m going to go through a few iterations of formats and give screenshots of the mdnotes output in Obsidian, along with references about what the setting does. You can use the settings for whatever format fits your needs.

I start with the default settings and add additional formats in steps so it’s easy to pick the effects you do want, and notice what’s happening with each one. I assume for this that you’re comfortable with using the config editor (described in 3.1.1 above).

Each of these requires you to extract annotations using zotfile after adding the formatting edits in the config editor, and then exporting the whole item using mdnotes (right click on parent item → Mdnotes → Create full export note) to get the formatted output in Obsidian.

#### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-321-default-zotfile-extraction-15)3.2.1 Default Zotfile Extraction

By default, Zotfile extraction of Annotations gives Highlights as text in quotes (“Lorem ipsum dolor sit amet”), Annotated comments as italicised text (*Test comment on yellow highlight with \[\[backlinkthingamagees\]\]*), and Underlined annotations as Underlined text in quotes (“Lorem Ipsum Text PDF”). Each of these is followed by a link that opens the page at which the annotation is made in your default PDF viewer. (Screenshots 20, 21)

[![20 Defaut-zot](https://forum.obsidian.md/uploads/default/optimized/2X/d/dd82e748fbd48e621f2e79a74c7ede9524399c3a_2_618x500.png)](https://forum.obsidian.md/uploads/default/original/2X/d/dd82e748fbd48e621f2e79a74c7ede9524399c3a.png "20 Defaut-zot")

  

[![21 Default](https://forum.obsidian.md/uploads/default/optimized/2X/0/0bc5011724ea5fe45f04e35fcd4bac8d3e59f526_2_690x431.png)](https://forum.obsidian.md/uploads/default/original/2X/0/0bc5011724ea5fe45f04e35fcd4bac8d3e59f526.png "21 Default")

#### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-322-changing-the-note-title-16)3.2.2 Changing the Note Title

In zotero’s config editor, the setting `extensions.zotfile.pdfExtraction.formatNoteTitle` Can be edited to change the Title of the Extracted Note.  
The default is `<p><b>%(title) (%(date))</b><p>`. Because I’m not interested in keeping the date, I change it to `<p><b>%(title) </b><p>`.  
Output in Screenshots 22, 23.

[![22](https://forum.obsidian.md/uploads/default/optimized/2X/6/64662eab9b13de6781df2c8813b0b03d4c3298f1_2_621x500.png)](https://forum.obsidian.md/uploads/default/original/2X/6/64662eab9b13de6781df2c8813b0b03d4c3298f1.png "22")

  

[![23](https://forum.obsidian.md/uploads/default/optimized/2X/3/328940059286d80fef69ca17a1028f3e975217d9_2_690x431.png)](https://forum.obsidian.md/uploads/default/original/2X/3/328940059286d80fef69ca17a1028f3e975217d9.png "23")

#### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-323-editing-the-annotated-comments-17)3.2.3 Editing the Annotated Comments

I want to visually separate out my annotated comments from the parts of the main text that are highlighted. I also want to add a tag to my name for searchability.

This requires editing the `extensions.zotfile.pdfExtraction.formatAnnotationNote` preference.  
The default is `<p><i>%(content) (<a href="%(uri)">note on p.%(page)</a>)</i></p><br>`

##### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#adding-blockquotes-18)Adding Blockquotes

I change it to `<blockquote><p> [[%(label)]] %(content) (<a href="%(uri)">note on p.%(page)) </blockquote><br></p>`  
This adds a blockquote to my annotations; that gives a visual break to emphasise that these are separate from the rest of the text when I review the reference notes, and I know that I wrote them. %(label) extracts the name of the author from the PDF reader used for the annotations. the \[\] tags it, so it’s backlinked to the name in Obsidian for easy reference.  
Output in screenshots 24, 25.

[![24](https://forum.obsidian.md/uploads/default/optimized/2X/c/c204f96df4738585d12e0652b8d920082a3b4db8_2_622x500.png)](https://forum.obsidian.md/uploads/default/original/2X/c/c204f96df4738585d12e0652b8d920082a3b4db8.png "24")

  

[![25](https://forum.obsidian.md/uploads/default/optimized/2X/6/6214fae67f2e4cb71a3fd204922662a44623410f_2_690x431.png)](https://forum.obsidian.md/uploads/default/original/2X/6/6214fae67f2e4cb71a3fd204922662a44623410f.png "25")

(Side note - you might prefer to put highlights in blockquotes, but since this is a reference note, I assume that the default is a quote, and try to emphasise my thoughts on the note with the blockquote, since that is what I need to pay attention to while reviewing).

#### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-324-changing-underlines-19)3.2.4 Changing Underlines

Mdnotes converts underlines to markdown headers. This makes sectioning in the annotations easy - Underlining headers in the PDF makes them sections. To facilitate this, I edit the underline to remove quotation marks and the citation link.

The underlining can be edited in `extensions.zotfile.pdfExtraction.formatAnnotationUnderline`  
The default value is `<p>"<u>%(content)</u>" (%(cite))</p>`.

I edit that to `<p><u>%(content)</u><br></p>`  
Output in screenshots 26, 27.

[![26](https://forum.obsidian.md/uploads/default/optimized/2X/4/47d7c270492126ff9f7c40752f77f736ba83f323_2_621x500.png)](https://forum.obsidian.md/uploads/default/original/2X/4/47d7c270492126ff9f7c40752f77f736ba83f323.png "26")

  

[![27](https://forum.obsidian.md/uploads/default/optimized/2X/d/dfcbf9cfd20bd31f4575e8631174ff09d91053f1_2_690x431.png)](https://forum.obsidian.md/uploads/default/original/2X/d/dfcbf9cfd20bd31f4575e8631174ff09d91053f1.png "27")

#### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-325-highlight-colors-20)3.2.5 Highlight Colors

Zotfile can extract the Highlighted text according to color. It can also separate out the annotations into separate notes according to the color of the highlight. This is controlled in the preference  
`extensions.zotfile.pdfExtraction.colorAnnotations`. This is a boolean preference, the default value is “false”. Doulble clicking it changes it to “true”.

If you want separate notes for each color, double click on the boolean preference `extensions.zotfile.pdfExtraction.colorNotes`. The default value is false. Changing it to true makes zotfile extract highlights into different notes, grouped by the color of the highlight. For the screenshots, I’m keeping this value as “false”, so you can see the different colors within the same screenshot.

Output in screenshots 28, 29.

[![28](https://forum.obsidian.md/uploads/default/optimized/2X/0/02ab04836b74eb14e13759b930d83e2a57e5ac8c_2_616x500.png)](https://forum.obsidian.md/uploads/default/original/2X/0/02ab04836b74eb14e13759b930d83e2a57e5ac8c.png "28")

  

[![29](https://forum.obsidian.md/uploads/default/optimized/2X/7/7a492bd2005e76e66723287d9609da4881eabfcb_2_690x431.png)](https://forum.obsidian.md/uploads/default/original/2X/7/7a492bd2005e76e66723287d9609da4881eabfcb.png "29")

#### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#h-326-editing-the-color-title-output-21)3.2.6 Editing the color title output

Now, the reason that I use colored highlights is to visually separate out what I’m thinking when I annotate a document. Yellows are default highlights, Cyans are things that the author says that I think are important for things I’m working on, reds are things that I disagree with the author of the paper on, greens are references I want to follow up and read, Magentas are places where the author critiques someone else.

Having the extracted tags name the color before each annotation does not help me much. Zotfile lets me edit the color categories, so I can tag it with whatever I actually want it to say.

This is in the preference `extensions.zotfile.pdfExtraction.colorCategories`. The default value is a string of colors and hex codes: `{"Black": "#000000", "White": "#FFFFFF", "Gray": "#808080", "Red": "#FF0000", "Orange": "#FFA500", "Yellow": "#FFFF00", "Green": "#00FF00", "Cyan": "#00FFFF", "Blue": "#0000FF", "Magenta": "#FF00FF"}`. The color names refer to a range of RGB points that will be read as that particular color category, the hexcode is the category name that zotfile can use instead. I edit this preference to read `{"Black": "", "White": "", "Gray": "[[Argument]]:", "Red": "[[Disagreement]]:", "Orange": "[[Idea]]", "Yellow": "", "Green": "- [ ] ", "Cyan": "[[Important]]", "Blue": "[[Confusion]]:", "Magenta": "[[Critique]]:"}`  
to correspond with the labels I want it to use. I put some of these in backlinks for Obsidian.

For the green tag, I edit the hex code to use a “task” tag, which Dataview can extract.

This is insufficient for getting the output I want, however, which is for the color names to be replaced with the custom tags.  
That setting is in `extensions.zotfile.pdfExtraction.formatAnnotationHighlight`  
the default value for this is `<p>"%(content)" (%(cite))</p>`  
I change that to `<p>%(color_category) %(content) (%(cite)) <br></p>`  
Which tells zotfile to use the custom color tags.

Output in screenshots 30, 31.

[![30](https://forum.obsidian.md/uploads/default/optimized/2X/3/391f5d54071a6e18f3b1b4486e26c97e7ece065f_2_672x500.png)](https://forum.obsidian.md/uploads/default/original/2X/3/391f5d54071a6e18f3b1b4486e26c97e7ece065f.png "30")

  

[![31](https://forum.obsidian.md/uploads/default/optimized/2X/6/680047f461af0eac59d89ad2686cdaab9f66d041_2_690x431.png)](https://forum.obsidian.md/uploads/default/original/2X/6/680047f461af0eac59d89ad2686cdaab9f66d041.png "31")

##### [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#removing-the-colors-retaining-colortags-22)Removing the colors, retaining colortags

Because of the excessive html text that now gets exported, I prefer not to have colored highlights in my extracted annotations. I can retain the custom color tags and remove the highlights by setting `extensions.zotfile.pdfExtraction.colorAnnotations` to “false” once again, while retaining the %(color\_categories) wildcard in the highlight extraction.  
Output in screenshots 32, 33.

[![32](https://forum.obsidian.md/uploads/default/optimized/2X/0/099d6f3e4f427b885d5ccf5dc1e789f38db7e740_2_663x500.png)](https://forum.obsidian.md/uploads/default/original/2X/0/099d6f3e4f427b885d5ccf5dc1e789f38db7e740.png "32")

  

[![33](https://forum.obsidian.md/uploads/default/optimized/2X/e/e38c8d77df34b539d48c5e68bd36108ff506fae8_2_690x431.png)](https://forum.obsidian.md/uploads/default/original/2X/e/e38c8d77df34b539d48c5e68bd36108ff506fae8.png "33")

## [](https://forum.obsidian.md/t/zotero-zotfile-mdnotes-obsidian-dataview-workflow/15536#dataview-23)Dataview

Once in obsidian, the Dataview plugin can extract and output your references based on different conditions.

In reference to my “green” color tag replacement above, one thing I like to have is an automated reading list, sorted by the book/paper I got the reference from. For this, I use

````
```dataview
task from #zotero    
````

For this output, I’m restricting it to the fake tag I created (#authorref) to keep it to the fake reference note. (I usually use #zotero, which lists my reading list from all exported literature notes)

````
```dataview
task from #authorref 
````

Output in screenshot 34.

[![34](https://forum.obsidian.md/uploads/default/optimized/2X/4/402770dca8b9b4876611348d02f9aca98a8dad21_2_690x219.png)](https://forum.obsidian.md/uploads/default/original/2X/4/402770dca8b9b4876611348d02f9aca98a8dad21.png "34")

Other Dataview queries and the general format for Dataview can be seen [at this link](https://blacksmithgu.github.io/obsidian-dataview/#/queries).