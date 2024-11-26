
## Summary (Summarize the bug encountered concisely)

    When creating a new blank project in GitLab, the text contains a typo: "black" instead of "blank".

## Steps to reproduce     

    Navigate to "Create a new project" page (https://gitlab.com/projects/new#blank_project)
    Find the upper left section under the heading "Create new project"
    Locate the first line of text

## What is the current bug behavior?

    The text displays incorrectly as
        "Create black project"   

## What is the expected correct behavior?

    The text should display as
        "Create blank project"
     
## Relevant logs and/or screenshots

    Screenshot:
        (Image\Bug_Project_create_blank.png)

## Possible fixes

    Line of code with the bug:
        (<h3 class="gl-text-size-h2 gl-text-inherit">
                Create black project
            </h3>)

    Fixed line of code:
        (<h3 class="gl-text-size-h2 gl-text-inherit">
                Create blank project    
            </h3>)

## Whom do you report/ Assign To/ Tags

    /label ~bug ~reproduced ~needs-investigation 
    /cc @project-manager
    /assign @qa-tester

## Priority

    Major
        The typo occurs in a critical section of the webpage and could confuse users during project creation.