README
======

Wolf-PAC Georgia Wiki
---------------------

This wiki is built on [MDWiki](http://mdwiki.info). Below is a cut down version of the base README with added instruction for users of the web interface.

First things first
------------------

Learn [Markdown](https://help.github.com/articles/github-flavored-markdown)! Then check out MDwiki's [quick start](http://dynalon.github.io/mdwiki/#!quickstart.md).

File Structure
--------------

_All file references here are relative to their respective language folder._

| Name | Type | Description |
| :--- | :--- | :--- |
| `index.md` | File | Starting point (a.k.a. "home page") for your wiki. **Note this is not the `index.html`, but `index.md`**! |
| `navigation.md` | File | Various settings of your wiki (e.g., name of your wiki, items in the navigation bar at the top, etc.) |
| `config.json` | File | If you don't know what this is for, don’t touch it. |
| `pages` | Folder | Ideally, inside this folder, you create one `*.md` file for every page inside your wiki (e.g., `foo.md`, `much-longer-names-are-also-okay.md`, etc.) You can also create as many subfolders as you need, just remember to link them accordingly. |
| `uploads` | Folder | An example folder structure where you could put other files. **Although it is best to host your files somewhere else, like Dropbox, or a CDN, etc.** |

How to Update the Wiki
======================

Use of this particular wiki is presumed to be primarily through GitHub's web interface for working with repositories. All content should be placed underneath in [pages/](https://github.com/wolf-pac-georgia/wolf-pac-georgia-wiki/tree/gh-pages/en_US/pages). Follow that link to get started.

Creating an Article
-------------------
Click the "Create new file" button in the top right. You will be presented with a text box to fill in the name of the article, and a larger editor below, where you will write the article content using Markdown formatting.

NOTE: In order to create a new directory, type the name in the box for the file name, followed by a '/', then the article name. It is not possible to create an empty directory here, as it is created at the same time as the file.

Previewing Changes
------------------
The "Preview changes" tab in the editor will let you see what the formatted text looks like, before you commit it. However, since the MDWiki software adds its own styling to the pages, this will not be a perfect representation of the end result. Additionally, if you are editing a document, it will show more than just the final content (see below).

Committing Changes
------------------
Not unlike most wikis, it is required that you commit changes with a descriptive message, which is done in the box below the text editor. You should not need to change any of the fields beyond the commit message. Once you have added that, click the commit button to finish.

Editing / Deleting
------------------
Editing works much the same as adding a new file, the only difference is you first click on the file you want to change, then click the pencil icon in the top right.

The delete button is right next to that, represented by a trash can icon. Deletions are also done via the same commit structure as the other operations.

NOTE: The "Preview changes" functionality in these modes will show you ALL changes from the previous version, which includes deletions (indicated by a red color in the margin). This is just a consequence of how GitHub is designed to be used, which is.. not exactly what we are doing here, but it works. :)


Best Practices
--------------

### Relative URLs

Instead of using absolute URLs when linking one wiki page to another, use relative URLs.

For instance if `en/pages/foo.md` page had to link to `en/pages/bar.md`, it is enough to just add `[Click here](bar.md)` in your markdown.

### Don't Host Your Uploads in Git(Hub)

Instead of hosting your uploads inside an `uploads` folder, consider using Dropbox, Google Drive, or a CDN.

### Add References to Uploads

**Whenever you can, avoid hosting your uploads using Git(Hub).**

If you _must_ add references to files hosted inside the `uploads` folder here's how to do it, for instance: `![Image Title](uploads/images/foo.png)`. Add that in your markdown and you're good to go.




