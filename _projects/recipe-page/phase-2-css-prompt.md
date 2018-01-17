# Project 1 - Recipe Page
### Phase 2 - Add styling with CSS

### Languages
- HTML
- CSS

### Frameworks
None

### Primary Goals
1. Learning to style HTML using CSS
2. Receiving and incorporating constructive feedback on a project

### Overview
In this project you will create a well-designed webpage that displays one of your favorite recipes. It will include the ingredients, the steps needed to make the dish, links to similar recipes, and at least one photo.

Phase 1 of the project involves coding the structure of your webpage using HTML. This includes the ingredients, the steps needed to make the dish, links to similar recipes, and at least one photo.

Phase 2 of the project involves adding styling and pizazz using CSS. This includes changing the font style, font size, colors, and significantly altering the layout.

Phase 3 of the project involves incorporating Bootstrap. You'll add a navigation bar and several other Bootstrap components of your choosing.

Phase 4 of the project involves incorporating jQuery. You'll add at least one interactive element of your choosing.

### Context
- You completed a basic HTML page in Phase 1
- You learned basic CSS syntax and rules in the intro lesson
- Let's style your HTML with CSS!

### Basic Requirements
1. Create a file tree for your Recipe Page project
2. Create a CSS file in the proper directory of your file tree
3. Link to your CSS file from within your HTML `<head>` tags
4. Change the background color of your webpage
5. Change the font and font color of your headings and paragraphs
6. Constrain the description to the width of the image
7. Make the image and ingredients appear on the left
8. Make the instructions appear on the right
9. Obtain a code review from Techtonica staff once you've fulfilled these requirements

