# Step 5: Create MkDocs Configuration (mkdocs.yml)

1. **Create the `mkdocs.yml` file**:
   - In the root of the project, right-click the folder and choose "Create File".
   - In the window that appears, enter the filename `mkdocs.yml`.
![create yaml.png](image/Documentation%20Setup/Create%20MkDocs%20configuration%20%28mkdocs_yml%29/create%20yaml.png)
   ➤ To create a Yaml file, just add the `.yml` extension to the file name.
   - Add the file to Git.
![add to git.png](image/Documentation%20Setup/Create%20MkDocs%20configuration%20%28mkdocs_yml%29/add%20to%20git.png)
   ➤ After this step, you will have a `mkdocs.yml` file in your project tree.
# Step 6: Create Documentation in Markdown Format

1. **Create a `docs` folder** for storing the source text files.
2. **Create an `image` folder** for storing images.

   As a result, your project structure will be scalable and look like this:

Web-docs/ # Parent directory 
```
├── .venv/ # Virtual environment of the project 
├── docs/ # Documentation source files 
├── image/ # Documentation images 
├── mkdocs.yml # MkDocs configuration file
```

Next, within the `docs` folder, create your first Markdown file.
![First docs file.png](image/Documentation%20Setup/Create%20documentation%20in%20Markdown%20format/First%20docs%20file.png)
➤ To create a Markdown file, just add the `.md` extension to the filename and start adding content according to the rules described below.

## Basics of writing text in Markdown

Markdown is a simple markup language for formatting text. It allows you to create structured text using simple symbols.  
Here are the main features:

1. **Headings**  
   Use the `#` symbol to create headings of different levels. The more `#` symbols, the lower the heading level.  
   Example:
   ```markdown
   # Heading Level 1
   ## Heading Level 2
   ### Heading Level 3
2. **Paragraphs and Line Breaks**
* To separate paragraphs, leave a blank line.
* To force a line break, add two spaces at the end of a line.

**Example:**
```markdown 
This is the first paragraph.

This is the second paragraph.
And this is the second line without a paragraph.
```
3. **Text Formatting**
* Bold: Wrap text in double asterisks (**) or double underscores (__).
**Example:**
```markdown 
**Bold text**
__Bold text__
```
* Italics: Wrap text in single asterisks (*) or single underscores (_).
**Example:**
```markdown 
*Italics*
_Italics_
```
* Strikethrough: Use double tildes (~~).
**Example:**
```markdown 
~~Strikethrough text~~
```
4. **Lists**
* Bulleted list: Use -, *, or +.
**Example:**
```markdown 
- Item 1
- Item 2
  - Sub-item
  ```
* Numbered list: Use numbers with a period.
**Example:**
```markdown 
1. First
2. Second
```
5.	**Links**
```markdown 
[Link text](URL)
```
6.	**Images**
```markdown 
![Image name](../image/1_structure_project.png)
```
➤ To add an image, you don’t need to specify the path manually. Just drag the image from the left menu to the desired location, and PyCharm will automatically generate the path.
![drug-n-drop image.png](image/Documentation%20Setup/Create%20documentation%20in%20Markdown%20format/drug-n-drop%20image.png)
➤ PyCharm has three document display modes, including a preview with images.
![Preview .png](image/Documentation%20Setup/Create%20documentation%20in%20Markdown%20format/Preview%20.png)
7.	**Code**
* Inline code: Wrap the text in backticks (`).
**Example:**
```markdown 
`python -m venv .venv`
```
* Code block: Wrap the text in triple backticks (`````) followed by the language.
**Example:**
```markdown 

```print("Hello, World!")```

```
8.	**Tables**
Create tables using vertical bars (|) and hyphens (-).
**Example:**

```markdown 
| Heading 1 | Heading 2 |
|-----------|-----------|
| Text 1    | Text 2    |
```
9.	**Note**
Use the `>` symbol to create notes.
**Example:**
```markdown 
> Note: Always test your code before deploying.
```

> In some cases, the numbering may be broken. To fix this, I use HTML to continue the numbering:

```
<ol start="5">
  <li>Links:</li>
  <a href="URL">Link text</a>
</ol>
```

# Step 7: Complete the Structure of Your Project

1. In the source folder, create the file `index.md` — the text of this document will be displayed on the home page of the site.
![Create index_md.png](image/Documentation%20Setup/Complete%20the%20structure%20of%20your%20project/Create%20index_md.png)
2. Create the `.gitignore` file in the root of the project and write `site` in it — this will prevent Git from tracking the compiled files.
![Gitignore.png](image/Documentation%20Setup/Complete%20the%20structure%20of%20your%20project/Gitignore.png)
➤ The "site" folder will be automatically generated during deployment.

Now, your project structure looks like this:
```
Web-docs/  # Parent directory
├── .venv/  # Virtual environment
├── docs/  # Documentation source files
	├── index.md/  # Home page
├── image/  # Documentation images
├── mkdocs.yml  # MkDocs configuration file
├── .gitignore  # Ignored files
```







