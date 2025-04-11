---
layout: page
name: SubwooferDestroyer
title: SQL Injection
---

In this challenge we are trying to use SQL Injection to gain access to the webapp and get the flag!
![image](images/BHS_SQL_CHALLENGE/sql_challenge_start.png)

## SQL Injection

The unsafe query is ```SELECT * FROM users WHERE username = '{username}' and password = '{password}' ```

This query is unsafe since it directly adds user input into the query and can execute code.

![image1](images/BHS_SQL_CHALLENGE/sql_input.png)

After using the input ```admin'; --``` in the admin input we get into the webapp home.

![image2](images/BHS_SQL_CHALLENGE/after_login.png)

Once in the webapp we can go into the admin profile, where we can see the post that contains the flag.

![image3](images/BHS_SQL_CHALLENGE/challenge_flag.png)

Now we have the flag!.
