[[ReadItLater]] [[Article]]

# [An Integrated Qualitative Analysis Environment with Obsidian](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/)

Published Aug 13, 2021

![Qualitative data analysis using Obsidian](https://fulcra.design/media/_Obsidian-IQAE.png)

Qualitative data analysis using Obsidian

[Download the Qualitative Analysis Environment kit from GitHub](https://github.com/ryanjamurphy/obsidian-qualitative-analysis-environment)

MaxQDA, NVivo, Atlas.ti, and a variety of other apps are designed to help researchers analyze qualitative data. These apps are doubtlessly powerful, but they all offered too steep of a learning curve when I was tasked with a small analysis project in 2020. (Plus, they’re expensive!) Instead,\*\* I crafted an Obsidian environment for qualitative data analysis.\*\*

The core idea: take each of the pieces of text you’re working with, make it easy to traverse them, and add in ways of coding them and writing up what the codes mean.

In this example, I had to analyze a set of open-ended questions about the student experience during the COVID-19 pandemic. There were hundreds of answers ranging from one or two words to hundreds of words from individual students. My goal was understanding the key themes and interesting outliers in this set of data.

I adopted a grounded field theory approach for this study. I deeply read each response, highlighting the key points and looking for commonalities and oddities. As those interesting phenomena emerged, I clustered and described them. Once the data had been thoroughly reviewed, I quantified the number of responses attributed to each of the themes I uncovered in order to get a sense of the most and least common themes. I also checked each theme/insight against one another and refined them to reduce redundancy as needed. The final report consisted of a ranked list of these themes, sorted by how often they were reported, a description of each theme, and a selection of illustrative responses for them from students.

[

## \# How to do this with Obsidian

](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/#how-to-do-this-with-obsidian)

I have created a kit for this Qualitative Analysis environment for you to download and use for any new analysis project you take on. To set it up, see the instructions immediately below. Throughout the rest of this guide, however, I explain how to do this from scratch (while referencing the kit).

[

### \# Setting up the Environment

](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/#setting-up-the-environment)

1.  Install Obsidian, if you haven’t already. See [https://obsidian.md](https://obsidian/) for the latest releases.
2.  [Download the Qualitative Analysis environment starter kit from GitHub](https://github.com/ryanjamurphy/obsidian-qualitative-analysis-environment).
3.  Extract the downloaded kit wherever you’d like on your computer.
4.  Open Obsidian, open the Vault Picker (the little vault icon in the bottom-left), and open the newly-extracted folders.
5.  To use all of the environment’s functionality, you have to disable Safe Mode in the vault (because it uses some community plugins). To do this, go to Preferences → Community Plugins and turn Safe Mode off.

[

### \# Preparing the data

](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/#preparing-the-data)

First, make every data point its own markdown (`.md`) file, naming them sequentially starting at 1. Create a folder on your computer titled “Integrated Qualitative Analysis Environment” (or whatever you’d like). Create a subfolder in that folder called “data” (or whatever you’d like). Then, open Obsidian, go into the Vault Picker (the vault icon in the bottom-left of the app), and create a new vault. Select the “Integrated Qualitative Analysis Environment” top-level folder you created a moment ago. This will create a data analysis vault for you to customize into the perfect environment for this task.

Putting the data points in each of their own files and numbering them sequentially is a trick: it allows us to use the core Daily Note plugin’s “Next Daily Note” and “Previous Daily Note” commands to quickly traverse the responses. So, enable that plugin, and set those two commands to an easy-to-reach hotkey (I used cmd+alt+→/←. You will be using these commands at least once for every piece of data you’re analysing!

Second, create a folder in your “Analysis Project” called “Themes”. Then, in your new Obsidian vault, go to `Preferences → Files & Links → Default Location for New Notes`, and change this to your new Themes folder. This will mean that every new note you create from links or from the “New note” command will show up in this folder.

[

### \# Coding the data

](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/#coding-the-data)

Open the first data point—the file in the “data” folder named “1”.

Below the text data, add a footer. You could use a heading (e.g., `## Coding`). I just left a couple of new lines between the data itself and where I was putting the codes (see the screenshot). In this footer, you will simply list each of the themes you identify in the data point.

Review the data. What does it say? What’s interesting about it? How might it help you answer your research question(s)? Think of the answers to these questions as themes: they are the interesting takeaways relevant to this piece of data. In the footer, write out these themes.

Here’s the secret to making this whole set-up work: add each code as an internal link. That affords us several things:

-   Codes are suggested when you start a new internal link `[[`, so that we can choose from the options instead of trying to recall them.
-   The individual responses will be structurally related to the codes via backlinks (and visually linked to the codes via the graph view).
-   Editing a code by renaming it will propagate the change to that code throughout the data.
-   Finally, it makes codes themselves an object we can add information to. You can open a code-as-link as a note and describe it, embed exemplary instances of the coding from the responses, and so on.

You may want to keep a Code Index, just to provide an easy place to organize and see all the codes you’ve identified at once. In the code Index, list each code you add to your data. Feel free to order them under headings or however else you’d like!

Once you’ve finished reading this data point and adding themes, move onto the next one by using the Next Daily Note command (or tapping the hotkey you assigned earlier).

[

### \# Analyzing the data

](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/#analyzing-the-data)

When using grounded field theory, you should incrementally update, revise, and refine your theory—your encoding—as you review the data. The goal is to render visible all of the interesting insights that lie inside your data, to clearly explain what those findings are, and to continually check and re-check them as you continue to review your data.

That means that as you review more and more data, you’re doing four things:

1.  labelling the data points with the themes you’ve identified already;
2.  creating new themes to call-out anything new in the data point you haven’t already picked up on;
3.  refining existing themes by (a) summarizing and adding detail to them (commonly referred to as writing memos about the themes), (b) embedding particularly illustrative examples of them in the data, (c) splitting up themes if they actually contain different important ideas, and (d) combining themes if they are significantly overlapping; and
4.  as necessary, looking for themes of themes: clusting and structuring the insights you’ve found inasmuch as the clustering makes your takeaways clearer or more impactful.

[

### \# Reporting on the data

](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/#reporting-on-the-data)

Once you’ve reviewed all the data at least once, you should have a set of themes clustering the different data points by the interesting insights they contain. You may want to go back through the data—or the themes, or the specific subsets of the data—more than once to refine your analysis further (see analysis steps 1-4 above). Once you feel satisfied with the takeaways, it’s time to write it up.

[

#### \# Quantifying your themes

](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/#quantifying-your-themes)

An easy thing to do is quantify the number of data points associated with each theme. This gives you a quick estimate of how frequent or common these takeaways are found in your data. 

There are many many ways you may quantify the number of data points per theme. The simplest is just to use Obsidian’s core Search functions. For each theme, enter `"` followed by the exact name into your search, then end the search query with `"`. This will search for exact mentions of the linked theme. Once the search has finished, tap on the Copy Search Results button above the search query text box. Last, in the options presented to you, change the List Prefix to “Numbered.” This gives you a count for the number of results for each theme.

However, that could be tedious if you have a lot of themes to count. Instead, you can use Dataview as follows:

1.  Install and enable the Dataview plugin.
2.  Create a “Statistics” page in your vault’s top-level folder.
3.  Put the following code block in the new statistics page, making sure to initialize give the code block the type “dataview”. (I.e., type “dataview” immediately after the first three backticks of the code fencing.) Note that if you named the “Themes” folder something different, you’ll have to change the name specified in the second line of the code block.

(Note: this is already done in the Qualitative Analysis environment starter kit. Just visit the Statistics note to see this info!)

|   ``` 1 2 3 ```   |   ``` TABLE length(file.inlinks) as "Data Points", length(file.outlinks) as "Related Themes" FROM "codes" SORT length(file.inlinks) DESC ```   |
| --- | --- |

This generates a table listing each theme, the number of data points associated with that theme, and the number of other themes you’ve linked to that theme (if you have done so at all).

When reporting on your themes, these counts give you some starting points. Why do the top themes appear so frequently? Why are the bottom ones rare? Speculate, theorize, debate, and discuss!

[

#### \# Writing up each theme

](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/#writing-up-each-theme)

It’s your job to report on the relevance of the themes you’ve uncovered to your research question(s). The memos you’ve already developed about each theme give you a starting place for commentary. Build on those, and use any exemplary cases you’ve embedded to illustrate your points. If you need to look back at your data, the backlinks from your themes will point to all of the data points you coded with a given theme.

You may also want to examine themes that seem to have common data points in mind. Why did these overlaps happen? What might they mean?

As you sift through your data to develop your ideas and arguments, it may help to open many notes at once so that you can quickly refer to each.

[

### \# Conclusion

](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/#conclusion)

That’s all! I will include this write-up in the kit itself.

[

## \# Changelog

](https://fulcra.design/Posts/An-Integrated-Qualitative-Analysis-Environment-with-Obsidian/#changelog)

-   August 11, 2021: I have open-sourced the environment. [Find and contribute to it on GitHub!](https://github.com/ryanjamurphy/obsidian-qualitative-analysis-environment)