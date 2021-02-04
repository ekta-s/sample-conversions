Practices for Lesson 9: Using Oracle Machine Learning with Autonomous Database
==============================================================================

Practices for Lesson 9: Overview
--------------------------------

### Overview

In these practices, you create a project and a workspace in Oracle
Machine Learning.

**Note:** The initial workspace and the default project are created by
the Oracle Machine Learning service automatically when you log in to
Oracle Machine Learning for the first time. The term default applies to
the last project that you work on, and it is stored in the browser
cache. If you clear the cache, there would be no default project
selected. Then, you must select a project to work with notebooks.

### Assumptions

-   As part of your course environment, SQL Developer is installed on
    your local system.

-   All previous practices are completed successfully.

Practice 9-1: Creating Projects and Workspaces in Oracle Machine Learning
-------------------------------------------------------------------------

### Overview

In this practice, you create a project and a workspace in Oracle Machine
Learning.

A project is a container for your notebooks, and a workspace is a
container for your projects. You can own multiple projects in a
workspace.

### Tasks

Log in to your assigned Oracle Cloud account as described in the
previous practices.

Navigate to the **Autonomous Databases** page and click your service
instance name (in this example, the name of the instance is
**TRAINING**).

<img src="./media/image1.JPG" style="width:6.5in;height:1.00903in" />

On the instance information page, click **Service Console**.

<img src="./media/image2.JPG" style="width:6.5in;height:3.21181in" />

This will open a new browser tab for the service console. If prompted,
sign in to the service console as the **admin** user.

On the left hand menu, click **Administration**.

<img src="./media/image3.jpeg" style="width:6.5in;height:1.72847in" />

Click **Manage Oracle ML Users**.

<img src="./media/image4.JPG" style="width:6.5in;height:1.79653in" />

This will open a new browser tab for the Machine Learning User
Administration page, as shown below. If prompted, sign in as **admin**
user.

<img src="./media/image5.png" style="width:6.5in;height:1.6375in" />

Click
<img src="./media/image6.png" style="width:0.90983in;height:0.375in" />
and create the **MLADMIN** user, as shown below. Only enter mandatory
(\*) fields and click **Create**. For your convenience during the
practice session, you can choose to use the same password you used for
the admin account.

<img src="./media/image7.jpeg" style="width:6.5in;height:1.66875in" />

This completes the task of OML user account creation. The following
screenshot confirms you now have two OML user accounts.

<img src="./media/image8.jpeg" style="width:6.5in;height:1.33819in" />

Create projects and workspaces in Oracle Machine Learning.

Click **Oracle Machine Learning** **Home**
<img src="./media/image9.png" style="width:0.4375in;height:0.34375in" />
on the top right corner of the User Administration page. You will be
prompted to enter a username and password (in this example, it will be
**MLADMIN** and its password).

<img src="./media/image10.jpeg" style="width:6.5in;height:2.24653in" />

After you are logged in, you can see the default project and workspace
displayed on the top right side of the window. In this example,
**MLADMIN Project** is the project and **MLADMIN Workspace** is the
workspace because you logged in using the **MLADMIN** account. To create
a new project, click **New Project**.

<img src="./media/image11.png" style="width:6.5in;height:1.50139in" />

In the **Create Project** window, enter the **Name** and **Comment** for
the project and click **+.** In the **Create Workspace** window, enter
the **Name** and **Comment** for the workspace and click **OK**. Back on
the **Create Project** window, click **OK** again.

<img src="./media/image12.png" style="width:5.21391in;height:2.77381in" />

Still logged in as the **MLADMIN** user, you are now in the newly
created project and workspace.

<img src="./media/image13.png" style="width:6.5in;height:1.39514in" />

Practice 9-2: Creating and Running Notebooks in Oracle Machine Learning
-----------------------------------------------------------------------

### Overview

In this practice, you create a notebook and run it in Oracle Machine
Learning.

### Tasks

Log in to your Oracle Cloud account.

Navigate to the **Autonomous Databases** page where your instance is
listed.

Click your instance name.

Click the **Service Console** option:
<img src="./media/image14.png" style="width:0.90476in;height:0.2567in" />

Log in as the **admin** user. Here, you are signing in to the Oracle
Autonomous Transaction Processing console.

On the left hand menu, click **Administration**.

Click **Manage Oracle ML Users**.

Log in as the **admin** user. Here, you are signing in to the Oracle
Machine Learning console.

Click **Home** on the right hand top corner, highlighted in the
following screenshot:

<img src="./media/image8.jpeg" style="width:6.5in;height:1.33819in" />

