In this reading, it will explain many defense mechanisms


# Handling User Access
Most web applications use these mechanisms when they are handling access:
>Authentication
<br>

>Session management
<br>


>Access control<br>

A defeat in any of these mechanism will lead to a gain of unrestircted access to the attacker.

### Authentication
Authentication mechanism is logically the most basic dependency in an application's handling of user access. because of the fact that it is the most basic dependency, the range of vulnerability is also huge. It has huge range of defects in both design and implementation. 

> Tip : When you are attacking a website, you should give a big atten to these authentication-related functions and a lot of times you get access to sensitive data and functionality by the attack on these systems.


### Session Management

This mechanism is when the Authentication session has passed and when the user goes to the next part and gets a visual of various types of informations, making a series of HTTP requests. Then if you think about it, there should be a way for the web application to identify from the various HTTP requests which is who. So what many web applicatoins use is that they give a token to a user and make their token to return in each subsequent HTTP requests. HTTP cookies are a standard way token. In terms of attack, the token takes up a big job. And the defects on this mechanism come from how the token is generated. If there is a defect in how the token is generated and if the attacker gains a specific token, the attacker can mimic as the user and gain sensitive informations.


### Access Control

After both mechanisms explained are safely completed, the web application needs to decide if the user is authorized for the data that he is requesting. Developers oftenly make flaws in this mecahnism so it is always good to spend time on looking for these vulnerabilities. 

# Handling User Input

As a recall, all user inputs are untrusted. Often times a lot of attacks are based on unexpected inputs, causing actions that was not a purpose of the developer. So these days "input validation" seems like a necessary defense against these unexpected inputs, where it tests out user's inputs from the web application.

