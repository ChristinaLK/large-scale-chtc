Computing At Scale (Template Lesson)
==============

This repository contains a customizable template for 
an introductory training on using a large scale 
computing resource, based on this [lesson template][github].  

> Disclaimer: While this template uses the [Software Carpentry][swc] 
and [Data Carpentry][dc] lesson template, it is in no way affiliated 
with or endorsed by these organizations, and is not considered part 
of either organization's official scope or curriculum.  Any instructor 
or trainer can use this material at their own discretion.  

## Customization Instructions

1.  Do *not* fork this repository directly on GitHub.
    Instead, 
    > add import instructions

2.  Edit the following files and values: 
    > _yaml, title, intro text on first page, includes in `_episodes/custom` dir, figs

3.  See layout/formatting below for more info.  

4.  Commit changes to the gh-pages branch.  Push a copy to repsitory on github
    [automatically published as a website by GitHub][github-pages].

5.  To preview material,
    please run `make serve` from the command line
    to launch Jekyll with the correct parameters,
    or push to your repository's `gh-pages` branch
    and let GitHub take care of the rendering.

6.  Run `make lesson-check` to check that your files follow our formatting rules.
    For a list of other helpful commands run `make` in this directory.

7.  If you find an error or omission in this documentation,
    please [file an issue in this repository][example-issues].
    If you find an error or omission in the lesson template,
    please [file an issue in the styles repository][styles-issues] instead.

## Layout Overview

The layout of this repository is explained in [this site's episodes][rendered].
In brief:

1.  The source for pages that appear as top-level items in the navigation bar
    are stored in the root directory,
    including the home page (`index.md`),
    the reference page (`reference.md`),
    and the setup instructions (`setup.md`).

2.  Source files for lesson episodes are stored in `_episodes`;
    `_episodes/01-xyz.md` generates `/01-xyz/index.html`,
    which can be linked to using `/01-xyz/`.

4.  Files that appear under the "extras" menu are stored in `_extras`.

5.  Figures are stored in the `fig` directory,
    data sets in `data`,
    source code in `code`,
    and miscellaneous files in `files`.
    
## Formatting overview

1.  Markdown, links, link to gh-markdown

2.  Callouts, challenges, checklists, prereq, solutions

[collections]: https://jekyllrb.com/docs/collections/
[dc]: https://datacarpentry.org
[editing-config]: https://swcarpentry.github.io/lesson-example/03-organization/
[example-issues]: https://github.com/swcarpentry/lesson-example/issues/
[github]: https://github.com/swcarpentry/lesson-example/
[github-pages]: https://help.github.com/articles/creating-project-pages-manually/
[issues]: https://github.com/swcarpentry/lesson-example/issues
[rendered]: https://swcarpentry.github.io/lesson-example/
[setup]: https://github.com/swcarpentry/lesson-example/blob/gh-pages/setup.md
[styles-issues]: https://github.com/swcarpentry/styles/issues/
[styles]: https://github.com/swcarpentry/styles/
[swc]: https://software-carpentry.org
