

## Description:
 
The Simple Gym Management System In Laravel/MySQL is a mini project for keeping records of members in the gym. Talking about the project, it contains an admin side from where can manage all the timetables and records of the gym users easily.  

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; `The administration part consists of 4 types of managers who can enter the system`  

1- `Admin`  :    
&nbsp; &nbsp; &nbsp; &nbsp; Admin will have access to everything in the system,he can see any links or make any action Gym Manager   
&nbsp; &nbsp; &nbsp; &nbsp; and City Manager can do with these extra functionalities.    

2- `City Manager` :    
&nbsp; &nbsp; &nbsp; &nbsp; City Manager can do what Gym Manager do with extra functionalities … like he can see all gyms in his city and  
&nbsp; &nbsp; &nbsp; &nbsp; make CRUD on any gym or gym manager in his city.  

3- `Gym Managers` :  
&nbsp; &nbsp; &nbsp; &nbsp; Gym Manager can CRUD training sessions and assign coaches to these sessions, also he can buy training  
&nbsp; &nbsp; &nbsp; &nbsp; package for a user through stripe.  

4- `coach` :  
&nbsp; &nbsp; &nbsp; &nbsp; Can only see the sessions in which he trains.  

5- `User` (It will be API only) :  
&nbsp; &nbsp; &nbsp; &nbsp; Cann't access the system because it is for the administration only, but there is an endpoint (API) for the user.   

instalation:
 
&nbsp; &nbsp; &nbsp; &nbsp; Run migration to create dababas tables use a command ` $ php artisan migrate `.

`Step 6` :    
&nbsp; &nbsp; &nbsp; &nbsp; Run data seed to create fake data in your database use a command ` $ php artisan db:seed `.  

OR you can shorten the previous two steps (5 , 6) by using this command ` $ php artisan migrate:fresh --seed `.  


- Now `226` Accounts have been created on the system, distributed as follows :  
The first two accounts are for `admin`.    
From 3 to 26 are `cityManager`.  
From 27 to 66 are `gymManager`.  
From 67 to 126 are `coach`.  
From 127 to 226 are `user`.  
All created accounts have a unified password `123456`.  


  
&nbsp; &nbsp; &nbsp; &nbsp; To create a new admin account use a command  

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ` $ php artisan create:admin --email=admin2@admin.com --password=123456 `.  

`Step 8`:    
&nbsp; &nbsp; &nbsp; &nbsp; Run schedule use a command `php artisan schedule:work`   
&nbsp; &nbsp; &nbsp; &nbsp; then use a command `php artisan notify:users-not-logged-in-for-month`






## author
soufiane refai : Soufiane.1refai@gmail.com