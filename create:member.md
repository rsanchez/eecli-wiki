Create a new member. If you omit a password, one will be generated for you. If you omit an email, the username will be used as the email address. If you omit a member group, the default member group for your system will be used.

```
# create a member with same username & email
eecli create:member your.email@site.com

# create a member with different username & email
eecli create:member --email="your.email@site.com" your_username

# create a member with the specified screen name
eecli create:member --screen_name="Your Name" your.email@site.com

# create a member with the specified password
eecli create:member --password="so48jf48jss4sk" your.email@site.com

# create a superadmin
eecli create:member --member_group=1 your.email@site.com
```