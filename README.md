# cfp-mockup
Code For Philly mockup. View our progress here: codeforphilly.github.io/cfp-mockup/

# Goal 
The goal of this particular project is just to re-do the homepage first, and connect it to the existing old pages and laddr. The issues on our "Issues" page in this repo are ones that the leadership team has identified as things they would like changed. However we're open to other ideas of course.

# More Details and our Blog
https://codeforphilly.org/projects/code_for_philly_website_redesign

# How to change a project on the home page

There are 2 things to change in index.html:
- the project card in the "Portfolio Grid", and
- the modal that pop ups when you click on the project card.

You can change index.html by going to https://github.com/CodeForPhilly/cfp-mockup/blob/main/index.html then clicking the edit button, which looks like a pencil. It's close to the "Raw" and "Blame" buttons.

Below are instructions on how to change index.html. Here is an example change: https://github.com/ZacharyRSmith/cfp-mockup/pull/1/files

How to change the project card:

In index.html, search for `<!-- Portfolio Grid -->`. Here, you will find the project card to change. Change:
  - the img
  - the heading
  - the subheading

How to change the popup modal:

1. Copy html/projects/template_modal.html to any location where you can replace all the `TODO`s.
- For `id="portfolioModalTODO"`, you'll set the id to the project card's href minus the `#`. Ex.: `id="portfolioModal3`.
- For `<!-- MODAL TODO -->`, replace TODO with the modal number. Ex.: `<!-- MODAL 3 -->`.
- Replace the rest of the TODOs.
2. Now that your HTML is ready, find the modal to replace in index.html by searching for the popup modal id. Replace it with your HTML.

# Development
## Changing nav or footer

1. Make changes in index.html
1. Either:
- run `node sync_nav_and_footer.js`, or
- manually update the final HTML pages by copying & pasting from index.html to the other pages (currently sponsor.html and volunteer.html).
