THIS IS AN UNCONNECTED FORK OF _Programming Historian_ (<http://programminghistorian.org>) MADE AS PART OF THE COLLABORATIONS WORKSHOP! PLEASE DO NOT REFER TO THIS AS OFFICIAL OR FINISHED FOR NOW !!!!

## Technical notes for administrators/maintainers

### How to add new lessons for translations

Each lesson has a separate repository in the
[GitHub organisation for Programming Historian internationalisation](https://github.com/orgs/programminghistorian-i18n). Initially this repository stores the latest original English version
of the lesson, uploaded to transifex (with a commit message referring to
the respective commit in the [Programming historian website](https://github.com/programminghistorian/jekyll/)
and has a copy of the LICENSE under which the lesson is distributed
(it will be necessary to link this license when creating a project
in Transifex), and a README explaining the purpose of this repository
(in particular, it should indicate that one should not submit issues and
PRs regarding the content of the lesson). Later, this repository might
also have intermediate versions of translations downloaded from Transifex,
for the preview of their rendered versions on the testing website
https://github.com/programminghistorian-i18n/jekyll_new/, with the intention
that after the review of a particular translation is completed, it is
submitted via a pull request to the official [Programming historian website
repository](https://github.com/programminghistorian/jekyll/).

Note that this intermediate repository will allow us to fix versions of
files uploaded/downloated to/from Transifex, which (as it seems) lacks
versioning information. This setup also allows to interact with the official
[Programming Historian website] and its possible forks via files, and
therefore will not be impacted, for example, if Programming Historian
will reorganise its site and move each lesson into a separate repository.

## Administrator's Guide:

The administrator's workflow to add a new lesson for translation:

1. Create a lesson repository
2. Populate it with: 
    - README: see a template (TODO)
    - License: all submissions to Programming Historian are published
      under a [Creative Commons ‘CC-BY’ license](https://creativecommons.org/licenses/by/4.0/deed.en)
    - the `.md` file with the lesson, copied from the
      [Programming historian website](https://github.com/programminghistorian/jekyll/)
3. Create a corresponding translation project in Transifex
4. Upload the `.md` file with the lesson as a resource for translation
   (see [documentation](https://help.transifex.com/en/articles/6236812-uploading-content-for-translation))
6. Notify translators and reviewers that they may start their work

## Editor's Guide:

When there is a version of the translation ready for preview:
1. Download it from Transifex
2. Commit to the lesson translation repository
3. Duplicate it in the appropriate location on the testing 
   website https://github.com/programminghistorian-i18n/jekyll_new/

When there is an approved version of the translation:
1. Repeat, if necessary, steps 1-3 from the previous section
2. Edit the header in the `.md` file with the lesson to add
   details of the translators and translation reviewers (can
   be done at a preview step too)
3. Submit a PR to the
   [Programming historian website repository](https://github.com/programminghistorian/jekyll/)

When there is an updated English version of the lesson:
1. DO NOT upload it to Transifex without agreeing this with
   the team working on thatr lesson's translation - do it
   only by an agreement, since this will 


## Translator's Guide:

Since Transifex is already used for a similar internationalisation
project by the Carpentries, whose lessons also use Markdown, at the
first step we can refer to their [Translator Guide](https://carpentries-i18n-handbook.readthedocs.io/en/latest/guide/translator/index.html). See
also a blog post [Top tips for translating open education resources](https://www.software.ac.uk/blog/2022-05-26-top-tips-translating-open-education-resources) by David Pérez-Suárez (UCL) on the
[Software Sustainability Institute](https://www.software.ac.uk/) website.

For the Ukrainian translation, Olexandr will be able to demonstrate
Transifex and provide further training and support, based on [their
experience with translating the Carpentries](https://olexandr-konovalov.github.io/posts/2023/03/28/carpentries-translation/).