## Setup Instructions
Use the Terminal for navigating around the file system and creating new folders and files. Refer to the lesson on [The Command Line Interface](https://github.com/Techtonica/curriculum/blob/master/command-line/command-line-interface.md) if you need guidance on using the Terminal.

When you get to the steps below that ask you to initialize a git repo and track files using git, refer to the lesson on [Git and Version Control](https://github.com/Techtonica/curriculum/blob/master/git-version-control/lesson-plan.md) if you need guidance.

1. Navigate to the `recipe-page` directory.  

If you have questions, do not disturb your colleagues until you have spent at least 20 minutes troubleshooting on your own. Be sure to format your question using the template we practiced in the [Asking Good Questions](https://github.com/Techtonica/curriculum/blob/master/asking-good-questions/asking-good-questions.md) lesson.  


## Lab Instructions  


### Starter Code
You'll be building on the HTML code you completed in Phase 1 of this project.


### Lab Exercise  

#### Part 1 - Create a file tree for your Recipe Page project

Using the Terminal, ensure you are in the `recipe-page` directory. Run the `ls` command. The only file you should see is `index.html`.

The CSS file needs to go in the `css` directory, which goes inside the `static` directory, which goes inside the `recipe-page` directory. So, the path to the CSS file should be: `recipe-page` > `static` > `css` > `styles.css`. Here's how to accomplish this:

1. Since `recipe-page` is the current working directory, create a new directory called `static` and then navigate to `static`. 
2. From within the `static` directory, create a directory called `css` and then navigate to `css`.

#### Part 2 - Create a CSS file in the proper directory of your file tree

1. Now that you're in the `css` directory, create the `styles.css` file. You can verify this worked by running the `ls` command.
2. Navigate back to the `recipe-page` directory. Use the Terminal shortcut to open this whole directory in Atom.
3. Navigate back to `techtonica-projects` to easily run all the git commands.
4. Run `git status`. You should see something similar to this:

![Result of running git status after creating file tree](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/git-status-static-folder.png)

> **PAUSE.** Obtain a code review from Techtonica staff.

Add and commit, making sure to write a descriptive commit message in the present tense, such as "Create project file tree and stylesheet."

#### Part 3 - Link to your CSS file from within your HTML `<head>` tags

1. Find the `styles.css` file in Atom that you just created. Add this small bit of CSS code to the file, then save the file. 

```css
p {
  font-color: blue;
}
```

We're doing this so we can easily see if we've successfully connected `styles.css` to `index.html`. We'll know it worked if all of our paragraph text appears blue instead of the default black when we load `index.html` at the end of this step.

2. Now we need to link to `styles.css` from within `index.html`. Find the `index.html` file in Atom. Read the following code snippet and make sure you understand what it does. Then, copy and paste it into the `<head>` area of `index.html`, just below the `<meta>` tag.

```html
<link rel="stylesheet" type="text/css" href="static/css/styles.css">
```

**Questions to Consider**
- What are `rel`, `type` and `href` called?
- What are `"stylesheet"`, `"text/css"` and `"static/css/styles.css"` called?
- Why do we use the filepath `"static/css/styles.css"`?

Open `index.html` in Chrome. The blurb under your title should be blue!

![Webpage after making paragraph text blue](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/blue-blurb.png)

When you're satisfied that `styles.css` is properly linked to `index.html`, run `git status`. Add and commit, making sure to write a descriptive commit message in the present tense, such as "Link stylesheet to index."


#### Part 4 - Change the background color of your webpage

If you want to change your paragraph text back to black from the temporary blue, do so now by simply deleting all the code in `styles.css`.

Now, write some CSS code in `styles.css` that will change the background color to any color you like! You can use [this color picker](http://htmlcolorcodes.com/color-picker/) to find the right hexadecimal color code.
- Keep in mind that readability is really important. It's very hard for most people to read screens that have really bright backgrounds (yellow, orange, red, pink) or really dark backgrounds (black, brown, navy).

Refresh `index.html` in Chrome by pressing `<COMMAND> + r`. Does your new background color show up?

![Web page after changing the background color](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/background-color.png)  

When you're happy with the background color, run `git status`. Add and commit, making sure to write a descriptive commit message in the present tense, such as "Change background color."


#### Part 5 - Change the font and font color of your headings and paragraphs
1. Select all the headings by writing CSS code inside `styles.css` and change the color to something that works well with your background color. 
- Hint 1: Can you figure out how to use multiple selectors for the same style change, rather than writing code for each one separately?
- Hint 2: Use the drop-down menu on the color picker website to easily find contrasting and complementary colors.

![Color picker drop-down menu](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/Screen%20Shot%202018-01-17%20at%203.05.48%20PM.png)

Refresh `index.html` in Chrome by pressing `<COMMAND> + r` to see if it worked! 

![After changing header colors](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/change-header-colors.png)

When you're happy with the new font color, run `git status`. Add and commit, making sure to write a descriptive commit message in the present tense, such as "Change font color."

2. Find a [Google font](https://fonts.google.com/) that you think works really well with your color scheme, recipe and the overall vibe you want to create on your webpage.

![Monoton Google Font](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/google-font-monoton.png)

When you find a font you want to use, click the orange plus sign in its upper right hand corner. A black strip will appear at the bottom of your browser. 

![Google Font Selection](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/google-font-selection.png)

Click on it to expand it. You'll now see a pane that contains some HTML code and some CSS code. Copy and paste these code snippets into the proper files in order to include this new font in your project.

![Google Font Selection Expanded](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/google-font-selection-expanded.png)

Refresh `index.html` in Chrome by pressing `<COMMAND> + r` to see if it worked.

![After importing Google Font](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/after-google-font-import.png)

If you need to make the font size larger or smaller for your headings due to the new font's default size, go ahead and make these changes now in `styles.css`.

When you're happy with the new font, run `git status`. Add and commit, making sure to write a descriptive commit message in the present tense, such as "Link to Google font for headers."

> **PAUSE.** Obtain a code review from Techtonica staff.  


#### Part 6 - Make the description the same width as the image

You may remember from Phase 1 of the project that we constrained the width of the image to 600px. (If you didn't do this yet for some reason, please do so now.) Let's now also constrain the blurb text under neath the title to a width of 600px, to make it easier for the user to read.

The description is currently inside a pair of `<p>` tags. But if we use the `<p>` element as a selector, if we add more paragraph text later, it will also be affected by the 600px constraint. A better way to select the description is to give its opening `<p>` a class called "description" and then use `.description` as a selector in `styles.css`. Go ahead and do this, implementing the width constraint to 600px on your own.

Refresh `index.html` in Chrome by pressing `<COMMAND> + r`. Did it work?

![After limiting description to 600px](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/constrained-description.png)   

When you've successfully constrained the width of the description to match the width of the image, run `git status`. Add and commit, making sure to write a descriptive commit message in the present tense, such as "Constrain description width to 600px."

#### Part 7 - Make the image and ingredients appear on the left

Right now, the entire webpage is displayed in a vertical fashion. We can make all the content appear on the screen, side by side, and eliminate the need for a user to have to scroll to read everything.

We've already accomplished some initial steps for making this happen. We have the title and description in their own `<div>` which has a class called `top`. If we don't specify any layout styling for this div in `styles.css`, it just defaults to taking up the whole width of the screen. This is what we want, based on the layout image [shown in the instructions](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/phase-1-html-prompt.md#part-9---add-some-divs-for-easy-css-integration-later).

We've also created divs that have a class called `left` and `right`, respectively. Can you guess what we're going to use those classes for? We're going to use them as CSS selectors!

1. In `styles.css`, use the `left` class as a selector. We want to constrain the width of this div to 600px so that it aligns perfectly with the image above it. Implement that now. We also want it to float on the left. Implement that now, too.

Refresh `index.html` in Chrome by pressing `<COMMAND> + r`. Do you see a change to your layout?

You should see that while the div with the `left` class has stayed on the left, the div with the `right` class is now on the right and overlapping some of the content. Progress! Let's fix that silly overlap in the next step.

![result of floating the left class](https://github.com/Techtonica/curriculum/blob/master/_projects/recipe-page/screenshots/float-left-left.png)   

When you've successfully made the `<div>` with the `.left` class float on the left of the webpage, run `git status`. Add and commit, making sure to write a descriptive commit message in the present tense, such as "Float half the content on the left."

-----

### Questions to Consider
- What, if anything, was challening about this phase of the project?
- What did you enjoy the most while working on this phase of the project?
- What questions came to mind as you were working through the steps?
- If you were to explain to a bright child what you worked on during the phase, what would you tell them?

### Extensions
- thing
    