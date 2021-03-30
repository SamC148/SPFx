For detailed instructions on how to build this web part and teh needed list please watch: https://www.youtube.com/watch?v=oIr-rgGvUUk

## react-faq-video
### Prep
1. Build a SharePoint Online list named "FAQ"
2. Rename Title column to "Question"
3. Add 3 additional columns

    - Multiple lines of text column, toggle 'use rich text' to yes, name "Answer"
    - Choice column, Options "Work", "Personal", and "Hobby", name "Category"
    - Yes/no column, set default to No, name "Featured"
4. Add items to your list making sure to set some to 'yes' in the featured column
5. Navigate to your sites workbench (https://<tenant>.sharepoint.com/sites/<your site>/_layouts/15/workbench.aspx)

### Building the code
1. Clone the repo
2. In the command line run
    a. npm i
    b. gulp serve --nobrowser

### Deploying the code
1. In the command line run
    a. npm i
    b. gulp bundle --ship
    c. gulp package-solution --ship
2. Add to App Catalog
3. Add App to site with FAQ list
4. Add web part to page

### Features
DefaultButton,
Modal,
DetailsList,
IColumn,
from office-ui-fabric-react

IPropertyPaneDropdownOption 
 from @microsoft/sp-property-pane

RichText,
Accessible Accordion 
from @pnp/spfx-controls-react

