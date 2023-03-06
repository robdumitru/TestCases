# Test Cases Samples

Below are some Test Cases that I wrote while self-learning.

_______________________________________________________________

## Login Test Cases ##

### 1. Title: Test login with correct credentials ###

**Description:**
Test the login by using correct credentials.

**Steps to Reproduce:**
1. Go to the Login Page (https://login.wordpress.org)
2. Add correct credentials
3. Observe if the user can login

**Expected result:**
The user is able to login.

**Test Data:**
- User: qatestingproject
- Pass: hjA$FiTwcsVO!IOv
_______________________________________________________________

### 2. Title: Test if login username is case sensitive ###

**Description:**
Test the login by using correct username in all caps and correct password.

**Steps to Reproduce:**
1. Go to the Login Page (https://login.wordpress.org)
2. Add correct username in all caps and correct password
3. Observe if the user can login

**Expected result:**
The user is able to login.

**Test Data:**
- User: QATESTINGPROJECT
- Pass: hjA$FiTwcsVO!IOv
_______________________________________________________________

### 3. Title: Test login with incorrect credentials ###

**Description:**
Test the login by using incorrect credentials.

**Steps to Reproduce:**
1. Go to the Login Page (https://login.wordpress.org)
2. Add incorrect credentials
3. Observe if the user can login

**Expected result:**
The user is not able to login.

**Test Data:**
- User: wrongid
- Pass: w123

_______________________________________________________________

### 4. Title: Test login without typing any password ###

**Description:**
Test the login by using correct username but no password.

**Steps to Reproduce:**
1. Go to the Login Page (https://login.wordpress.org)
2. Add correct username
3. Leave the password field empty
4. Observe if the user can login

**Expected result:**
The user is not able to login.

**Test Data:**
- User: correctid

_______________________________________________________________

### 5. Title: Test login without typing any credentials ###
  
**Description:**
Test the login by not using any credentials.
  
**Steps to reproduce:**
1. Go to the Login Page (https://login.wordpress.org)
2. Leave the credentials fields empty
3. Observe if the user can login

**Expected result:**
The user is not able to login.

**Test Data:**
- N/A
  
_______________________________________________________________

### 6. Title: Test login by inversing username & password order ###
  
**Description:**
Test the login by using correct username and correct password in inversed order
  
**Steps to reproduce:**
1. Go to the Login Page (https://login.wordpress.org)
2. Add correct username in the password field
3. Add correct password in the username field
3. Observe if the user can login

**Expected result:**
The user is not able to login.

**Test Data:**
- User: qatestingproject
- Pass: hjA$FiTwcsVO!IOv
  
_______________________________________________________________

### 7. Title: Test if login password is case sensitive ###
  
**Description:**
Test the login by using correct username and correct password with all caps.
  
**Steps to reproduce:**
1. Go to the Login Page (https://login.wordpress.org)
2. Add correct username and correct password in all caps
3. Observe if the user can login

**Expected result:**
The user is not able to login.

**Test Data:**
- User: QATESTINGPROJECT
- Pass: GJA$FITWCSVO!IOV
  
_______________________________________________________________

### Title: Test if the "Remember me" fuction works properly ###
  
**Description:**
Test the remember me function by closing the page after logging in while "Remember me" checkbox is checked.
  
**Steps to reproduce:**
1. Go to the Login Page (https://login.wordpress.org)
2. Add correct credentials
3. After succesfully logged in close the page/browser
4. Open the website again (https://wordpress.org)
5. Observe if the user remained logged in

**Expected result:**
The user remains logged in.

**Test Data:**
- User: qatestingproject
- Pass: hjA$FiTwcsVO!IOv
  
_______________________________________________________________

### Title: Test if the website can handle XSS ###
  
**Description:**
Test the website response by using cross-site scripting.
  
**Steps to reproduce:**
1. Go to the Login Page (https://login.wordpress.org)
2. Add any XSS script into the credentials field
3. Observe the website behavior

**Expected result:**
The website ignores the script and tells the user that the credentials are wrong.

**Test Data:**
- XSS: <script>alert(1) </script>
  
_______________________________________________________________

### Title: "Test search bar popular searches functionality ###
  
**Description:**
Test the search bar popular searches by clicking on the options.
  
**Steps to reproduce:**
1. Go to EMAG Website (https://www.emag.ro)
2. Open the search bar
3. Click on the first option prompted to user on the popular searches tab
4. Observe if the user is taken to a page with relevant related products

**Expected result:**
The search bar popular searches function properly.

**Test Data:**
- N/A
  
  _______________________________________________________________

### Title: Test search bar with valid item names ###
  
**Description:**
Test the search bar by using valid item names.
  
**Steps to reproduce:**
1. Go to EMAG Website (https://www.emag.ro)
2. Open the search bar
3. Search for "lapte"
4. Observe if the search bar is showing the user relevant items to his search

**Expected result:**
The search bar is showing the user relevant items to his search.

**Test Data:**
- lapte

_______________________________________________________________

### Title: Test search bar with diacritics ###
  
**Description:**
Test the search bar by using diacritics.
  
**Steps to reproduce:**
1. Go to EMAG Website (https://www.emag.ro)
2. Open the search bar
3. Search "cârpă"
4. Observe if the search bar finds relevant results

**Expected result:**
The user can find relevant products by using
diacritics.

**Test Data:**
- cârpă

_______________________________________________________________

### Title: Test if the search bar can handle XSS ###
  
**Description:**
Test the search bar by using a cross-site script.
  
**Steps to reproduce:**
1. Go to EMAG Website (https://www.emag.ro)
2. Open the search bar
3. Add any XSS script into the search bar
4. Observe the website behavior

**Expected result:**
The search function ignores the injected script and tries to show the user appropriate and relevant items.

**Test Data:**
- XSS: <script>alert(1) </script>
