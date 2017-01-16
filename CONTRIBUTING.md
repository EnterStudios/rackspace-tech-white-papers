- [Contributing to the Rackspace Tech White Paper content repository](#contributing-to-the-rackspace-tech-white-paper-content-repository)
	- [Getting started with GitHub](#getting-started-with-github)
		- [Create a fork of this repository](#create-a-fork-of-this-repository)
		- [Keeping your fork up to date](#keeping-your-fork-up-to-date)
	- [Creating and changing articles](#creating-and-changing-articles)
		- [Create an article](#create-an-article)
		- [Edit an article](#edit-an-article)
		- [Make a change to a PR](#make-a-change-to-a-pr)
		- [Request an article change](#request-an-article-change)
	- [Writing guidelines](#writing-guidelines)
	- [Support and feedback](#support-and-feedback)

## Contributing to the Rackspace Tech White Paper content repository

This file describes the general process for maintaining source code for content
published at [https://support.rackspace.com/white-paper/](https://support.rackspace.com/white-paper/).

See [Treat Documentation Like Code](https://www.youtube.com/watch?v=haFooDkKr-A&feature=youtu.be)
for a brief video overview of how to contribute content to the support network
The examples focus onHow-to articles, but the process is the same for white
papers.

**Note**: If you already have a GitHub account, you can quickly edit an
existing article by clicking on the Edit This Article button on the left-hand
side of the page.

### Getting started with GitHub

To contribute to the How-To repository, you need a GitHub account. If you do
not have a GitHub account, you can sign up for one
[https://github.com/join](https://github.com/join).

#### Create a fork of this repository

Before you create a new article or make edits to an existing one, create a
*fork* of the Rackspace-tech-white-paper repository.

1. In the top-right corner of the page, click the **Fork** button.

2. In the pop-up box, select your personal GitHub account.

A personal copy of the How-To repository is created in your GitHub account. You
can access your fork by going to the [GitHub home page](https://github.com) and
selecting **rackspace-tech-white-paper** under **Your repositories**.

#### Keeping your fork up to date

Because your forked copy of the repository is not live, you need to
periodically update it with changes from the live repository. A status message
above the latest commit activity informs you whether your forked repository is
current with the master How-To repository. If the status says `This branch is
X commits behind rackerlabs:master`, update your repo by clicking the
**Pull request** button to the right of the message.

**Note:** If you get a message that the rackerlabs:master branch is up-to-date
with commits from your master branch, click the "switching the base" link.

**WARNING:** To avoid any merge conflicts or difficulties when making a pull
request, always check that your copy of the fork is up to date with the master
repository.

### Creating and changing white papers

Use the following instructions to create a new white paper, make edits to an
existing one, or suggest edits via an issue.

White papers are grouped into one directory per category. Each directory
contains one file per white paper.

If you're planning a white paper for a new category, put it in the best-fitting
directory, and mention your suggestion of a new category in the pull request.

#### Create a white paper

Follow these steps to create a new white paper within a category folder of the
**rackerlabs/rackspace-tech-white-paper** repo.

1. Go to the [Rackspace Tech White Paper content folder](https://github.com/rackerlabs/rackspace-tech-white-paper/tree/master/content) and click the category for which you want to create a white paper.

2. Click **New file**.

3. Enter a name for your white paper in the text box at the end of the **rackspace-tech-white-paper/content/*categoryName*/** string. The name should be in the format **your-white-paper-name.md** and should reflect the title of the white paper.

4. <a name="metadata"></a>Enter header information using the format shown in the following example:

           ---
           permalink: title-of-white=paper/
           audit_date:
           title: Title of white paper
           type: white paper
           created_date: 'YYYY-MM-DD'
           created_by: Your name
           last_modified_date: 'YYYY-MM-DD'
           last_modified_by: Your name
           category: Name of category
           category_url: category-url
           ---
5. Write your white paper in Markdown. Markdown guidelines are at https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet.

6. When you have finished writing your white paper, review it in the **Preview** tab.

7. Click **Propose new change**.

8. Create a pull request (PR). On the "Comparing changes" page, check the following settings:

    - `base fork: rackerlabs/rackspace-tech-white-paper`
    - `base: master`
    - `head fork: {your-username}/rackspac...`
    - `compare: {your-branch}`

   If the settings are not correct, use the drop down menus to select the correct settings.

   If the settings are correct, click **Create pull request**.

10. Describe the reasons for your change in the comment box, than select **Create pull request**.

**Note:** If your white paper includes images, send an email to <how-to@rackspace.com> with the image files. Note where the images belong in the white paper by using comments: `<!--this is a comment-->`.

Your PR will be reviewed. Depending on the review feedback, you might be asked to make additional changes. The How-To editorial team will merge your pull request once your contribution is reviewed.

#### Edit a white paper

Follow these steps to edit an existing white paper within a product folder of the **rackerlabs/rackspace-tech-white-paper** repo.

1. Go to the [Rackspace Tech White Paper content folder](https://github.com/rackerlabs/rackspace-tech-white-paper/tree/master/content) and click the category for which you want to edit a white paper.

2. Find the white paper you want to edit and click to open the file.

3. At the top of the white paper, click the pencil (Edit this file) icon.

4. Make any edits to the white paper directly through the GitHub website.

    **Note:** If you are using a desktop client or the command line, and you are forking or cloning the repository, be sure to make your changes in a new branch. Doing so ensures that you are producing a pull request (PR) rather than committing changes directly to the master.

5. When you have finished editing the white paper, click **Propose file change**.

6. On the "Comparing changes" page, check the following settings:

    - `base fork: rackerlabs/rackspace-tech-white-paper`
    - `base: master`
    - `head fork: {your-username}/rackspac...`
    - `compare: {your-branch}`

   If the settings are not correct, use the drop down menus to select the correct settings.

   If the settings are correct, click **Create pull request**.

7. Describe the changes that you made in a PR message.

   Use the following guidelines to create the PR message:

    - Provide a brief description of the change, starting with an imperative verb. For example, "Add a paragraph about... ."
    - If you make a complex edit, explain why you are making the edit in the larger box under **Commit changes**. For example, if you are changing the formatting of a white paper because a list should be ordered instead of unordered, say, "Switch list in middle of article to ordered to show clear progression of steps".

8. Click **Create pull request**.

Your PR will be reviewed. Depending on the review feedback, you might be asked
to make additional changes. The How-To editorial team will merge your pull
request once your contribution is reviewed.

#### Make a change to a PR

You might be asked by a member of the editorial team to update your PR. Follow
the steps below to make an update to your PR.

1. Go to the [Rackspace Tech White Paper content folder](https://github.com/rackerlabs/rackspace-tech-white-paper/tree/master/content) and select the **Pull requests** tab.

2. Find and click your PR.

3. Click the **Files changed** tab.

4. Click the pencil icon next to the file that you want to change.

5. Make your change in the editor.

6. Provide a brief description of the change.

7. Click  the **Commit directly to the `your-branch-name` branch** option, and then click **Commit changes**.

The How-To team will comment on the PR if any more changes need to be made.

#### Request a white paper change

To request a change, create an issue by clicking **Issue** near the top of this
page. Describe the changes that you are requesting.

### Writing guidelines

Use the following general writing guidelines, which are described in detail in
[style-guidelines.md](style-guidelines.md):

- Use sentence-style capitalization for titles and headings
- Use active voice
- Use present tense
- Write to the user by using second person and imperative mood
- Write clear and consistent step text
- Use consistent text formatting
- Clarify pronouns such as *it*, *this*, *there*, and *that*
- Clarify gerunds and participles
- Write clear and consistent code examples
- Use consistent terminology

Following are some specific guidelines for Rackspace technical white paper
content:

- For the first-level headings in an article, use the H3 level (designated by ###). Avoid using more than three levels of heading in an article (H3, H4, and H5). If you need more than three levels, you should consider breaking your article into two or more articles.

- If a title contains a special character, such as a colon, enclose the title with single quotation marks.

- When code includes placeholders, show them in camelCase and enclose them in angle brackets. For example, `<hostName>`.

- When creating complex lists, such as procedures with sublists, graphics, and code examples, use [these spacing guidelines](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#lists).

### Support and feedback

If you find a problem, open a GitHub issue.

If you need additional assistance, contact us at
[how-to@rackspace.com](mailto:how-to@rackspace.com).
