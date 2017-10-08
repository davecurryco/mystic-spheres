# WikiPack User Guide

**Version 1.7, Dec 2012**

WikiPack is designed to be simple & intuitive to use, and as such you should be able to jump in and skip the whole _RTFM_ step, so this guide covers more in-depth aspects of the system for those looking for a deeper understanding.

## Changelog

* **Version 1.7** - Added todo lists!
* **Version 1.6** - Added the ability to insert wiki links to other pages with autocomplete
* **Version 1.5** - Added a default homepage
* **Version 1.4** - Added auto-linking of pasted URLs
* **Version 1.3** - Added the ability to mark pages as favourites, and browse a list of all of your wiki pages from the sidebar
* **Version 1.2** - Added the ability to change your Dropbox folder for existing accounts
* **Version 1.1** - Added the ability to edit pages using the keyboard shortcut Control/Command-E

## Default homepage

You can specify a default homepage for your wiki that will be immediately accessible from any page by clicking on the home icon in the menu bar, and will also be the page that loads automatically whenever you log into your wiki.

### Setting your home page - from the pages index

When viewing the list of all the pages in your wiki, you can click the home icon on the far right of the row for the desired page.

### Setting your home page - when viewing a page

When viewing a particular page, just click the home icon in the top right of the page to set it as your homepage.

## Dropbox Sync

Dropbox sync happens transparently and shouldn't concern you most of the time, but there are some situations where you may be interested in how to make it work to suit your needs.


### Uploading changes made with WikiPack to Dropbox

Dropbox sync takes place automatically whenever you save an edited page through the WikiPack web interface,  which will be evident by the spinner animation that appears on the sync button in the sidebar, and the absence of the other action buttons. When your changes have been uploaded to Dropbox, the sidebar buttons will return to normal but you don't have to wait for the sync operation to complete before navigating away to another wiki page, or even closing the browser window.

### Importing changes from Dropbox back into to WikiPack

One of the main reasons for adding Dropbox sync to WikiPack is to allow you to work on your documents with other applications. It may not be apparent to you how to import those changes back into your wiki though. It's fairly simple, but can be done in one of two ways:

* **Updating a specific page**
    * Navigate to the page which has been edited on Dropbox and hit the **Sync** button in the sidebar
    * WikiPack will update the page with the latest version from Dropbox
* **Updating all of your pages together**
    * If you've edited several files it could be tedious updating each one individually, so you can update all of your pages at once by using the **All Pages** button to go to your pages index, and hitting the **Sync** button in the sidebar. Any pages with changes on Dropbox will be updated to the latest version

**Tip:** To add new pages to your wiki using an external app:

