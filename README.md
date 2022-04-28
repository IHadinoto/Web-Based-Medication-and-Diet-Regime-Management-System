# Biomedical and Health Informatics (BIOM9450)

# Major Project: A Web-Based Medication and Diet Regime Management System

Due: Tuesday 30 th November 5 : 00 pm

Tasks
In this project you are required to design a web-based medication and diet regime management system that
would be suitable for use by a qualified health practitioner in an aged-care facility. You will not be given in-
depth details on how the tasks are to be achieved: that is up to your ingenuity, creativity and perseverance. The
medication database, as well all web pages in your application should be your own design. However, essential
user information must be entered and validated, and the referential integrity of the data maintained. In addition,
patient confidentiality is to be maintained via a secure login feature.

As a starting point, your database design should include at least four tables: a Medications table, a Diet regime
table, a Patient table, and a Practitioner table. You will very likely need other tables to tie all the information
together – but this is by your design!

The conceptual way such a system works is that a Web service running on aged-care facility system that
populates the Medications and the Diet regime tables for all residents for the upcoming week. The aged-care
facility system also delivers (in blister packs) the medications and the diet regime for each patient for the
upcoming seven days. There are three medications and Diet regime rounds: morning, afternoon, and evening.
The process is as follows:

1. A practitioner logs onto the system
2. A medications round (morning, afternoon or evening) for a particular day is selected.
3. A diet regime round (morning, afternoon or evening) for a particular day is also selected.
4. A patient is selected from a list (possibly also displaying their picture).
5. Each medication and the diet regime menu for this patient is viewed and prepared and the medication
    name, dosage, route of administration (as a minimum) are displayed. A set of rules about food, exercise,
    or beauty in the diet regime menu are also displayed. The practitioner dispenses and acknowledges
    delivery of EACH medication and the diet regime for the patient. Medications do not always have to be
    given, so the system should record such options as: given, refused, fasting, no stock, ceased. The system
    should also naturally record the name of the dispensing practitioner. If the medication for a patient is
    refused, the system should send an email to the aged-care facility’s director with patient ID and
    practitioner name.
6. Step 4 is repeated for each medication and diet regime for this patient.
7. Steps 3-5 are repeated for all patients in the facility for which the practitioner is caring.

It should be assumed that the medications and the diet regime data is available. For the sake of this project you
should choose to manually pre-populate the medications and the diet regime tables with data for the upcoming
week (i.e. the first week of December starting 30th November). You should also include data for the previous
week and have dispensed the medications and the diet regime to various (at least five) patients by at least two
practitioners. This will allow us to test the system and generate reports on medications and the diet regime
usage.

If you do not know about diet regimes, you can browse the web. Many diet regime databases are proprietary but
there are some open source collections, e.g. https://www.healthdirect.gov.au/healthy-eating-over- 60


