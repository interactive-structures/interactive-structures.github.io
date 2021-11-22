
# How to install, run, deploy

## Install dependencies

1. Install **Jekyll** on your local machine: https://jekyllrb.com/docs/installation/
2. Install the website dependencies by navigating to the theme directory and running `bundle install`
3. To run it locally, use `bundle exec jekyll serve --trace` to start the Jekyll server.

### Troubleshooting
The issues should be resolved as the Gemfile was updated appropriately, but just as notes:
- On Windows: [gem wdm issue](https://stackoverflow.com/questions/32723710/add-line-of-code-to-gemfile-that-already-contains-that-line-of-code)
- Add webrick for Ruby 3.0: [issue](https://github.com/jekyll/jekyll/issues/8523)


## Deployment

To update the website on https://interactive-structures.org/, you need to 
1. Run it locally using use `bundle exec jekyll serve`, which will update the `_site` folder
2. **Verify that you didn't break anything** at http://127.0.0.1:4000/
3. Push to the main branch, that's it.

(Backround: Pushing to the main branch will trigger an [Action](https://github.com/interactive-structures/interactive-structures.github.io/blob/main/.github/workflows/deploy.yml) on github that copies the `_site` folder to the `gh-branch`, which is the content visible at https://interactive-structures.org/)


# How to add conent

- Adding people to the team page: [instructions](./_people/README.md)
- Adding news items: [instructions](./_news/README.md)
- Adding publications: *todo*
- Set which publications are displayed on the home page: *todo*


# Licence
*todo*


# Acknowledgements

This website is an adapted version of the [Zolan blog template](https://zolan-jekyll.netlify.app/) and inspired by the [CMU Data Interaction Group template](https://dig.cmu.edu/).

### Credits

Based on the Zolan template, we use the following scripts, fonts or other files as listed.

*   [Google Fonts](https://fonts.google.com/specimen/Nunito) (Roboto, Sans Serif).
*   [Ionicons Icons](https://ionicons.com/)
*   [FitVids.js](http://fitvidsjs.com/)

In addition, we use
* [Jekyll Email Protect](https://github.com/vwochnik/jekyll-email-protect)

* * *

# Other Notes

[Linking A Custom Domain To Github Pages](https://richpauloo.github.io/2019-11-17-Linking-a-Custom-Domain-to-Github-Pages/)

[Direkt links to google drive](https://www.labnol.org/internet/direct-links-for-google-drive/28356/)

[Link to PDF from gdoc](https://eduk8.me/2016/06/link-google-doc-view-pdf-browser/#:~:text=Go%20to%20Sharing%20on%20the,of%20others%20finding%20your%20document.&text=Now%20the%20document%20opens%20up%20as%20a%20PDF%20in%20the%20browser.)

