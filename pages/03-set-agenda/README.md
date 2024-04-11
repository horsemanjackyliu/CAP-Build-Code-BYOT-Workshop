# Set the agenda for your workshop

The agenda (the sidebar that you see on the left) is completely customizable. You can show or hide pages, create nested elements and hierarchies as needed...

The agenda is controlled in the file `agenda-sidebar.md` (in the root folder) and it is written in Markdown. As an example, the source code for the agenda of this website is:

```md
- **EXAMPLE WORKSHOP TITLE**
- [Home](/)
- How to get started
  - [Copying the template to a new repository](pages/01-setting-repository/README.md)
  - [Project structure](pages/04-project-structure/README.md)
  - [Writing the content](pages/05-writing-content/README.md)
  - [Testing locally](pages/06-testing-locally/README.md)
  - [Setting the title](pages/02-set-title/README.md)
  - [Setting the agenda](pages/03-set-agenda/README.md)
- For the SAP BTP Adoption team
  - [Dynamic content (numbers, users, passwords)](pages/10-dynamic-content/README.md)
  - [Deployment](pages/11-deployment/README.md)
  - [Updating the website](pages/12-updating/README.md)
- Best practices
  - [Writing markdown](pages/20-writing-markdown/README.md)
  - [Writing exercises](pages/21-writing-exercises/README.md)
- Downloads:
  - [Exercises in PDF](_assets/files/exercises.pdf ':ignore :target=_self')
```

As you see, it is simply a Markdown list, you can mix regular text and links and do nesting:

```md
- [Business Case](pages/usecase/README.md)
- Day 1
  - [Exercise 1](pages/01-exercise/README.md)
- Day 2
  - [Exercise 1](pages/01-exercise/README.md)
- Day 3
  - [Exercise 1](pages/01-exercise/README.md)
- [Additional information](pages/additional-info/README.md)
- Resources
  - [Troubleshooting](pages/troubleshooting/README.md)
```

> [!WARNING]
> It is crucial that you keep paths as they are: use `pages/...`
> Using `/pages/...` or `./pages/...` or `../pages/...` might work locally, but won't work when you deploy!

## Agenda for the PDF document

The repository is set up so that when the website is built (to be deployed), a PDF will be generated. You control which content will be shown in the PDF, and this is done in the `agenda-for-pdf.md` (in the root folder).

Most of the time, the only differences between `agenda-sidebar.md` and `agenda-for-pdf.md` will be:

- `agenda-sidebar.md` includes the link to the PDF, while `agenda-for-pdf.md` does not.

  ```md
  - Downloads:
    - [Exercises in PDF](_assets/files/exercises.pdf ':ignore :target=_self')
  ```

- `agenda-for-pdf.md` includes a warning about the dynamic content (they should remember to replace `${number}` with their assigned number).

  ```md
  - [PDF number warning](pages/01-pdf-number-warning/README.md)
  ```

Just remember, every time you modify `agenda-sidebar.md`, just copy and paste the content to `agenda-for-pdf.md`, remove the last _Downloads_ section, and add the number warning.

> [!TIP|icon:fa-solid fa-check|label:Congratulations]
> You have set the agenda of your workshop, and prepared the agenda for the PDF!