Log in as the **MLADMIN** user. This time, you are signing in to the
Oracle Machine Learning console as the **MLADMIN** user.

<img src="./media/image10.jpeg" style="width:6.5in;height:2.24653in" />

Ensure you are in the **MYPROJ \[MyWorkspace\]** project and workspace,
which was created in the previous project. If not, change the project
using the **Select Project** menu option from the project/workspace
drop-down list, highlighted in the following screenshot:

<img src="./media/image15.png" style="width:6.5in;height:1.39375in" />

On the Oracle Machine Learning home page, click **Notebooks**.

<img src="./media/image16.png" style="width:6.92246in;height:1.97024in" />

In the **Notebooks** action item, click **Create**.

<img src="./media/image17.png" style="width:6.5in;height:1.65in" />

In the **Create Notebook** window, enter **Name**, **Comment,** and
**Global** as a connection string. After you click the **OK** button,
you will get your notebook ready, as in the following screenshot. In
this case, MYNOTEBOOK is the notebook name.

<img src="./media/image18.png" style="width:3.45238in;height:2.71559in" />

In the newly created notebook, you can enter SQL commands and run them.

In the notebook editor type, use the following SQL statements to fetch
data from an Oracle Database:

We are using the table name **tab** in this example as we do not have
any tables yet in this database. Ensure you have **%sql** as the first
line of the editor. Click **Run** next to the **READY** sign when you
are ready.

<img src="./media/image19.png" style="width:6.5in;height:1.17639in" />

You can run a notebook by clicking the **Run** icon next to the
**READY** sign. This is a single paragraph run. Alternatively, you can
press **Shift+Enter**.

<img src="./media/image20.png" style="width:6.5in;height:1.76597in" />

For a multiscript or multiparagraph run, which is also called an all
paragraph run, click **Run** next to the notebook name.

<img src="./media/image21.png" style="width:6.5in;height:1.76667in" />

In order to perform data analysis and data visualization, you must first
fetch data in a notebook from the data source. There are three ways in
which you can fetch data into notebooks:

Run SQL Statement

Run SQL Script

Create Notebooks

You can see these three options on the Oracle Machine Leaning home page,
as shown in the following screenshot:

<img src="./media/image16.png" style="width:6.5in;height:1.85in" />

In the next practice, you perform more tasks with SQL statements and SQL
scripts.

Practice 9-3: Creating SQL Scripts in Oracle Machine Learning
-------------------------------------------------------------

### Overview

In this practice, you create a SQL script in Oracle Machine Learning.

### Tasks

Log in to your Oracle Cloud account.

Navigate to the **Autonomous Databases** page where your instance is
listed.

Click your instance name.

Click the **Service Console**
<img src="./media/image14.png" style="width:0.90476in;height:0.2567in" />
option.

Log in as the **admin** user. Here, you are signing in to the Oracle
Autonomous Transaction Processing console.

On the left hand menu, click **Administration**.

Click **Manage Oracle ML Users**.

Log in as the **admin** user. Here, you are signing in to the Oracle
Machine Learning console.

Click **Home**
<img src="./media/image22.png" style="width:0.29328in;height:0.25595in" />
on the right hand top corner.

If you had signed out, you will be prompted to log in. Log in as the
**MLADMIN** user.

Ensure you are in the **MYPROJ \[MyWorkspace\]** project and workspace,
which was created in the previous project. If not, change the project
using the **Select Project** menu option from the project/workspace
drop-down list.

If you are continuing from the previous practice, just click the
**Application Navigation** menu (highlighted in the following
screenshot) and click **Home**.

<img src="./media/image23.png" style="width:6.5in;height:1.72986in" />

Click **Run SQL Script**.

<img src="./media/image16.png" style="width:6.5in;height:1.84997in" />

You will find the **%script** tag in the beginning of the scratch pad.
Do not delete it. Let this be the first line. Copy and paste the
following SQL script into the scratch pad:

Create table small\_table

(

name varchar(200),

id1 integer,

id2 varchar(200),

id3 varchar(200),

id4 varchar(200),

TEXT varchar(200)

);

begin

for i in 1..100 loop

insert into small\_table
values('Name\_\_\_\_\_'\|\|i,i,'ID2\_'\|\|i,'ID3\_'\|\|i,'ID4\_'\|\|i,'TEXT\_'\|\|i);

end loop;

commit;

end;

Click **Run** next to the SQL Script Scratchpad and click **OK** in the
confirmation window. The script executes and you will see the successful
execution message.

<img src="./media/image24.png" style="width:5.22024in;height:2.72224in" />

SQL scripts can be saved on your system as a **.json** file by clicking
the **Export the notebook** option.