If you do not know about types of medication you can browse the web. Many medication databases are
proprietary but there are some open source collections, e.g. [http://medlibrary.org/drugs/index.html](http://medlibrary.org/drugs/index.html)

The practitioner table should include a user name and a password for each practitioner/administrator in the
system. It can be assumed that this data already exists in appropriate tables (i.e. you do not need to create web
forms to do this data entry). Besides patient name and a photo, the patient table should also include a field to
describe what room the patient resides in the aged-care facility. The above patient data is to be entered into the
database via an appropriate web page form.

Practitioners should be able to insert new patient data into the database, as well as search, browse and edit data.
In addition, practitioners should be able to view flexible medications and diet regime summary reports (two
separate summaries) that can be configured for either all patients or a single patient and can be retrospective (for
past week) or prospective (for the upcoming week). This report should also be able to be sub-categorised by
practitioner. A sample report from a significantly more complex web-based system is shown below to give you
some ideas on report layout.

If you are unsure about what directory PHP is working from (the directory from which relative paths are
defined), use the command echo getcwd(); to display the current working directory on the page. It will be
the directory of the PHP file which is running the PHP code. A sample php file to plot a very simple chart is
included on Moodle to get you started.

Server side validation of data should be performed using PHP. You may choose to also perform some client
side data validation using JavaScript.

Report

You are expected to hand in a complete report detailing the tasks undertaken and the approaches adopted,
including database design and user interface descriptions. This should include a brief “user’s manual”. It is not
necessary to print your PHP code (unless there are particular code snippets that you want to make mention of as
we will be accessing this from the server). Please clearly explain which web page(s) to access to run your
project. Also ensure you include in your report the username and password of practitioners.


Ideally, the system should be complete and bug free. If sections of your program do not work as expected, you
should explain where and why the bug(s) occurred, and what attempts you have made to track the source of the
error. Marks will be allocated for functionality, data entry checking, integrity checking, innovative design, error
free operation, etc.. If you develop the system outside of the GSBmE computer lab you MUST check the full
functionality of the system on the GSBmE computer system (including database, web server and browser).
Many times we have had projects submitted that fail to work as expected due to incompatibility issues.

Please make sure as part of the user manual you provide sample login usernames and passwords so we
can easily check your design. NB: A non-plagiarism declaration form must be attached to your hand-in report.

Zip everything up and submit your files on Moodle but also leave the current copy on your G: drive. All
by the due date.

How will we assess the main project?

- The score will be divided as below:
- 30% of the score for individual group member contribution to the project (we will ask each member to
    run the healthcare system and provide an explanation about the scripts).
- 70% will go for the whole project. This includes the final product (60%) + written report (10%).
- Individual team member assessment will be based on the task that each team member is responsible for.

How can you deliver your Major project?

- We will give you 15 minutes to deliver your Major project to the instructor. You need to show that your
    healthcare system works without any issue.
- The healthcare system can be run either on i) your own machine; ii) Green room machines (remotely).
- You can present the Major project through Microsoft TEMAS.
- All group members should be in the presentation and must be able to run and explain the product (their
    healthcare system).

Proposed Marking Rubric (Total 100)

- Database (20)
    o Required data structures and data ( 10 ) [should be giveaway marks]
       ▪ Patient (2)
       ▪ Practitioner / Password protection (2)
       ▪ Medications (2)
       ▪ Diet regimes (2)
       ▪ Prepopulated medication data for two weeks (second week not dispensed) (2)
    o Table design (6)
       ▪ Normalisation, layout, overall design (2) [a general feel]
       ▪ Data type selection (2) [using appropriate data types]
       ▪ Constraints (2) [primary key, field constraints]
    o Relationships ( 4 )
       ▪ Justification ( 4 ) [a brief discussion in the report]
- Web functionality ( 28 )
    o Login ( 5 )
       ▪ Username / password check ( 2 )
       ▪ Logout (1)
       ▪ Behaviour, overall security (of all pages) ( 2 )
    o Medication administration and dispensing ( 4 )
       ▪ Dispensing round ( 4 )


```
o Diet regime administration and dispensing ( 4 )
▪ Dispensing round ( 4
o Practitioner tasks (1 1 )
▪ Inserting patient data (2)
▪ Search/browse/edit data (2)
▪ Display patient photo (may be pre-loaded into table) (3)
▪ Medications report ( 2 )
▪ Diet regime report ( 2 )
o Navigation ( 4 )
```
- Error checking and validation (15)
    o PHP server validation (and optional Javascript) of key fields (10)
    o SQL error handling (2) [1 for no SQL errors encountered, 1 for correct handling]
    o General user-friendliness of messages (3) [general feel]
- Web interface, design, presentation (20)
    o Web (15) [mainly a general feel for the interface, use of CSS, etc.]
    o Code (5) [style, comments, etc.]
- Report (1 7 )
    o Tasks undertaken / approaches (5)
    o Website user manual (10)


