[reprex]: https://github.com/jcblum/reprex-howto/blob/master/reprex.md
[reprex-newbie]: https://github.com/jcblum/reprex-howto/blob/master/reprex_newbie.md
[data]: https://github.com/jcblum/reprex-howto/blob/master/reprexdata_advanced.md
[data-builtin]: https://github.com/jcblum/reprex-howto/blob/master/reprexdata_advanced.md#heading--builtin
[data-generate]: https://github.com/jcblum/reprex-howto/blob/master/reprexdata_advanced.md#heading--generate
[data-owndata]: https://github.com/jcblum/reprex-howto/blob/master/reprexdata_advanced.md#heading--owndata
[data-newbie]: https://github.com/jcblum/reprex-howto/blob/master/reprex_newbie.md#make-it-self-contained

## First and foremost, *please ask!*

A core goal of this community is to be a friendly place to chat about topics related to data science, R, and RStudio.

We know that posting to technical forums can be intimidating. You may even have had experiences that make you wary of how you will be treated in a space like this. But know that many here would love to see you overcome your inhibition and engage with us, and that we are always working to make this community worthy of your trust.

## Second, read these tips :grin:

It can be difficult to figure out the best ways to ask questions about code problems when you're new to the whole topic. Luckily, you don't have to guess :grinning:! Here are some tips that folks here think might be helpful.

