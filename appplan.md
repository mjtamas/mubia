*MUBIA -- Multi Business Access*

2\. Goals of the application

-   Providing access to a building with multiple offices

-   Achieving greater security

-   Providing useful information for employers

-   Facilitate accounting

3.Target audience

-   Employers

-   Employees

-   Building administrator

-   Security staff

4\. User interactions

-   ![](.//media/image1.png){width="1.0159722222222223in"
    height="0.8569444444444444in"}access the building (check in)

-   exit the building (check out)

-   go on vacation

-   ask for assistance

-   ![](.//media/image2.png){width="1.070138888888889in"
    height="1.070138888888889in"}manage a firm ( update )

-   manage the firms employees (add/update/remove)

-   get information (charts , notifications) about employees

```{=html}
<!-- -->
```
-   ![](.//media/image3.png){width="0.9902777777777778in"
    height="1.1756944444444444in"}grant/revoke access from users

-   get information about users ( check in/out timestamps)

-   get notifications ( when users ask for assistance)

-   open/lock the system

-   ![](.//media/image4.png){width="1.3375in"
    height="1.2826388888888889in"}manage firms (add/remove)

-   manage employers (add/remove)

-   manage security staff (add/remove)

-   get information (charts, notifications) about firms

5\. Back-end technologies

1.  PHP

2.  Laravel 7.x framework

3.  MySQL

4.  ??

5.  ??

6\. Front-end technologies

1.  HTML

2.  CSS

3.  JavaScript

4.  ??

5.  ??

7\. Database tables

Employees

-   id

-   name

-   password

-   firm_id

-   has_access

-   checked_in

-   checked_out

-   on_vacation

Employers

-   id

-   name

-   password

-   firm_id

-   admin_id

-   has_access

Administrators

-   id

-   name

-   password

Securitymembers

-   id

-   name

-   password

-   admin_id

-   system_opened

-   system_locked

Firms

-   id

-   name

-   admin_id

8\. Database relations ( Eloquent)

-   an employee belongsTo a firm

-   a firm hasMany employees

-   an employer hasOne firm

-   a firm hasMany employers

-   an employee hasMany employers Through firm

-   a firm hasOne administrator

-   an employer hasOne administrator

-   a security member hasOne administrator

-   an administrator belongsToMany firms

-   an administrator belongsToMany employers

-   an administrator belongsToMany security members

9\. Database Schema Design

[http://www.laravelsd.com/share/HEvLTt]()

![](.//media/image5.png){width="6.6930555555555555in"
height="3.209722222222222in"}
