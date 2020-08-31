# **Test Login_Page**

 **Task** :Test the new Sign In page for the given link [Link for the above Signin page](https://pages.github.com/).
##### 1.**Scenario**:Login to fillr home page with valid Credentials
**Given** *User is navigating on fillr Login Page*
**When** *User enters username as "validuser" and password as "validpassword"*
**Then** *User successfully logs in and lands on fillr home page*
#### *Testcases* 
| TEST | EXCEPTED |
| ------ | ------ |
| Enter valid password | The password should display in asterick symbols only |
| click text 'Show' underline | The field should display valid password in characters from asterick |
| click 'Logout' on the fillr home page | The application should take user back to login page |
| click browser back,forward or refresh button on login page | The application should redirects on login page |
| Perform click Action 'Signin'| The application should display spinner icon and should not visible usename and password on url while redirecting to fillr home page |
| Enter valid credentials before activation | The application should not allow user to successfully login |
| Verify activation link expiry | The user is not successfully activated |

##### 2.**Scenario**:New User registration with fillr
**Given** *New Account is created with fillr* 
**When** *User enter details and complete registration on ‘Create an account’*
**Then** *User successfully logs in and lands on fillr home page*
#### *Testcases* 
| TEST | EXCEPTED |
| ------ | ------ |
| Reenter Registered account details | The Application should not successfull in registration and display message that account is already with fillr  |
| Restrict user to enter password with atlist 1 special character,1 numeric,1 Uppercase and limit to 8 characters | The application should not allow to save untill entered in correct format |
| click Recaptcha checkbox | The application should sucessfully save new Registration |


##### 3.**Scenario**:Perform Action 'Forgot your password?'
**Given** *User is successfully login’s with new Credentials*
**When** *User receives new reset password email to validate the email address*
**Then** *User successfully logs in and lands on fillr home page*
#### *Testcases* 
| TEST | EXCEPTED |
| ------ | ------ |
| Enter invalid email address from credentials | The Application should not send reset password link and display error message  |
| Verify reset password link expiry |  The Application should not allow to reset new password if expired |

##### 4.Scenario:Login to fillr with invalid Credentials
**Given** *User redirecting on fillr Login Page with validation error message*
**When** *User tries to login with invalid Credentials*
**Then** *User is not landing on fillr home page*
#### *Testcases* 
| TEST | EXCEPTED |
| ------ | ------ |
| Enter valid username and invalid password | The Application should redirects and display error message  |
| Enter invalid username and valid password |  The Application should redirects and display error message  |
| Enter both invalid username and password | The Application should redirects and display error message |
| Verify invalid Credentials for more than 3 attempts | The Application should block user and display the error message |

##### 5.Scenario:Login to fillr with void Credentials
**Given** *User is redirecting on fillr Login Page with error message*
**When** *User leaves both Credentials unfilled*
**Then** *User is not landing on fillr home page*
#### *Testcases* 
| TEST | EXCEPTED |
| ------ | ------ |
| Unfill both credential testfields  | The Application should highlight textfields and display error message  |
| Unfill username and enter valid Password |  The Application should highlight username textfield and display error message  |
| Unfill username and enter invalid Password | The Application should highlight both textfields and display error message |
| Enter valid username and unfill Password | The Application should highlight password textfield and display error message |
| Enter invalid username and unfill  Password | The Application should highlight username textfield and display error message |

##### 6.Scenario:Login to fillr from 'Google'
**Given** *User is navigating on Google signin page*
**When** *User click on Action button ‘Continue with Google’*
**Then** *User is successfully land on fillr home page*
#### *Testcases* 
| TEST | EXCEPTED |
| ------ | ------ |
| Display message on the header of signin page | The Application should display 'Login Goggle account with 'fillr'(Company URL)|
| Allow to select one account from the Google accounts | The Application should land on fillr homepage with selected account |
| Click Action button new account | The Appliction should land on Google sign in page |

##### 7.Scenario:Login to fillr from Facebook
**Given** *User is navigating on Facebook signin page*
**When** *User click on Action button ‘Continue with Facebook’*
**Then** *User is successfully land on fillr home page*
#### *Testcases* 
| TEST | EXCEPTED |
| ------ | ------ |
| | Apply same test coverage from the scenario 6 |

##### 8.Scenario:Login to fillr from Apple
**Given** User is navigating on Apple signin page
**When** User click on Action button ‘Continue with Apple’
**Then** User is successfully land on fillr home page
#### *Testcases* 
| TEST | EXCEPTED |
| ------ | ------ |
| | Apply same test coverage from the scenario 6 |

##### 9 .Scenario:Login to fillr home page with valid/invalid/void Credentials (Cross Browsers)
#### *Testcases* 
| TEST | EXCEPTED |
| ------ | ------ |
|Crome,Safari,Firefox and Inter Explorer | Apply same test coverage from the scenario 1,4,5 |

##### 10 .Scenario:Login to fillr home page with valid/invalid/void Credentials (Mobile app on multiple devices)
#### *Testcases(Functionality)* 
| TEST | EXCEPTED |
| ------ | ------ |
|Android,Safari | Apply same test coverage from the scenario 1,4,5 | 
| Download and install the app | The App should be successfully installed |
| Auto installation of App with new version | The App should work/behave as expected |

#### *Testcases(Usability)* 
| TEST | EXCEPTED |
| ------ | ------ |
|App Buttons should be user-friendly size.|
| App Buttons location, style, etc should consistent within the app |
 |App Icons should be consistent within the application |
| Zoom in and out facilities should work as expected |
| The Mobile device keyboard should be minimized and maximized easily |

#### *Testcases for Desktop and Mobile (Security)* 
| TEST |
| ------ |
| 1. The Application should not permit an attacker to access credentials without proper authentication. This includes making sure the communications with the backend are properly secured with Database. ex: The Password should be securely sync with database and stored in encrypted format |
|2. Verify the strong password protection system within the mobile app/System. ex: Autofill Password feature from the Browsers settings or provide MFA security option while registration or settings related to Cookies or clear browing data |
|3. Analyze and prevent any vulnerabilities from different data streams. ex: The Database should detect/identify if any unauthenticated activity |




  
   
