# Adding a team member to the website

1. Filenames have the structure `YYYY-Firstname-Lastname`. The year is the year you started in the lab. Example: `2021-Alexandra-Ion.md`. Make sure that the filename is *unique*.

2. Add a photo of yourself as in the folder `/assets/people/`. The aspect ratio is **square** and with min. 400 px. Use the filename above, i.e., `YYYY-Firstname-Lastname.[jpg|png]`. 
For busy backgrounds, run your photo through the a background remover tool (e.g., https://www.remove.bg/) and use a neutral background image, or `#dadada` as the background color.

3. Create a new `*.md` in `/_people/`. Use the filename above, i.e., `YYYY-Firstname-Lastname.md`

Then fill it with the following content.


```
---
name: ...
role: copy from the list below
position: ...
department: ...
email: ...
website: ...
image: /people/YYYY-Firstname-Lastname.[jpg|png] --> add the real filename here 
---
```


- **name:** The name to display, e.g., Alexandra Ion, Yunqi "Willa" Yang
- **role:** This field is used for sorting. Use of the following roles verbatim:   
    - Professor
    - Admin
    - PhD student
    - Visiting PhD student
    - Masters student
    - Undergraduate student
    - Collaborator

- **position:** The position that will be displayed. It is often the same as the role, so use the same text if applicable.
- **department:** The department that you are majoring in. Add the University for visiting team members.
- **email:** Your email such that people can reach out to you. We use an email protection library.
- **website:** Your website, if applicable.
- **image:** The path to the photo file, relative to the root folder of this repository (i.e. to index.html)

- *alumni_since:* Once someone leaves the group, add `alumni_since: YYYY` to mark them as alumni.
