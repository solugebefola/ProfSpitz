## Prof Spitz educational site
### Summary
The site is intended to act as an enrichment for elementary, middle school and high school students.  The vehicle for the enrichment is a series of lessons that make use of rap lyrics to explore topics such as:
- literary devices
- grammatical parts of speech
- critical thinking
- rhetoric

There will be several classes of users for the site.  Students, Teachers, Administrators.

The site will contain lessons, all modeled on a single template.  Each lesson will have a video or text segment provided to the student explaining and giving examples for the lesson objectives, followed by a field for the student to input lyrics and possibly record lyrics(?).

### Users
All users will have the ability to:
 - Sign up for the site through an email invite from a user higher up on the hierarchy from the same school.  
 - Log on to the site after setting a username and password (authorization through BCrypt) and have an associated school/institution.
 - Log out of the site
 - Delete their account.

##### Students
Students have at least one associated class (more may be necessary if multiple types of classes in the school are using the site, i.e. a social studies class uses it for students in a particular grade as well as an english class).

Upon login, a student will be presented with a list of lessons, both completed and uncompleted, perhaps organized by class.  Uncompleted lessons will contain any new lessons made available since last login.  

Students will be able to:
- View all available lessons, both completed(locked) and uncompleted(organized by class?).
- Edit their contributions to any lessons that have not been locked by the teacher.
- Edit profile information
- Share lyrics with other members of the same class?

##### Teachers
Upon login, teachers will be presented with a list of classes, possibly with which lesson template are currently associated with those classes, along with a list of all available lesson templates.

Teachers will have the ability to:
- Create classes.
- Invite students to a particular class.
  - If the student already has an account, site will simply add them to a class.
  - If the student does not have an account, site will send them an email invite, and will automatically add them to the class when they create an account.
- Remove students from a class.
- Clear a class of all students (for new term).
  - possibly add to class alum list?
- Delete a class.
- Add lessons to a class from a list of available lesson templates.
  - these lessons will be distributed to each student in the class.
- View individual student input for each lesson.
  - View student interaction with all lessons for the class (number of assignments completed, skills gained).
- Add comments to each student input for each lesson.
- Assign a grade for each student for each lesson.
- Save particular inputs to a 'hall of fame' for lyrics.

##### Administrators
Upon login, admins will be presented with a list of teachers with profiles within their school as well as outstanding invites.

Admins will have the ability to:
- Invite users (admins, teachers, students) to create an account.
  - Users with accounts will be associated with the admin's school.
  - Users without accounts will have an account created and automatically connect to the admin's school.
- Remove user accounts from their school.
- Look at any teacher's views.

### Lessons
Lessons will consist of a top section with either lesson text or a video frame and a bottom input section.  

##### Lesson content
Lesson content will be either a text section that describes the task for this particular lesson and associated resources, or a video frame that contains the video for that particular lesson.  Other content can go here depending on what you guys think would work.

##### Lesson input
The input section can be a standard textarea, or something more elaborate that will be more in line with the lyrical focus of the site (maybe a line number-based input field...you guys can let me know what ideas you might have.)

##### Comments
The input section will also have a comments section so that the associated teacher can make comments on the input, either corrections or suggestions or plaudits.
