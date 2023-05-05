# GNOME GSoC PROPOSAL


<b>Gotam Gorabh</b><br>
gautamy672@gmail.com<br>
@gautham_x:matrix.org / Gotam Gorabh

# Create a New “System” panel in GNOME Settings

## General Details

<b>Name:</b> Gotam Gorabh<br>
<b>University:</b> Indian Institute of Information Technology, Kottayam<br>
<b>Primary Email:</b> gautamy672@gmail.com<br>
<b>Secondary Email:</b> gotamgorabh20bcs173@iiitkottayam.ac.in<br>
<b>Matrix ID:</b> @gautham_x:matrix.org<br>
<b>IRC Nick:</b> Gotam Gorabh<br>
<b>TimeZone:</b> India(GMT+5:30)<br>
<b>GitHub:</b> [GOTAM672](https://github.com/GOTAM672)<br>
<b>GitLab(GNOME):</b> [gautham_x](https://gitlab.gnome.org/gautham_x)<br>
<b>GitLab(Inkscape):</b> [Gau672tam](https://gitlab.com/Gau672tam)<br>
<b>Size of the Project:</b> Large(350 Hours)<br>

## Description

<b>GNOME Settings</b> (aka gnome-control-center) is a graphical user interface tool used in
GNOME-based Linux distribution for managing system settings and preferences. This proposal
plans to create a new system panel and move Region & Language, Date & Time, Users, and
About panels into a new System panel.

## Mentors

- [Felipe Borges](https://gitlab.gnome.org/felipeborges) (@felipeborges)
- [Georges Basile Stavracas Neto](https://gitlab.gnome.org/feaneron) (@feaneron)

## What city and country will you reside in during the summer?

I will stay at my college in Pala, Kerala, India

## What applications/libraries of GNOME will the proposed work modify or create?

GNOME Settings (aka gnome-control-center)

## What benefits does your proposed work have for GNOME and its community?

The goal of this project is to create a new system panel that will provide users with a unified
interface for managing various settings by moving <b>Date & Time, Users, Region & Language,</b>
and <b>About</b> panels, and Implementing a <b>Remote Desktop</b> page into the new system panel.

By creating a new system panel, we can provide a more streamlined and user-friendly
experience for GNOME users. This will also make it easier for users to find the panel they’re
looking for.

## Why are you the right person to work on this project?

I believe I am the right person to work on this project as I have prior experience working on
open-source projects and I have been using GNOME for a long time. <b>During my contribution, I
learned GTK, GObject, LibAdwaita, XML, UI, C, Git, etc.</b>

Also, <b>I am aware of GNOME’s Newcomer’s guidelines, coding standards, and community
working culture.</b> If I don’t know something, I try my best to learn it and don’t hesitate to ask
questions.

My previous contributions to GNOME and other open-source projects demonstrate my
commitment to the open-source community. I am familiar with the development process, version
control system, and project management tools. I also understand the importance of
documentation, and I always ensure that my code is well-documented.
Overall, I believe that my skills, experience, passion, and commitment make me the right person
to work on this project.

## How do you plan to achieve the completion of your project?

We have approx 12 weeks or even more to achieve the goal and have 5 panels to merge or
implement it into the system panel. The plan is to first study the <b>Accessibility panel</b> for
inspiration to make a minimalistic system panel.

I’ll give approx 2 weeks for attaching each panel as a page to the system panel. <b>Within these 2
weeks, I’ll work on eliminating any errors, and wrong coding standards and updating the
UI with the help of my mentors and extensive use of documentation.</b> After successfully attaching of page,
I will delete that panel from the panel list.

Also, take feedback from my mentors and design team members for any modification apart from
mockups.

## Please provide a sequence of tasks and subtasks and how long (days) you estimate it will take you to complete each of them. Highlight important milestones/deliverables.

My proposed timeline for the tasks will be as follows:

<b>Before May 04</b>
- I’ll continue working on the existing issues and my opened MR which is halted due to GNOME’s UI freeze schedule to get more understanding of the project.
- Also, I’ll keep interacting with the GNOME community to help each other if needed.
- Study the <b>GObject</b> concept.

<b>May 04 – May 28 (Community Bonding Period)</b>
- With the help of my mentors, I’ll familiarize myself with the community and will try to know the culture and ethics of the organization.
- Take inspiration from <b>Accessibility Panel’s</b> code implementation.
- Understand how to implement <b>CcSystemPanel</b> class, <b>AdwLeaflet</b> page, and bind system panel to panel list.
- Read and gather all the documentation and resources that will be used in this project.
- With the help of my mentors, I’ll plan a timetable and weekly calls/meetings, to submit the weekly report and ask for additional resources.

<b>May 29 – June 04 (Week 1) [System Panel Implementation]</b>
- Create a system panel by implementing <b>CcSystemPanel</b> class.
- Implement <b>AdwLeaflet</b> content page with temporary dead rows when clicked will open each page.
- Add <b>.desktop.in, meson.build, .gresource.xml files</b>, and <b>icons</b> folder to the system panel folder.
- Update necessary files and folders to bind the system panel to the panel list.
- Run and test the minimalistic System Panel.
- Eliminate errors, and wrong coding standards and update the UI with the help of my mentors and documentation
- I implemented week 1 work [Here](https://gitlab.gnome.org/gautham_x/gnome-control-center/-/commit/cecf857a4b66c6e2339070233a892def292c950a) (At New-System-Panel Branch).

<b>June 05 – June 18 (Week 2 & Week 3) [Region & Language Page Implementation]</b>
- Study <b>Region & Language</b> panel code to identify the code that can be reused/refactored.
- Use the <b>CcRegionPanel</b> class code to create <b>CcSystemRegionPage</b> class.
- Implement Region & Language page using <b>CcSystemRegionPage</b> class and <b>AdwPreferencesPage</b> for the GUI part.
- Bind this page to Region & Language row inside the <b>AdwLeaflet</b> page. Update necessary files and folders.
- Run and test the Region & Language Page.
- Eliminate errors, and wrong coding standards and update the UI with the help of my mentors and documentation.
- Finally, delete Region & Language panel from the panel list.
- The work done till now for weeks 2 & 3 is [Here](https://gitlab.gnome.org/gautham_x/gnome-control-center/-/commit/2ec28dbee7c95f547898d2ca1dd96b9a8bbb4a5a) (At New-System-Panel Branch)

<b>June 19 – July 02 (Week 4 & Week 5) [Date & Time Page Implementation]</b>
- Study the <b>Date & Time</b> panel code to identify the code that can be reused/refactored.
- Use the <b>CcDateTimePanel</b> class code to create <b>CcSystemDatePage</b> class.
- Implement the Date & Time page using <b>CcSystemDatePage</b> class and <b>AdwPreferencesPage</b> for the GUI part.
- Bind this page to Date & Time row inside the <b>AdwLeaflet</b> page. Update necessary files and folders.
- Run and test the Date & Time Page.
- Eliminate errors, and wrong coding standards and update the UI with the help of my mentors and documentation.
- Finally, delete Date & Time panel from the panel list.
- The work done till now for weeks 4 & 5 is [Here](https://gitlab.gnome.org/gautham_x/gnome-control-center/-/commit/307aec8ebce3399742ba300fa369fcc19e5d4f0) (At New-System-Panel Branch).

<b>July 03 – July 09 (Week 6) [About Page Implementation]</b>
- Study <b>About</b> panel code to identify the code that can be reused/refactored.
- Use the <b>CcInfoOverviewPanel</b> class code to create <b>CcSystemAboutPage</b> class.
- Implement the Users page using <b>CcSystemAboutPage</b> class and <b>AdwPreferencesPage</b> for the GUI part.
- Bind this page to the Users row inside the <b>AdwLeaflet</b> page. Update necessary files and folders.
- Run and test the About Page.
- Eliminate errors, and wrong coding standards and update the UI with the help of my mentors and documentation.
- Finally, delete the About panel from the panel list.
- The work done till now for week 6 is [Here](https://gitlab.gnome.org/gautham_x/gnome-control-center/-/commit/546a1d4ddaa516340ae1b0ff1d0d711c99c953e5) (At New-System-Panel Branch).

<b>July 14 – August 03 (Week 7, Week 8 & Week 9) [Users Page Implementation]</b>
- Study <b>Users</b> panel code to identify the code that can be reused/refactored.
- Use the <b>CcUserPanel</b> class code to create <b>CcSystemUsersPage</b> class.
- Implement the Users page using <b>CcSystemUsersPage</b> class and <b>AdwPreferencesPage</b> for the GUI part.
- Bind this page to the Users row inside the <b>AdwLeaflet</b> page. Update necessary files and folders.
- Run and test the Users Page.
- Eliminate errors, and wrong coding standards and update the UI with the help of my mentors and documentation.
- Finally, delete the Users panel from the panel list.

<b>August 04 – August 10 (Week 10) [Remote Desktop Page Implementation]</b>
- Implement a Remote Desktop page using <b>CcSystemRemotePage</b> class and <b>AdwPreferencesPage</b> for the GUI part.
- Inside Remote Desktop Page, use <b>CcListRow</b> to create Remote Desktop, Remote Control, Device Name, and Remote Desktop Address row.
- use <b>CcListRow</b> with <b>GtkEntry</b> and <b>GtkPasswordEntry</b> to create a User Name and Password row.
- Bind this page to the Remote Desktop row inside the <b>AdwLeaflet</b> page. Update necessary files and folders.
- Use <b>GtkClipboard</b> to implement copy button.
- The work done till now for weeks 9 & 10 is [Here](https://gitlab.gnome.org/gautham_x/gnome-control-center/-/commit/d1c85b318fee0ed96bf374c91cb7b414708d9336) (At New-System-Panel-Branch).

<b>August 11 – August 24 (Week 11)</b>
- Run and test the Remote Desktop Page.
- Eliminate errors, and wrong coding standards and update the UI of <b>Remote Desktop Page</b> Implementation with the help of my mentors and documentation.
- Also, Use <b>AdwExpanderRow</b> to Implement the <b>System Start Options</b> row.
- Also, take feedback from my mentors and design team members for any modification.
- Complete all pending works(if any) related to other pages.
- If there is enough time, start a discussion on <b>adding the unit test cases</b>. With the help of mentors, I’ll Identify the modules or functions that need to be tested.
- Also decide which unit testing framework will be used (possibly <b>GLib or JUnit, NUnit, pytest</b>).
- If any errors are found during the testing, debug the code to identify the cause of the error and fix the errors.

<b>August 25 – August 31 (Week 12)</b>
- This week is utilized as space for any possible delays or unforeseen events

<b>Post GSoC Goals</b>
- Continue working on GNOME and solve issues, and I’ll also try to implement pending mockups.
- Working at GNOME is something I have enjoyed, so would like to continue it.

<b>What are your past experiences with the open-source world as a user and as a contributor?</b>  

I have a great experience with the open-source world as a user, which lead me to become a
contributor as well.  

From a user's perspective, I have been a long-time user of open-source software, including
Linux, Git, and Inkscape. I'm a very enthusiastic user of Arch distribution with the GNOME
desktop environment. And I wondered how these products were still free, so I decided to
contribute to the open-source to pay my part. As a user, we have the privilege to make our
(users’) voices heard directly by the project's maintainers.  

From a contributor's perspective, That was a great moment for me when my first MR get
merged into <b>GNOME Nautilus</b> and I feel proud that the code I wrote is now being used by
thousands of people, however small the contribution may be. I began my open-source journey
with GNOME and got the opportunity to meet and work with amazing people around the world.  

Through my experiences as a user and contributor, I have developed a strong understanding
of the importance of open-source software and the benefits it provides to developers and users
alike. I have gained a deep understanding of the value of open-source software and the
importance of collaborating with others to improve it. Also, open-source contribution teaches
not only to develop software but also an attitude to play an active role in improving the world.

<b>Please include links to your code contributions which have already been
merged, or to Gitlab merge requests for the issues you fixed for the
project ofyour proposal or any other GNOME projects. This demonstrates
your willingness to learn and familiarity with development workflow.</b>    

My contributions to GNOME Settings(gnome-control-center) so far are described below:  
- Updated Hotspot Dialog: [MR 1622](https://gitlab.gnome.org/GNOME/gnome-control-center/-/merge_requests/1622) [Merged]
- Removed account activity window: [MR 1559](https://gitlab.gnome.org/GNOME/gnome-control-center/-/merge_requests/1559) [Merged]
- Renamed ‘Test Your Settings’ button: [MR 1486](https://gitlab.gnome.org/GNOME/gnome-control-center/-/merge_requests/1486) [Merged]
- Fixed cancel button issue: [MR 1732](https://gitlab.gnome.org/GNOME/gnome-control-center/-/merge_requests/1732) [Merged]
- Redesigned remove user dialog: [MR 1584](https://gitlab.gnome.org/GNOME/gnome-control-center/-/merge_requests/1584) [Open]
- Updated Forget Connection dialog with AdwMessageDialog: [MR 1699](https://gitlab.gnome.org/GNOME/gnome-control-center/-/merge_requests/1699) [Open]

Apart from these contributions, I also contributed to some other GNOME projects.
- GIMP: Added scrolled window to TIFF description field. [MR 745](https://gitlab.gnome.org/GNOME/gimp/-/merge_requests/745) [Merged]
- GNOME Epiphany: Used suitable tooltip-text for bookmark icon. [MR 1271](https://gitlab.gnome.org/GNOME/epiphany/-/merge_requests/1271) [Merged]
- GNOME Nautilus: Used consistent language. [MR 930](https://gitlab.gnome.org/GNOME/nautilus/-/merge_requests/930) [Merged]
- GNOME Nautilus: Removed trailing ellipsis. [MR 1012](https://gitlab.gnome.org/GNOME/nautilus/-/merge_requests/1012) [Merged]
- GNOME Nautilus: Added trailing ellipsis. [MR 986](https://gitlab.gnome.org/GNOME/nautilus/-/merge_requests/986) [Merged]
- GNOME Photos: Addes tooltip-text to UI elements. [MR 260](https://gitlab.gnome.org/GNOME/gnome-photos/-/merge_requests/260) [Open]
- GNOME Calendar: Used lock-icon for read-only calendars. [MR 304](https://gitlab.gnome.org/GNOME/gnome-calendar/-/merge_requests/304) [Open]

<b>If available, please include links to any code you wrote for other opensourceprojects.</b>    

I started my Open-Source journey with GNOME. But other than GNOME projects I also
contributed to <b>Inkscape Project</b>. Here are my contributions to <b>Inkscape:</b>    
- Adding Clone task operation to context menu. [MR 5050](https://gitlab.com/inkscape/inkscape/-/merge_requests/5050) [Merged]
- Fix overlapping info box in measurement tool. [MR 4728](https://gitlab.com/inkscape/inkscape/-/merge_requests/4728) [Merged]
- Fix differences in position of Infobox for different display-unit. [MR 4944](https://gitlab.com/inkscape/inkscape/-/merge_requests/4944) [Merged]
- Replace html tags with an open and close parenthesis. [MR 4813](https://gitlab.com/inkscape/inkscape/-/merge_requests/4813) [Merged]
- Enlarge Autosave Entry Field. [MR 4730](https://gitlab.com/inkscape/inkscape/-/merge_requests/4730) [Open]

<b>What other relevant projects have you worked on previously and what
knowledge have you gained from working on them?</b>

Not worked on any direct relevant project...

But I did a GUI project, which is used to convert an image from one format to another format.
This project is written in Go programming language and for the GUI part I used NuxUI. [Project
ImageFormater](https://github.com/GOTAM672/ImageFormater) 

From this project I learned...
- Go Programming Language
- NuxUI
- How to compile and run a Go base project.

<b>What other time commitments, such as school work, exams, research,
another job, planned vacation, etc? What are the dates for these
commitments and howmany hours a week do these commitments take?</b>

I will take GSoC as a full-time commitment for 3 months (May, June, and July) because of my
semester break. During this semester break, I will devote 40-45 hours a week to the project.
After August 1, My 7th semester will start and the company starts visiting my college for hiring
students. So for preparing for Interviews and Exams, I will devote only 30-35 hours a week to
the project.

<b>About Me</b>     

I am pursuing B.Tech in Computer Science and Engineering from the Indian Institute of
Information Technology, Kottayam. I am currently in my pre-final year.I love to learn and try new stuff in my free time and <b>I believe in learning by doing</b>. Currently,
I am learning <b>Rust Programming language</b> via project building, and contributing to rust opensource projects.

Being a student of a technical institute, I have learned <b>Data Structures & algorithms,
problem solving-skills, C, C++, Go, GTK, and Shell scripting</b>. Also learned some other
technical concepts like Computer-Networks, Operating-System, and DBMS.Becoming a <b>DevOps</b> engineer is my long-term career goal. I want to be part of a team that
builds innovative software products that make a difference. I believe that DevOps skills are
essential to achieving this goal, and I’m excited to learn more and contribute to this field.

My goal for this project is to gain experience working on a large-scale open-source project and
make a meaningful contribution to the community. I am excited about the project because it
aligns with my interests and offers an opportunity to learn new skills and work with talented
individuals.Also wants to keep contributing to meaningful projects, to give back to the community by
sharing my knowledge, learning from the community, developing new skills, enhancing existing
projects, and building new projects.
