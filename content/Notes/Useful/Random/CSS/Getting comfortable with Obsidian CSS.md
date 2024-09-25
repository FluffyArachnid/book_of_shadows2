[[ReadItLater]] [[Article]]

# [Getting comfortable with Obsidian CSS](https://forum.obsidian.md/t/getting-comfortable-with-obsidian-css/133)

While using Obsidian, if you press CTRL-SHIFT-I (option-cmd-i for mac) then it will bring up the developer window. In the developer window, at the top left is an icon with a pointer in a box. This allows you to select elements on the screen and see how to refer to them and what styles. I will occasionally update this post with more pictures of how to do stuff.

[![Developer Tool](https://forum.obsidian.md/uploads/default/optimized/1X/f2a25eac6be2a49339c99f542d8096dddcd045f8_2_443x499.png)](https://forum.obsidian.md/uploads/default/original/1X/f2a25eac6be2a49339c99f542d8096dddcd045f8.png "Developer Tool")

You can hover over items to see what they do and then click on an item to select it. Then go down to the styles section at the bottom of developer tools and scroll through the classes and styles invovled.

[![Element Inspector Tool Hover](https://forum.obsidian.md/uploads/default/optimized/1X/4c1b2a2a24eb62cbfa705f19fb4fce238dca97b3_2_518x500.png)](https://forum.obsidian.md/uploads/default/original/1X/4c1b2a2a24eb62cbfa705f19fb4fce238dca97b3.png "Element Inspector Tool Hover")

You can force elements into states to see what selectors to use for adjusting the CSS for that state.

[![Element Inspector Tool Select State](https://forum.obsidian.md/uploads/default/optimized/1X/6b0a727796d90f6688a713b779e084bdb4c9e5f0_2_351x500.png)](https://forum.obsidian.md/uploads/default/original/1X/6b0a727796d90f6688a713b779e084bdb4c9e5f0.png "Element Inspector Tool Select State")

You can see the different selectors [here](https://forum.obsidian.md/t/common-selectors/1984)

98 Likes

I’d just like to add that if you use the same classes that are specified in the app.css then most of the time you won’t need to use `!important`

For example, if you try to change the colour of `code`, it won’t work unless you add `!important`  
But if you use the inspector you’ll find that the colour of code in the preview is set by the rule `.markdown-preview-view code`. And if you use that rule, you won’t need to use `!important`  
![image](https://forum.obsidian.md/uploads/default/original/1X/a34ace710472771683693bbaf5a1b75a7ead464a.png)

11 Likes

The developer window looks like an amazing tool!

When you fill out this tutorial more, can you elaborate on how one might use it to follow through and make a change to their obsidian.css? There are so many unanswered questions here.

To give you some insight on your audience, I’m a curious noob who’s interested in learning to customize but also doesn’t want to accidentally break Obsidian. Here’s an example of what goes through my mind as I look at your post.

Say I want to adjusts how far bullet lists are indented. I open the developer window, use the select element pointer to pinpoint an element. And then I can see several references to what I’m focusing on.

There’s an Elements window that highlights this:  
`<ul style="padding-left: 40px;">`  
There’s a Styles window that highlights this:  
`element.style { padding-left: 40px; }`  
Maybe there are more pieces of relevant information, but how do I know?

There’s a lot of other stuff that doesn’t seem related at all. But it’s hard to tell. The window looks cluttered with a lot of accidents waiting to happen if I do something wrong.

I cautiously proceed I find that I can change 40px to 18px and that looks great to me. And I also feel like I could easily break something important if I type in the wrong spot. All mentions I’ve seen for the developer window talk about it pretty casually. But it also feels like I’m irreparably screwing things up in there. Is it a sandbox to expore ideas or am I actually screwing things up? Is there a way to revert what I’ve done? I don’t see the app.css file anywhere in my vault.

What are the right pieces of information to be looking at?  
How do I know that I’ve found the information I need to make a system wide customization?  
How do you tie it together? What’s the next step?

I sense that this would be a super simple modification to my obsidian.css file. But I still don’t know what I should bring from this window to the obsidian.css to file to make that happen.

Please consider these questions, practicalities, and perspectives as you elaborate on this tutorial.

Thanks!

17 Likes

You make some good points here [@goodsignal](https://forum.obsidian.md/u/goodsignal), so I’d just like to clarify some of it for you.  
Firstly, I don’t think anything in css can break the app or your notes. Css is just presentation and can’t really affect any data. So feel free to experiment! Go nuts!  
If you’ve been playing around with the css in the dev tools and gotten lost and things look broken or wrong, a quick reload (ctrl+r I think) or closing and opening Obsidian should fix it.  
If you mess up your obsidian.css you can always delete or replace it.

As for transferring your changes to your obsidian.css so that they stick, this is where you start learning about css rules and things get tricky. In general you can copy the rules from the styles panel which you change.  
It’s a little more complicated than that, though. Css rules and selectors and classes is a whole topic. When starting out, it’s probably best to try and copy what’s there.

This obviously is not all you need to know. For instance with your indentation example, the css is on the element itself, and not actually part of the css rules. This makes it difficult to style. You’ll have to figure out what rule applies to that element and then also mark any styles you create as `!important`.  
CSS rules apply in order of what is most specific, and anything in the “styles” section of an element is *most* specific, with !important being a hacky override.

This is just scratching the surface, but hopefully it’s enough to get started…

8 Likes

[s0ph0s](https://forum.obsidian.md/u/s0ph0s) May 25, 2020, 2:31pm 6

Question: would it be possible to have a place in the preferences to override the existing CSS code, across whatever file is currently loaded? I recently noticed this in [Brett Terpstra’s Marked](https://marked2app.com/):

[![marked style prefs](https://forum.obsidian.md/uploads/default/optimized/1X/82cd8085d734a26d8d3927121001a1fe4d81eef0_2_351x500.png)](https://forum.obsidian.md/uploads/default/original/1X/82cd8085d734a26d8d3927121001a1fe4d81eef0.png "marked style prefs")

[![marked style prefs 2](https://forum.obsidian.md/uploads/default/optimized/1X/c57da1f02255ed13ca3c89ebba958e9d17bf6344_2_351x500.png)](https://forum.obsidian.md/uploads/default/original/1X/c57da1f02255ed13ca3c89ebba958e9d17bf6344.png "marked style prefs 2")

4 Likes

I really appreciate your feedback [@death.au](https://forum.obsidian.md/u/death.au). Thanks!

[@s0ph0s](https://forum.obsidian.md/u/s0ph0s) obviously I’m not well versed in this, but I’m pretty sure the CSS Plugin in Settings and corresponding obsidian.css file is the Obsidian equivalent override that you’re seeking.

[s0ph0s](https://forum.obsidian.md/u/s0ph0s) May 25, 2020, 4:18pm 8

So the obsidian.css file can be layered on top of another theme and not replace it? If so, that’s fantastic.

Oh I see what you were aiming for now. No, just have to add whatever changes you want to that file.

[Silver](https://forum.obsidian.md/u/Silver) May 25, 2020, 9:10pm 10

CSS rules have specificity, even if rule 2 comes after rule 1, if rule 1 is more specific, it will win.

Therefore, unless we’re talking about two rules that happen to be the same specificity, it shouldn’t matter in what order you use them.

If you would prefer theme 2 to override theme 1 though, it’s a good idea to append `theme2.css` at the bottom of `theme1.css` instead of the other way around.

5 Likes

[s0ph0s](https://forum.obsidian.md/u/s0ph0s) May 25, 2020, 9:38pm 11

Understood. I was thinking it would be ideal to have an extra snippet of code that could override all future imported css themes to customize them quickly to the user’s liking.

For example, if I want to use @random\_new\_contributor’s new theme, but I want my small code snippet to always override a particular part of any new theme I use, my add-on snippet would take precedence. Almost like a permanent `!important` attribute that overrides everything else. Probably not an issue for most people, I suppose.

4 Likes

[echej](https://forum.obsidian.md/u/echej) May 26, 2020, 1:49am 12

Really like this idea, I usually used this way to tweak themes in jekyll ![:wink:](https://forum.obsidian.md/images/emoji/apple/wink.png?v=12 ":wink:")

[death.au](https://forum.obsidian.md/u/death.au) May 26, 2020, 11:03pm 13

Here’s a trick I worked out for inspecting the styling of popovers:  
If you bring up the developer tools, go to the “sources” tab, hover over a popover so it appears then press `F8` the javascript will pause so the popover won’t disappear until you tell it to resume.

While it’s paused, you can still inspect elements and fiddle with the css, but obsidian will generally remain unresponsive until you resume by clicking the button or pressing `F8` again

2 Likes

Also from [@death.au](https://forum.obsidian.md/u/death.au), how to handle dark and light elements in your CSS

a) Create a CSS variable for your colour in .theme-light and .theme-dark blocks and use that variable where you need it:

```
.theme-dark {
  --title-color: black;
}
.theme-light {
  --title-color: white;
}
.view-header-title {
    font-size: 22px;
    color: var(--title-color);
} 
```

Or b) you can just add .theme-light or .theme-dark to the start of your selector:

```
.view-header-title {
    font-size: 22px;
}
.theme-light .view-header-title {
    color: white;
}
.theme-dark .view-header-title {
    color: black;
} 
```

4 Likes

[death.au](https://forum.obsidian.md/u/death.au) May 26, 2020, 11:28pm 15

Thanks. I prefer the variable method, myself because you can use the variable in multiple places and just tweak the colour in two.

But the latter approach is equally valid and could be useful in some cases (say if in dark mode the text needed to be bolder to stand out)

1 Like

[ksandvik](https://forum.obsidian.md/u/ksandvik) May 26, 2020, 11:52pm 16

A global user.css file that overrides specific elements would be a nice thing, other Markdown tools such as Typora has this as well. Sometimes it’s a small thing like larger `font sizes.`

3 Likes

Keyboard shortcut to bring up developer window on Mac with Obsidian v0.6.7 is Alt-Cmd-I.

2 Likes

Is there a starter template or similar to use when developing a new theme? Or is it normal to just start with an empty `obsidian.css` file?

3 Likes

Normal to start with empty CSS file. I think someone may be working on documentation that includes that. But it may be awhile because the program is in early development. I’d recommend checking out the Hulk theme, I believe they have the code laid out nicely to edit it the way you want.

2 Likes