# Two Sided Marketplace - Overview & Resources

This is a living document. Please add to it, change it, update it. Add useful resources, notes, and links as you find them.

To edit, go to [https://github.com/biancapower/two-sided-marketplace-notes/blob/master/README.md](https://github.com/biancapower/two-sided-marketplace-notes/blob/master/README.md), click on the pencil icon, and make your changes. Scroll to the bottom of the page and click "Propose file change". You will then be able to submit a pull request with your proposed changes.

---

## Planning

Planning should be done in roughly the order of the below sections.

### Project Management

[Trello](https://trello.com/) is a fantastic and free project management tool. Some examples of Trello boards used for app development and many other things: [Project Management with Trello](https://trello.com/inspiration/project-management).

Start using Trello (or the project management tool of your choice) from the very start. Plan before you do! Plan your planning (i.e. everything else in this section) too.

### Documentation

The README.md file should contain all of your documentation. This should include:

* Problem definition and solution
* User stories
* Workflow diagram
* Style guide
* Wireframes
* ERD
* Link to deployed website
* Notes on future development / project improvements

***Always*** insert actual images rather than giving just links, because links can go wrong, images are there forever (it's version control!).

The readme is written in markdown format. Here's a link on how to do everything you'll need to in markdown: [Mastering Markdown](https://guides.github.com/features/mastering-markdown/).

**Resources:**
* [Create TOC for README.md](https://github.com/ekalinin/github-markdown-toc)
* [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)

### Version Control

Git & GitHub. Set them up as soon as you have created your app.

**Resources:**
* [Try Git](https://try.github.io/levels/1/challenges/1) - beginner level
* [Codecademy's Learn Git](https://www.codecademy.com/learn/learn-git) - beginner level
* [Learn Git Branching](https://learngitbranching.js.org/) - beginner level (visual / interactive)
* [Pro Git](https://git-scm.com/book/en/v2) - beginner / intermediate / advanced level (detailed)

### Problem Definition & Solution

What is the problem that you have identified? Justify that it's a problem. How will you provide a solution to this problem? E.g. from [The Book Place](https://github.com/biancapower/the_book_place/blob/master/README.md#problem-definition-and-solution).

### Sign Up for Web Services

* Heroku
* AWS
* Mailgun
* Sendgrid
* Stripe
* Anything else you might need

### User Stories

Write lots of user stories from the perspectives of all potential users. E.g. both from sellers and from buyers.

**Resources:**

* https://medium.com/scrumi/what-is-a-user-story-eli5-9e6e83634482

### Workflow Diagram

Example: [Workflow Diagram](https://github.com/biancapower/the_book_place/blob/master/readme_resources/workflow_diagram.png)

**Resources:**

* [Draw.io](https://www.draw.io/)

### Style Guide

Outline the colour scheme and fonts you will use, and why.

**Resources:**

* [Google Fonts](https://fonts.google.com/)
* [Coolors](https://coolors.co/daffef-d0ffd6-d5e2bc-a6979c-d3c0d2)

### Content-First Wireframes

Example: [Content-first wireframe in Figma](https://www.figma.com/file/cHJ5winPhgKShwLn5E3RRi4l/Preloved-Books-Two-Sided-Marketplace)

**Resources:**
* [Figma](https://www.figma.com/)
* Why content-first? [Article 1](https://www.protofuse.com/blog/details/website-wireframing-helps-plan-better-content/), [Article 2](https://gathercontent.com/blog/designing-content-first-for-a-better-ux)
* [Placeholder images](https://placeholder.com/)


### Entity Relationship Diagram (ERD)
Data model, working out models and associations.

**Resources:**
* [DB Designer](https://dbdesigner.net/)
* [Basics of ERDs](https://www.youtube.com/watch?v=ymb9gsl_x1U)
* [Many to Many Relationships](https://www.youtube.com/watch?v=P_nhBKs25DQ) - "Bridge table" == "Join table"

## Implementation

The below sections are in no particular order.

### Postgresql database

Use Postgresql from the start, generating your new rails app with the following command:  ```rails new extragram --database postgresql```

Note: you may want to add additional options such as  ```--skip-active-storage```

**Resources:**

* [Getting started with Postgresql](https://www.codementor.io/engineerapart/getting-started-with-postgresql-on-mac-osx-are8jcopb) - Focus on "getting started" part 2.

### Authentication & Authorization

**Resources:**

* [Devise - getting started](https://github.com/plataformatec/devise#getting-started)
* [Devise wiki](https://github.com/plataformatec/devise/wiki)
* When in doubt, google "devise" and what you want to achieve, e.g. "devise log in using facebook"

### Payments

Start by getting Stripe Checkout fully functional in your application. Only once that is the case should you begin implementing Stripe Connect.

* [Stripe Checkout](https://stripe.com/docs/checkout/rails)
* [Stripe Connect](https://stripe.com/docs/connect)
* [Stripe Connect - how to by Scott](https://medium.com/@scottdixon/third-party-payouts-with-stripe-connect-d3a7c0d1bcb)

### Deployment

Deploy early, deploy often. Do your first deployment as soon as you have created your application.

**Resources:**
* [Heroku and Rails](https://devcenter.heroku.com/articles/getting-started-with-rails5)

### Transactional Emails

**Resources:**
* [Mailgun](https://github.com/mailgun/mailgun-ruby)
* [Sendgrid](https://sendgrid.com/docs/Integrate/Frameworks/rubyonrails.html)

### Search & Filtering

**Resources:**
* [Searchkick](https://github.com/ankane/searchkick)

### File uploads

**Resources:**
* [Carrierwave](https://github.com/carrierwaveuploader/carrierwave)
* [Amazon S3 with Carrierwave](http://blog.thefirehoseproject.com/posts/switching-carrierwave-to-use-s3-with-heroku-and-localhost/)

### Styling

**Resources:**
* [Visual Guide to CSS](https://cssreference.io/)
* [Bootstrap 4 with Rails 5](https://medium.com/@biancapower/how-to-add-bootstrap-4-to-a-rails-5-app-650118459a1e)
* [CSS Grid Garden](https://cssgridgarden.com/)
* [Flexbox Froggy](http://flexboxfroggy.com/)