### Contents

 - [Before you post](#heading--beforepost)
    - [Check out R Documentation](#heading--docs)
    - [Search](#heading--search)
 - [Writing your post](#heading--writingpost)
    - [Put extra effort into your title](#heading--title)
    - [Choose an appropriate category and tags](#heading--tags)
    - [Format your code](#heading-formatcode)
    - [Include a `Rep`roducible `Ex`ample](#heading--reprex)
    - [Data for my reprex?](#heading--reprexdata)
    - [Use screenshots the right way](#heading--screenshot)
 - [After you post](#heading--afterpost)
    - [Don't edit your original post in a confusing way](#heading--confusingedit)
    - [Avoid unnecessary backs-and-forths](#heading--backforth)
    - [Mark a solution](#heading--marksolution)
    - [New related questions belong in a new topic](#heading--newquestion)
---

<h2 id='heading--beforepost'>Before you post</h2>

<h3 id='heading--docs'>Check Out R Documentation</h3>

R has [built in documentation](https://www.r-project.org/help.html#helping-yourself) for packages and functions. This is a good place to start when you have a question! Documentation is written by many different humans, so it's not all equally clear or easy to understand, but it's always worth a try.

- Typing `?lm` into your R console will open [the documentation on the `lm` function](http://stat.ethz.ch/R-manual/R-devel/library/stats/html/lm.html)
- Typing `??"Normal Distribution"` will do a search across all your installed packages for the keywords you supplied
- Typing `browseVignettes("ggplot2")` into your R console will show you all the "vignettes" that come with the `ggplot2` package. Vignettes are long-form articles and tutorials that package authors write to explain what their package does. Often the rest of the documentation will make a lot more sense if you've read the vignettes first.

<h3 id='heading--search'>Search</h3>

Be sure to search for the basic keywords of your question. You may find that an answer is already out there! If you find something that's _almost_ an answer, but you can't figure out how to apply it to your problem, then that's a great link to include in your own question :smile:. Places to search:

- Your favorite search engine! Including "R" in your search terms may help you get more relevant results.
- [Stack Overflow](https://stackoverflow.com/tags/r/info) is a popular Q&A website with hundreds of thousands of R-related questions and answers.
- The [R-Help](https://stat.ethz.ch/mailman/listinfo/r-help) mailing list is the oldest place to get help with R questions. Unfortunately there is currently no single place where its _full_ archives can be searched, but you can search quite a few years of messages via [Nabble](https://r.789695.n4.nabble.com/R-help-f789696i96040.html).

> #### Note: Posting to Stack Overflow or R-Help
>
> It's important to know that Stack Overflow and R-Help each have different missions, and both have strong expectations about how new users should behave. Before posting a question in either place, pleaese carefully read their posting guides and spend some time watching how things work.
>
> - [Stack Overflow guides for asking questions](https://stackoverflow.com/help/asking)
> - [R-Help posting guide](https://www.r-project.org/posting-guide.html)

---

<h2 id='heading--writingpost'>Writing your post</h2>

<h3 id='heading--title'>Put extra effort into your title</h3>

Your title needs to give someone a clear enough idea of what your question is that they will want to click on the topic to read more. Tell us as much useful information as possible in as few words as possible.

#### Be specific

If your title is too general, people won't know what your question is about, and will likely be less interested in it. Here are some examples of titles that are too general, and alternatives that are much more likely to attract helpers.

- :x: Facing problem with R
- :white_check_mark: install.packages error: ggplot2 is not available for R 3.6.1


- :x: Plotting error
- :white_check_mark:


- :x: Cross-validation question
- :white_check_mark: Compute confusion matrix using k-fold cross-validation in caret::train

#### Be brief

It's easier for people to skim your topic title if you cut down on unneeded words. Think news headline, not chatty text message.

- :x: Don't know how to adjust the panel heights according to selected variable when filtering. Reason being that even for a single plot the panel size is huge.
- :white_check_mark: Keep panel height the same as number of plot panels changes

Even if you think you have an extremely simple question, please don't try to put your entire message into the title of your topic. This is considered a messy way to post, and we like to [keep things tidy]() here :grinning:.

#### Include distinct keywords

This makes your topic more likely to be discovered by the people best able to help, and helps it be discoverable in the future by people with similar problems.

Ideas for keywords:

- Key parts of error messages
- Function name *and* package name (there are _many_ cases where the same function name is used in more than one package!)
- Name of the statistical, modeling, or plotting method you are trying to use. Remember to include the full name, not just an acronym!

<h3 id='heading--tags'>Choose an appropriate category and tags</h3>

Putting your question into the right category and tagging it with relevant keywords is an important way of making your topic visible to the right people. Many folks only regularly follow certain categories and tags.

#### Categories

A Category is the section of community.rstudio.com where your topic will appear. Some Categories also have Sub-categories. You can only choose from the Categories and Sub-categories that already exist.

Here are **all the Categories**, with descriptions:

https://community.rstudio.com/categories

**Advice for choosing a Category:**

- Before you post a question in [RStudio IDE](), make sure your question is directly related to the RStudio IDE, and not a general R question. If you're not sure what the difference is, see: https://community.rstudio.com/t/differentiating-r-from-rstudio/8009

- If you are seeking support for a problem with **the shinyapps.io service**, please post in [shinyappsio](https://community.rstudio.com/c/shiny/shinyappsio) (a sub-category of the [Shiny](https://community.rstudio.com/c/shiny) category)
  - If you have a paid shinyapps.io plan, you are eligible for Premium Email Support! See: https://www.shinyapps.io/#support

- If you are seeking support for a problem with [**RStudio Cloud**](https://rstudio.cloud/), please post in the [RStudio Cloud category](https://community.rstudio.com/c/rstudio-cloud)

#### Tags

A **tag** is a keyword that helps describe the topic. You can use any term you want as a tag — if it doesn't already exist, a new tag will be created. However, it's a good idea to use an existing tag if you can.

Here are **all the currently existing Tags**:

https://community.rstudio.com/tags

**Ideas for tags:**

- :white_check_mark: Package name(s)
- :white_check_mark: Operating system
  - Most useful when reporting crashes or bugs in RStudio software, or when asking about package installation problems
- :white_check_mark: `package-installation`: if you are having a problem installing a package
- :white_check_mark: `recommendation`: if you are looking for general advice about which tools to use, or where to find specific resources
- :white_check_mark: If your question seemed to fit into two categories, include the name of the one you _didn't_ pick as a tag
- :x: Don't repeat a keyword in both Category and Tag
  - Example: If you posted in the [Shiny](#shiny) category, there's no need to also use the `shiny` tag
- :x: Don't include extra tags that aren't _directly_ related to your question

<h3 id='heading--formatcode'>Format your code</h3>

All **code** or **console output** you include in your posts should be formatted properly. Luckily, this is very easy to do! :grinning: Read this to learn how: https://community.rstudio.com/t/faq-how-to-format-your-code/6246

If you're trying to figure out how to include **properly formatted R Markdown source** in your post, here's the special trick: [Formatting R Markdown Source](https://community.rstudio.com/t/faq-how-to-format-your-code/6246#heading--rmarkdown)

<h3 id='heading--reprex'>Include a <code>Rep</code>roducible <code>Ex</code>ample — a <code>reprex</code></h3>

Most helpers will work on your code problem in two stages: first they will _read_ your code to form a hypothesis about what it does, then they will _run_ your code to test their hypothesis and find solutions to its problems.

Experienced helpers have learned that it is often a waste of time to try to debug code only by reading it, or to suggest solutions without testing them by running code. Most people here are helping others for free, on their own time. Every extra step that it takes for helpers to work on your problem is a reason for them to move on to a different question.

A good reproducible example makes both the reading and the running step as friction-less as possible for your helpers. Others should be able to copy your reproducible example and paste it into an R script to get as close to replicating your issue as possible.

If you’re still new to this idea, check out [So You’ve Been Asked to Make a `reprex`](https://www.jessemaegan.com/post/so-you-ve-been-asked-to-make-a-reprex/).

<h3 id='heading--reprexdata'>Data for my reprex?</h3>

Providing example data is often important for a good reprex. There are a few good ways to do this;
- Use [R’s built in example datasets](https://stat.ethz.ch/R-manual/R-devel/library/datasets/html/00Index.html). For example, simply calling `mtcars` in R produces the [mtcars dataset](https://stat.ethz.ch/R-manual/R-devel/library/datasets/html/mtcars.html).
- Here’s a nice discussion on [creating simple data frames for your reprex with `deparse`, `tibble` `readr::read_csv`, or `dput`](https://community.rstudio.com/t/5346).
- And many link to their data via a URL.

<h3 id='heading--screenshot'>Use screenshots the right way</h3>

Screenshots can be very useful in some cases. But in other cases a screenshot is unfriendly to your helpers, and will make it harder for people to answer your question.

Screenshots are the **worst possible way** to share anything that is **text-based**, such as error messages, code, or data :confounded:. Here's why:

- Screenshots are often difficult to read (and useless to anybody using a screen reader).
- Helpers usually want to try to _run your code_, not just look at it. Screenshots force your helpers to type everything back in by hand :weary:. That's a lot to ask and many people won't bother.
- Screenshots aren't searchable, so they don't help others with similar problems find your post later on.

#### :white_check_mark: DO use a screenshot to show…

- Plot output or complex formatted table output
- Problems with how an R Markdown file renders into a specific format (e.g., PDF or Word document)
- The location of software features (e.g. where's the environment pane?)
- What some kind of software behavior *should* look like (e.g. what should you see when you open RStudio's [Import Dataset GUI](https://support.rstudio.com/hc/en-us/articles/218611977-Importing-Data-with-RStudio)?)
- How your Shiny app looks when it is running
- An error message _that you can't copy and paste_
  - If you must do this, please try to at least include some of the key phrases from the error message in the text of your post

#### :x: Do NOT use a screenshot for…

- Including formatted code in your post
- Including sample data in a reproducible example
- Showing output or error messages from the R console

---

<h2 id='heading--afterpost'>After you post</h2>

Now the discussion can begin! :grin: Your job now is to be a polite and patient topic moderator. Keeping the discussion on track will help you find solutions faster and help others who may be reading your topic in the future.

<h3 id='heading--confusingedit'>Don't edit your original post in a confusing way</h3>

It's great to edit your original post to **add** clarifications or additional details (wondering how? see: https://community.rstudio.com/t/faq-how-do-i-edit-my-topic-or-reply/6681)

But **please don't replace your original post with something different** after people have already started discussing it. Doing this is quite unfriendly, since it makes the discussion impossible to follow for anybody who comes along later.

<h3 id='heading--backforth'>Avoid unnecessary backs-and-forths</h3>

Be as efficient as possible in any reply posts. For example, including a new `reprex`, debugging info, and extra clarifications to ensure others can help solve your issue. Keep in mind that people helping here are being incredibly kind by volunteering to assist you. They may only have a small amount of time each week to help out.

<h3 id='heading--marksolution'>Mark a solution</h3>

If someone solved your main problem, mark their reply as a solution. This helps people with similar questions quickly see what worked for you, and lets helpers find topics that still need help more easily. Solutions don't earn anybody points here, but acknowledging the person who solved your problem is friendly and will make them feel good! :heart:

https://community.rstudio.com/t/faq-how-do-i-mark-a-solution/5633

<h3 id='heading--newquestion'>New related questions belong in a new topic</h3>

Please don't treat your topic as an ongoing chat session. A few direct follow-ups are OK, but if the discussion sparks a question only loosely related to the main topic, **start a new topic** and **include a link** to your first topic to provide context.

---
<!--
#### Goals of this guide
- Pose your question so that it is more likely to get a useful response.
- Help potential responders grasp your issue.
- Keep our community tidy so folks in the future can easily find how people dealt with similar issues.

If you feel this guide or community.rstudio.com's processes can be improved, please let us know.
-->
