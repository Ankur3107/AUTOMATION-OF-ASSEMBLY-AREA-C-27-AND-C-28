# AUTOMATION-OF-ASSEMBLY-AREA-C-27-AND-C-28

# Step 1: Creation and setting up of the database for the project :

The major entities to be involved as tables and their major attributes in the database will be as under: 

Job (Job ID, Machine Id, Company ID, Start Date, Worker 1 ID, Worker 2 ID, Current Phase 1 ID, Current Phase 2 ID, Cause of Delay)

Machine (Machine ID, active status (0/1),working(0/1))

Admin (ID, Name, Password)

Stats Viewer (ID, Password)

Phase (Phase ID, Phase Name, Phase order (sequence in order),Phase Duration)

Holidays (Holiday ID, Date, Holiday Name)

Worker (Worker ID, Worker Name, Group Leader (0/1))

Customer (Customer ID, Customer Name)

Along all this, a central calendar will be maintained to calculate work hours and other associated tasks)

Additionally, tables and attributes will be added inside the database, as the work progresses and needs generate, which may not seem trivial right now, with permission/consent of the designated authority.



# Step 2: Setting up the front end of the project :

The front end, as of our understanding will consist of three interfaces.

1.	Machine specific phase input interface (At each station)
2.	Stats viewer interface (central to the visiting manager/authority)
3.	Admin Panel

 1.Machine specific phase input interface
    
This interface will be specific/unique to every machine/station.
The main design will contain a headings including the machine id, job id and customer name, along with a status indicator that whether the machine is in delay or not. 
The primary input frame will be an array of buttons which will be numbered or marked as different phases in order. The worker on the machine will have to click the phase button as soon as he completes that particular phase. It will be maintained that he can click a phase only if all preceding phases are complete. The parallel phases will be also be maintained. If by accident he/she clicks a phase which is not completed, he can just re-click it to revert back (same in case of accidently clicking more than one buttons, by re-clicking them in reverse order) 
There will be an additional drop down list of causes of delay which will be maintained by the worker/supervisor for each machine, if it goes in delay. 


 2.Stats viewer interface
    
This interface will be central to a visiting room or as such.
The main interface will consist of two-three pages.
The first page will be an option to choose C-28 or C-27
The second page will be a graphic map of the assembly area chosen, in an order and the topography in which the machines are set.
The machines will show up in 2 different colors based on whether they are active or not.
On hovering over a particular machine, it will show the machine id, job id and customer currently on that machine.
On clicking the machine, a machine specific window will open up showing primarily all phases complete in a graphic manner, delay status, currently maintained cause of delay.

Also there will be a list of generate report buttons, that may include generating a timeline of completion of every phase of current job, generating a list of customers who had been given this machine, reports of all jobs ever done on this machine, reports of all workers who worked on this machine and from when to when, (and ALSO ALL ADDITIONAL REPORTS THE AUTHORITIES REQUIRE US TO GENERATE IN THE SUBSEQUENT PROPOSAL)

We are also willing to put some generate report buttons on the assembly window and the option window preceding it , like generating customer data report , employee evaluation report , machine performance report , and again ALL ADDITIONAL REPORTS THE AUTHORITIES REQUIRE US TO GENERATE IN THE SUBSEQUENT PROPOSAL


 3.ADMIN PANEL
    
  The admin panel will be a handler friendly panel that will be central to the admin.
First of all, admin would have privileges to edit his/her password and create another admin.

Like all general admin panels, the admin will be able to see data in various tables through gridview and update them manually, if interface malfunctions.

The main interface will consist of several Add functionalities, like Add machine, Add holiday, add worker, Add customer, add phase, along with delete privileges for all of them. Also there will be edit functionalities for attributes associated with all these through gridview, mostly involving drop down lists for major changes

The major work for admin, will be adding a job, whenever there is a new job to be assigned. He/she will choose one out all working non-active machines. And with the help of drop down lists for workers, group leaders, customers available he will assign the attributes to the job.

Added privileges to admin will be updated as and when the management requires us or when during development, we feel a need for it.



# Step 3: Setting up the back end :

The back end will be optimized and in line with the various features of front end and database.

# Step 4: Testing and deployment

Unit testing, regression testing and final system testing will be maintained by us. We will await instructions on the mode of onsite testing, and deployment.