* Edit an existing page on WikiPack with a link to the new page _(which doesn't exist yet, but that's OK)_
* After saving the page, click the link to open the New Page interface
* Give the page a heading _(like `# My page heading`)_ and save it
* Once the page has synced to Dropbox, you can open it in another app to compose your document
* When done editing, return to the page on WikiPack and hit the **Sync** button to import your changes from Dropbox. _(That's how this very document was created; on an iPad using Writing Kit)_

### Deleting pages

When you delete a page from WikiPack, it is also removed from your Dropbox folder. This can be undone by visiting the Dropbox website and using the provided controls for restoring deleted files if needed.

If you delete a page from Dropbox, it will still appear in your wiki until the next time you sync your pages index _(go to All Pages, hit Sync)_, at which point edited pages will be updated, new pages will be imported, and deleted pages will be removed from your wiki.

### Renaming pages

When you rename a page on WikiPack, it is also renamed in your Dropbox folder, but Dropbox achieves this by essentially deleting the original file, and creating another file with the new name. _(Just to explain why Dropbox notifies you of two file changes when renaming a file, in case you were wondering.)_ The renamed file will retain your edit history however.

If you renamed the file on Dropbox directly, or with another app, rather than manually renaming the old page _(which no longer exists on Dropbox and will cause an error)_, please sync your pages index by going to All Pages and hitting the sync button.

#### Maintaining wiki links

If you want to rename a page but have already linked to it from other pages, don't worry, WikiPack will update the links _within those pages_ accordingly to maintain your wiki structure. It will show you which parent pages are going to be updated, and you may notice several pages syncing with Dropbox after renaming just one page.

#### A note on Windows invalid characters

Dropbox is intended to be used as a cross-platform cloud storage system, but different devices and operating systems enforce different constraints on the characters that are allowed in filenames. To compound the issue, the Dropbox API does not restrict which characters can be used to _create_ files, but does when _renaming_ files, and unfortunately one such character is the colon : as used extensively by Trunk Notes.

There is a work-around as employed by Trunk Notes, but as of yet _(April 2012)_, WikiPack will give an error when attempting to rename a file that contains colons or other "Windows invalid characters".

### Page history

Whenever you edit a page, it saves your changes as previous versions. You should feel empowered to fearlessly hack at your Markdown pages, because worse comes to worst, you can always revert your changes back again. That's the idea anyway.

#### Viewing & restoring previous versions of a page

To access your page history, hit the **History** button in the sidebar to bring up a list of previous versions of the page displayed by date. Click on a previous version to view the page as it was at that point in time. To revert the current version of the page back to that version, use the revert link at the top of the page.

#### Comparing different versions of a page

Sometimes it's handy to have a visual representation of the changes that you made to a page. WikiPack allows you to compare two different versions of a page, for example the current version with the first version, the current version with the previous version prior to the last change, or any two earlier versions.

It renders the Markdown as HTML with additions highlighted in green, and deleted sections highlighted in red.

**Note:** this technique does not display changes to the Markdown that don't affect the rendered HTML, such as whitespace.

 To compare two versions of a page:

* Use the **History** button in the sidebar to display a list of previous versions of the page
* Click the check-box next to the two versions you want to compare and press the **Compare** button

### Changing your Dropbox wiki folder

If you let WikiPack create the default wiki folder for you when signing up but later wish to hook WikiPack up with another folder on Dropbox, or you simply wish to use a different folder for whatever reason, you can do so using the "change wiki folder" function in the account settings page.

1. Go to the **account settings** page _(by clicking on your user name in the top right corner)_
2. Click the **"Change my Dropbox folder"** button in the sidebar
3. Confirm that you want to change your Dropbox folder
	1. WikiPack will remove the existing pages from your wiki, but not from Dropbox; they will be left intact in your current wiki folder
4. Select the new Dropbox folder to use
	1. WikiPack will then import the Markdown files from that folder into your wiki

The initial import may take some time if you have many files in your Dropbox, but should complete quickly for most people.

## Markdown Editor

WikiPack provides a great web Markdown editor with syntax highlighting, smart auto-completion, and keyboard shortcuts. Most of it's functionality should feel completely natural and familiar to you if you've used dedicated Markdown editors like Byword or iAWriter.

### Editing a page

To load the Markdown editor while viewing a page, either click the **Edit** button in the sidebar, or use the keyboard shortcut **Control-E** on Windows/Linux, **Command-E** on Mac.

### Toolbar buttons & functions

The editor tool-bar provides icons for various functions, some of which have a corresponding keyboard shortcut, and some of which act differently depending on whether there is selected text or not.

All keyboard shortcuts use the OS-specific modifier key: COMMAND for Mac OS X, or CTRL for other operating systems.

#### Headings

The **Heading** button which clicked, inserts a `#` at the front of the current line, marking it as a heading. Subsequent presses insert more `#` characters, turning it into a sub-heading. To undo, either used the undo button/keyboard shortcut, or hit backspace/delete.

* **Keyboard shortcut:** COMMAND/CTRL-H

#### Bold & Italics

Bold and italics work much as you'd expect - select a word/phrase and hit the tool-bar icon or use it's keyboard shortcut to delimit it with the appropriate Markdown. Alternatively, you can hit the bold/italic button while typing to have the delimiter characters inserted and the cursor positioned between them.

WikiPack uses double asterixes for bold, and a single underscore for italic, but _who's with me in thinking that it would be more intuitive for Markdown to have used:_ 

    *bold*, /italic/, _underline_, -strike-through-`?

* **Keyboard shortcut:**
    * **Bold:** COMMAND/CTRL-B
    * **Italic:** COMMAND/CTRL-I

#### Bulleted & numbered  lists

The bulleted & numbered list buttons act on the current line by first turning it into a list item, and then indenting it with subsequent presses. You can also use the TAB key to indent, and SHIFT-TAB to un-indent.

When hitting enter at the end of a list item, it will maintain the indentation and also the Markdown delimiter _(`*` for bulleted lists, and an incremented numeric counter for numbered lists)_. Hitting it again on a blank list item will un-indent the line until it reaches the left margin, at which point the list delimiter will be replaced with a blank line, exiting out of list mode. When changing the indentation of numbered list items, it recalculates the numeric counter for you. This works in the same fashion as you'd be accustomed to in a word processor.

* **Keyboard shortcut:** _none_

#### Todo lists

WikiPack treats "hyphenated lists" as todo lists, rendering each item in the list with a clickable checkbox which toggles a `@done` tag on that item and updates the page. The `@done` tags are timestamped with the current date, but the timestamps are optional.

Todo lists behave in the Markdown editor in much the same way as bulleted and numbered lists in terms of creating and editing the lists. When saving the page however, the list will be rendered with checkboxes for each item. Todo items can be indented in the same way as bulleted & numbered lists, and they support in-line Markdown like **bold**, *italics*, `code snippets`, links, etc.

* To create a todo list, edit any page and either click the todo list icon button in the tool bar, or begin a list using the "-" delimiter. 
    * Currently, the only way to **add** or **delete** todo items is by editing the page
* Save the page to see the list rendered with checkboxes
* To mark an item as done:
    * Click on its checkbox, or on the item itself
    * Todo items can also be marked as done when editing the page by using the keyboard shortcut COMMAND/CONTROL-D to insert a `@done` into the item with an automatic time-stamp

#### Links & images

The link and image buttons behave in much the same way, with the exception of images asking for an additional alt-text field. You can either select existing text and then hit the buttons, or just position the cursor and then hit the button to have it prompt you for the text to be entered.

Both will prompt for a URL to the external website or image, while the image button will also prompt for an "alt-text" field _(a title for the image)_.

* **Keyboard shortcut:** Command/Control-V _(see below)__

##### Pasting URLs into links/images

When you paste a URL into a page, WikiPack will prompt you to turn it into a link. If you had text selected, it will use it for the link text, otherwise it will prompt you to enter the text.

It's also smart enough to distinguish between links to web pages and URLs to image assets, and will insert a Markdown image accordingly.

* **To quickly turn some text into a link:**
    1. Copy the destination URL to the clipboard
    2. Select the text to be used for the link
    3. Paste the URL into the page, and confirm that you want to turn the selected text into a link
* **To quickly insert a Markdown image:**
    1. Copy the URL of the image to the clipboard
    2. Paste it into the page
    3. Confirm that you want to turn it into a Markdown image, and enter the alt-text for the image _(any descriptive title, or just "image" or "pic" for lack of inspiration)_

If you wish to paste a raw URL into the page without auto-linking it, just hit the escape key when the dialogue box appears.

#### Wiki Links

The Wiki Link button can be used to quickly insert a link to another wiki page. It will open an auto-complete text field where you can enter the page name and choose the page to which you wish to link.

You don't need to specify the link text if you don't want, just hit enter to insert the page name into the link as-is.

#### Quotes & code blocks/snippets

These buttons behave differently depending on whether there is selected text or not. The quote button does nothing while text is selected, while the code button switches between snippet mode with an selection, or block mode with a block selection or no text selected.

##### Quotes

Quotes are rendered as HTML as followed:

> Lorem ipsum dolor sit amet

This is achieved by delimiting the line with a preceding `>` character. Quotes can be nested by prefixing the line with several `>` quote characters, but there are some issues with whitespace and multiple nested levels that WikiPack takes care of for you as you type. For example:

This could be achieved by simply using the Enter and TAB keys intuitively, while WikiPack inserts double whitespace at the end of each line to instruct Markdown to honor the line-breaks, and inserts a blank line between each nested quote level:

> A top-level quote  
> That spans several lines  
> While maintaining line-breaks
> 
> > A nested quote  
> > That also maintains line-breaks
> 
> > > Nested three levels deep  
> > > Same deal with the line-breaks
> 
> > Back to the  
> > Second level
> 
> Back to the top level

* **Keyboard shortcut:** _none_

##### Code snippets

Code snippets are used for inserting code in-line like this: `collection.each {|thing| puts thing}` or this: `<strong>emboldened text</strong>`, and are achieved using the back-tick character _(which is on the same key as the tilde ~ on most keyboards)_. Select a code snippet within a line and hit the code button to have it wrapped in back-ticks for you.

* **Keyboard shortcut:** _none_

##### Code blocks

Code blocks are used to insert several lines of code, and are achieved by simply inserting 4 spaces _(or two tabs, depending on how you roll)_ before each line:

    10 print "Darren is a n00b"
    20 goto 10

Simply select a block of code and hit the code button, or just hit tab twice.

* **Keyboard shortcut:** the TAB key can be used to indent code blocks manually

#### Undo

The global ubiquitous undo keyboard shortcut, COMMAND/CTRL-Z is recognised, but there's also a tool-bar button that does the same thing.

* **Keyboard shortcut:** COMMAND/CTRL-Z

## Linking your pages together into a private wiki

To make the most of the "wiki" in WikiPack, you can simply insert **WikiWord** links into your pages to link them together and organise them however you like. The template wiki provides a few pages to get you started, like HomePage, Inbox, and Todo pages, but you can create as many pages as you like, and link them together as you see fit.

### What are WikiWords?

WikiWords are simply a title-case phrase with no spaces separating the words, for example: `ThisIsAWikiWord`. WikiPack generates the WikiWords for you automatically from your filenames. For example, a file named `My awesome file of awesomeness.markdown` would be given a WikiWord of `MyAwesomeFileOfAwesomeness`.

To add a link to this page, you would use this WikiWord in one of two ways:

* **Simple wiki links:** the rendered link simply shows the WikiWord
    * Wiki link: `[[MyAwesomeFileOfAwesomeness]]`
    * Renders as: [MyAwesomeFileOfAwesomeness](#)
* **Custom link text:** the rendered link is customised
    * WikiLink: `[[MyAwesomeFileOfAwesomeness|my awesome page]]`
    * Renders as: [my awesome page](#)

### Using wiki links to create pages

There is a lovely shiny **New Page** button in the sidebar, but personally I create new pages by first editing an existing page with a link to the page I want to create, and then clicking the link I just added to create the page. That way I don't end up with "orphaned pages", pages with no inbound links.

I have a HomePage that links out to landing pages for my various projects & areas of interest, so I'll usually start by editing one of those pages to add the link, often formatted like:

    **29-04-2012** - Creating a page about [[InterestingPage|something interesting]]

I also sometimes preempt that I might one day  create a page about something I'm writing about, and insert a link to it but not create the page immediately. If at some point I do create the page, and following my personal naming convention manage to use the exact same WikiWord, the pages will be automatically linked together for me already, giving a pleasant surprise. For example, I might write:

    Had some trouble today with my [[WiFiRouter|WiFi router]], but fixed it with a software update.

I may not need to create a page for it at that time, but might come back at a later time and create the page, and the two pages would already be linked together for me.


### A note on filenames & wikiwords

I know that many of you use WikiPack with the excellent iOS _(and soon Mac!)_ application **Trunk Notes**, which uses a WikiWord naming convention for its filenames. Not _everyone_ uses WikiPack with Trunk Notes however so it doesn't enforce this naming convention, but if you create a page in WikiPack and want it to be imported into Trunk Notes, please use a WikiWord for the filename.

### Searching & navigating your wiki

There are two schools of thought on how to best store & retrieve data: those who like to label, sort, and categorise their data into a carefully structured hierarchy, and those who prefer to keep their data in a flat structure and rely on search tools to retrieve it.

WikiPack doesn't currently support subdirectories within your wiki folder, but it does provide a fast and powerful search box for quickly jumping between pages, and searching the contents of your pages. It also allows you to mark your most frequently used pages as favourites for quick access from anywhere.

#### Jumping between pages

You can access the search box in most browsers by simply hitting the TAB key, and then beginning to type a page's **WikiWord**. For example, to quickly jump back to your home page from anywhere in your wiki, just hit TAB then start typing "home". The search box will auto-complete as you type, and may only require the first couple of letters. It highlights the top result, and will take you straight to that page as soon as you hit the enter key. You can use the up/down arrow keys to select different search results, and the enter key to jump to that page.

I use this method for navigating my wiki more than following the wiki links between pages usually, but there are other means of jumping between pages using the mouse, such as a list of every page in your wiki that you can scroll through manually, and a list of your favourite pages in the sidebar.

##### Favourites

The sidebar contains three panes:

* **TOC** - table of contents
* **Pages** - a list of every page in your wiki
* **Faves** - your favourite pages

While viewing a page, click the star icon in the top right to mark it as a favourite. It will then be accessible from the Faves pane when viewing any page in your wiki. The sidebar will remember which pane you have selected for the duration of your logged in session, so you can quickly jump between pages in your Pages/Faves lists.

#### Searching within the contents of your pages

It's good proactive to follow a naming convention when creating & organising your pages, but if you're like me you'll still occasionally forget _which page_ you wrote something in and won't be able to find it by WikiWord. To search within your pages for a matching string, select the search box by hitting the TAB key, and type in a word or phrase that you're looking for. When no auto-complete results are selected, hitting enter will perform a wiki-wide search for **an exact match** of the entered string.

Note that it doesn't yet support full-text search _(the ability to find partial matches, or to perform Google-like searches such as "Markdown editor iOS". Google might return a page containing "My favourite Markdown editors for iOS", but WikiPack currently will only match exactly "Markdown editor iOS" as of April 2012)_

## Markdown tables

You can use [PHP Markdown Extra](http://michelf.com/projects/php-markdown/extra/#table) table syntax:

    Table syntax:
    First Header  | Second Header
    ------------- | -------------
    Content Cell  | Content Cell
    Content Cell  | Content Cell

Alternatively, using optional leading & tailing pipes:

    | First Header  | Second Header |
    | ------------- | ------------- |
    | Content Cell  | Content Cell  |
    | Content Cell  | Content Cell  |

### Aligning columns

You can specify alignment for each column by adding colons to separator lines

* A colon at the **left** of the separator line will make the column **left-aligned**
	* _the default for no colons is left-aligned_
* A colon on the **right** of the line will make the column **right-aligned**
* Colons at **both sides** means the column is **center-aligned**

#### Right aligned

    | Item      | Value |
    | --------- | -----:|
    | Computer  | $1600 |
    | Phone     | $12   |
    | Pipe      | $1    |

Renders as:

| Item      | Value |
| --------- | -----:|
| Computer  | $1600 |
| Phone     | $12   |
| Pipe      | $1    |

#### Center aligned

    | Item      | Value |
    | --------- |:-----:|
    | Computer  | $1600 |
    | Phone     | $12   |
    | Pipe      | $1    |

Renders as:

| Item      | Value |
| --------- |:-----:|
| Computer  | $1600 |
| Phone     | $12   |
| Pipe      | $1    |


## Contact & support

If you have any questions, comments, or feedback, please get in touch:

* **Email:** info@wikipackit.com
* **Twitter:** @wikipack

