## Part 2: Configuring osTicket - A Beginner's Guide (With Explanations and Screenshots)

Now that osTicket is installed, we'll set it up to work for your organization. We'll cover important settings like roles, departments, and how tickets are handled.

**1. Accessing osTicket (Getting Started)**

* **Why?** We need to log in to osTicket to make changes.
* **Admin/Analyst Login:**
    * Open your web browser and go to `http://localhost/osTicket/scp/login.php`.
    * Enter the username and password you set up during the installation.
    * **Screenshot Hint:** Once logged in to the admin panel, take a screenshot of the main dashboard. This confirms successful login.
* **End User Portal:**
    * This is where your customers will go to create tickets. The address is `http://localhost/osTicket`.
* **Understanding the Panels:**
    * The **Admin Panel** is for setting up osTicket.
    * The **Agent Panel** is for managing tickets and users.

**2. Configuring Roles (Setting Permissions)**

* **Why?** Roles let you control what agents can do.
* **Admin Panel -> Agents -> Roles:**
    * Click "Add New Role."
    * Name: `Supreme Admin` (Or something like "IT Manager").
    * Check all the boxes to give this role full access.
    * **Explanation:** This role will have all the permissions to do anything inside of osTicket.
    * **Screenshot Hint:** Take a screenshot of the "Add New Role" page with the permissions selected.
* **Useful Addition:** Create another role called "Help Desk Agent" with limited permissions, only allowing them to work tickets.

**3. Configuring Departments (Organizing Tickets)**

* **Why?** Departments help route tickets to the right people.
* **Admin Panel -> Agents -> Departments:**
    * Click "Add New Department."
    * Name: `SysAdmins` (Or "IT Department").
    * Set the department's email and other settings.
    * **Explanation:** Departments help keep tickets organized. For example, you might have a "Help Desk" department and a "Network" department.
    * **Screenshot Hint:** Take a screenshot after you have created a department.
* **Useful Addition:** Create a second department called "Help Desk".

**4. Configuring Teams (Working Together)**

* **Why?** Teams allow agents from different departments to work together.
* **Admin Panel -> Agents -> Teams:**
    * Click "Add New Team."
    * Name: `Online Banking` (Or "Project Support").
    * Add agents from different departments to the team.
    * **Explanation:** Teams are useful when you need people from different departments to work on the same issue.
    * **Screenshot Hint:** Take a screenshot of the team after you have added agents to it.

**5. Allowing Ticket Creation (User Access)**

* **Why?** We need to control who can create tickets.
* **Admin Panel -> Settings -> User Settings:**
    * Uncheck "Unregistered users can create tickets."
    * Check "Require registration and login to create tickets."
    * **Explanation:** This ensures that only registered users can create tickets.
    * **Screenshot Hint:** Take a screenshot of the User Settings page.

**6. Configuring Agents (Adding Staff)**

* **Why?** Agents are the people who will work on tickets.
* **Admin Panel -> Agents -> Add New:**
    * Add new agents with their names, emails, and departments.
    * Example:
        * Jane (Department: `SysAdmins`)
        * John (Department: `Help Desk`)
    * **Explanation:** Agents are the ones who respond to and resolve tickets.
    * **Screenshot Hint:** Take a screenshot of the agent list after adding new agents.

**7. Configuring Users (Adding Customers)**

* **Why?** Users are the people who create tickets.
* **Agent Panel -> Users -> Add New:**
    * Add new users with their names and contact information.
    * Example:
        * Karen
        * Ken
    * **Explanation:** Users are your customers or employees who need help.
    * **Screenshot Hint:** Take a screenshot of the user list after adding new users.

**8. Configuring SLAs (Setting Time Limits)**

* **Why?** SLAs set time limits for responding to and resolving tickets.
* **Admin Panel -> Manage -> SLA:**
    * Click "Add New SLA Plan."
    * Example:
        * Sev-A (Grace Period: 1 hour, Schedule: 24/7)
        * Sev-B (Grace Period: 4 hours, Schedule: 24/7)
        * Sev-C (Grace Period: 8 hours, Business Hours)
    * **Explanation:** SLAs help ensure that tickets are handled in a timely manner.
    * **Screenshot Hint:** Take a screenshot of the created SLA.

**9. Configuring Help Topics (Categorizing Tickets)**

* **Why?** Help topics help users categorize their tickets.
* **Admin Panel -> Manage -> Help Topics:**
    * Click "Add New Help Topic."
    * Example:
        * Business Critical Outage
        * Personal Computer Issues
        * Password Reset
    * **Explanation:** Help topics make it easier to route tickets to the right department.
    * **Screenshot Hint:** Take a screenshot of the Help Topics list.
* **Useful Addition:** Create a help topic called "New Employee Onboarding".

**10. Knowledge base (Self Help)**

* **Why?** A knowledge base lets users find answers to problems themselves.
* **Admin Panel -> Knowledgebase -> Articles:**
    * Click "Add New Article".
    * Create an article that will help users solve a common problem.
    * **Explanation:** This allows users to find solutions without creating a ticket.
