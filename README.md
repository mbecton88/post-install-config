## Part 2: Configuring osTicket - A Beginner's Guide (With Explanations and Screenshots)

Now that osTicket is installed, we'll set it up to work for your organization. We'll cover important settings like roles, departments, and how tickets are handled.

**1. Accessing osTicket (Getting Started)**

* **Why?** We need to log in to osTicket to make changes.
* **Admin/Analyst Login:**
    * Open your web browser and go to `http://localhost/osTicket/scp/login.php`.
    * Enter the username and password you set up during the installation.
   ![image](https://github.com/user-attachments/assets/7e02c746-1678-4eaa-a794-4242a9e594fb)
    ![image](https://github.com/user-attachments/assets/e1b0976b-b820-4939-9d42-223cdbfcdfa9)

* **End User Portal:**
    * This is where your customers will go to create tickets. The address is `http://localhost/osTicket`.
   ![image](https://github.com/user-attachments/assets/f1d65674-5322-4ad8-8691-fe54b678e3ef)
* **Understanding the Panels:**
    * The **Admin Panel** is for setting up osTicket.
      ![image](https://github.com/user-attachments/assets/02d17b51-f61d-4443-a88a-2c13d3cda141)
    * The **Agent Panel** is for managing tickets and users.(This is the screenshot from earlier after you first logged into the admin page).

**2. Configuring Roles (Setting Permissions)**

* **Why?** Roles let you control what agents can do.
* **Admin Panel -> Agents -> Roles:**
  ![image](https://github.com/user-attachments/assets/2276dd2b-9d16-4c89-a2ca-78030becfddb)
    * Click "Add New Role."
    * Name: `Supreme Admin` (Or something like "IT Manager").
  ![image](https://github.com/user-attachments/assets/3af0972c-9fae-4ada-8ab7-fd38ebfb4d0e)
    * Check all the boxes to give this role full access.
  ![image](https://github.com/user-attachments/assets/708b8944-beae-41b5-9c1f-8acd777ad3a3)
    * **Explanation:** This role will have all the permissions to do anything inside of osTicket.
* **Useful Addition:** Create another role called "Help Desk Agent" with limited permissions, only allowing them to work tickets.

**3. Configuring Departments (Organizing Tickets)**

* **Why?** Departments help route tickets to the right people.
* **Admin Panel -> Agents -> Departments:**
    * Click "Add New Department."
  ![image](https://github.com/user-attachments/assets/503ee2c3-cce2-40bf-a2cb-dbf18517e940)
    * Name: `SysAdmins` (Or "IT Department").
    * Set the department's email and other settings.
    * **Explanation:** Departments help keep tickets organized. For example, you might have a "Help Desk" department and a "Network" department.
    

**4. Configuring Teams (Working Together)**

* **Why?** Teams allow agents from different departments to work together.
* **Admin Panel -> Agents -> Teams:**
    * Click "Add New Team."
    * Name: `Online Banking` (Or "Project Support").
    * Add agents from different departments to the team.
    * **Explanation:** Teams are useful when you need people from different departments to work on the same issue.
   ![image](https://github.com/user-attachments/assets/94021418-a558-4b3a-a873-911075b419d3)


**5. Allowing Ticket Creation (User Access)**

* **Why?** We need to control who can create tickets.
* **Admin Panel -> Settings -> User Settings:**
    * Uncheck "Unregistered users can create tickets."
    ![image](https://github.com/user-attachments/assets/121f82c4-2461-45e0-a95b-fff0ccc014ca)
    * **Explanation:** Allows users that are not registered to submit tickets.
 
      
**6. Configuring Agents (Adding Staff)**

* **Why?** Agents are the people who will work on tickets.
* **Admin Panel -> Agents -> Add New:**
    * Add new agents with their names, emails, and departments.
    * Example:
        * Jane (Department: `SysAdmins`)
        * John (Department: `Help Desk`)
  ![image](https://github.com/user-attachments/assets/c983298c-f41f-4d3e-badf-e1a52656abf9)
    * **Explanation:** Agents are the ones who respond to and resolve tickets.
    

**7. Configuring Users (Adding Customers)**

* **Why?** Users are the people who create tickets.
* **Agent Panel -> Users -> Add New:**
    * Add new users with their names and contact information.
    * Example:
        * Karen
        * Ken
     ![image](https://github.com/user-attachments/assets/78337e23-25a2-4237-9ea1-3dc91e4def57)
    * **Explanation:** Users are your customers or employees who need help.
    

**8. Configuring SLAs (Setting Time Limits)**

* **Why?** SLAs set time limits for responding to and resolving tickets.
* **Admin Panel -> Manage -> SLA:**
    * Click "Add New SLA Plan."
    * Example:
        * Sev-A (Grace Period: 1 hour, Schedule: 24/7)
        * Sev-B (Grace Period: 4 hours, Schedule: 24/7)
        * Sev-C (Grace Period: 8 hours, Business Hours)
          ![image](https://github.com/user-attachments/assets/7fcc8b94-6742-4457-8cca-d34fa8dddc63)
          ![image](https://github.com/user-attachments/assets/5f5db78c-5740-4b9d-8d49-40f6d11e9f17)
    * **Explanation:** SLAs help ensure that tickets are handled in a timely manner.
   

**9. Configuring Help Topics (Categorizing Tickets)**

* **Why?** Help topics help users categorize their tickets.
* **Admin Panel -> Manage -> Help Topics:**
    * Click "Add New Help Topic."
    * Example:
        * Business Critical Outage
        * Personal Computer Issues
        * Password Reset
    * **Explanation:** Help topics make it easier to route tickets to the right department.
    