<img src="./media/image25.png" style="width:4.68452in;height:2.98382in" />

SQL scripts that are stored as **.json** files can also be imported by
clicking **Import** in the **Notebooks** home page. This is called
**Import SQL Script**.

<img src="./media/image26.png" style="width:5.93452in;height:1.4945in" />

Practice 9-4: Running SQL Statements in Oracle Machine Learning
---------------------------------------------------------------

### Overview

In this practice, you run SQL statements in Oracle Machine Learning.

### Tasks

Log in to your Oracle Cloud account.

Navigate to the **Autonomous Databases** page where your instance is
listed.

Click your instance name.

Click the **Service Console**
<img src="./media/image14.png" style="width:0.90476in;height:0.2567in" />option.

Log in as the **admin** user. Here, you are signing in to the Oracle
Autonomous Transaction Processing console.

On the left hand menu, click **Administration**.

Click **Manage Oracle ML Users**.

Log in as the **admin** user. Here, you are signing in to the Oracle
Machine Learning console.

Click **Home**
<img src="./media/image22.png" style="width:0.29328in;height:0.25595in" />
on the right hand top corner.

Log in as the **MLADMIN** user. This time, you are signing in to the
Oracle Machine Learning console as the **MLADMIN** user.

Perform these tasks to run SQL statements.

On the Oracle Machine Learning home page, click **Run SQL Statement**.

<img src="./media/image16.png" style="width:6.5in;height:1.84997in" />

If there are SQL statements from a previous run, click **Clear
notebook** and click **OK** to clear the scratchpad.

In the SQL Query Scratchpad, type **%sql** as the first line and press
**Enter**.

Enter the SQL statement in the SQL Query Scratchpad and press **Shift +
Enter**:

The result is displayed as follows:

<img src="./media/image27.png" style="width:6.5in;height:1.72778in" />

Perform these tasks to visualize data using Oracle Machine Leaning.

Continue from the previous step and click one of the chart options.

<img src="./media/image28.png" style="width:5.14286in;height:1.37253in" />

A corresponding chart is displayed.

<img src="./media/image29.png" style="width:6.5in;height:2.30208in" />

This way, you can use the **Run SQL Statement** option to run SQL
statements and visualize data. This completes the task of running a SQL
statement.

Practice 9-5: Scheduling Jobs in Oracle Machine Learning
--------------------------------------------------------

### Overview

In this practice, you schedule a job to run in Oracle Machine Learning.

### Tasks

Log in as the **MLADMIN** user into the Oracle Machine Learning console
as shown in the previous practices. Create a notebook using the
following SQL statements. Refer to Practice 4-2 for instructions on how
to create a notebook.

This is how the notebook will look. After you are done, click the
**Application Navigation** menu and click **Home** to go back to the
home page.

<img src="./media/image30.png" style="width:6.5in;height:2.08819in" />

To create a job, click **Jobs**.

<img src="./media/image16.png" style="width:6.5in;height:1.84997in" />

Click **Create**, as shown in the following screenshot:

<img src="./media/image31.png" style="width:4.95833in;height:1.46875in" />

Enter the following details in the **Create Job** window:

Name: **MyJob1**

Notebook: Click the search icon, expand your workspace
(**MyWorkspace)**, select your notebook, and click **OK**. In this
example, we are scheduling a notebook called *new book*.

Enter the Start Date and Time. Select the current date and time.

Enter the Repeat Frequency as every **2 minutes**.

Click **Advanced Settings** and enter value 2 for **Maximum Number of
Runs** and **Maximum Failures Allowed**.

Finally, click **OK**.

The following screenshot is for a job schedule with a repeat frequency
of 2
minutes.<img src="./media/image32.png" style="width:4.58491in;height:4.71429in" />

After the job is created, its status can be tracked. The status changes
from Scheduled to Running and Success periodically.

<img src="./media/image33.png" style="width:6.5in;height:0.98889in" />

Click the job name. Select a row, that is a time frame, and click
**View**
<img src="./media/image34.png" style="width:0.73958in;height:0.25in" />
to get the run details and output along with the time stamp.

<img src="./media/image35.png" style="width:6.5in;height:0.85in" />

To stop a job, go back to the **Jobs** page. Select your job (that is,
select the row listing your job), click **Stop,** and click **OK**.

<img src="./media/image36.png" style="width:6.5in;height:1.42847in" />

To delete a job, go to the **Jobs** page, select your job (that is
select the row listing your job), click **Delete**, and click **OK**.

<img src="./media/image37.png" style="width:6.5in;height:1.40972in" />

This completes the task of creating and working with a project and
workspace in Oracle Machine Learning.
