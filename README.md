# Bug-Reports-Test-Cases---Web-Application-Testing-Examples

This repository showcases sample bug reports and test cases for web application testing. 
It demonstrates how to document functional and validation tests in a clear, structured way. 
All examples are safe for public viewing and intended to highlight QA and test design skills.

# Bug Reports & Test Cases

## Bug Reports

### 1. Validate Arabic Input Restriction for a Text Field

**Summary:**
The system should only accept Arabic text in a specific field.

**Precondition:**
User is on the relevant input page.

**Steps to Reproduce:**

1. Open the Arabic text field.
2. Enter text in another language (e.g., English).
3. Click Submit.

**Expected Result:**
The system should reject the input and show a validation message like: “Please enter text in Arabic only.”

**Actual Result / Status:**

**Environment:**
* Web application
* Browser: Any modern browser
* OS: Any OS

---

### 2. Validate English Input Restriction for a Text Field

**Summary:**
The system should only accept English text in a specific field.

**Precondition:**
User is on the relevant input page.

**Steps to Reproduce:**

1. Open the English text field.
2. Enter text in another language (e.g., Arabic).
3. Click Submit.

**Expected Result:**
The system should reject invalid characters and show a message like: “Please enter text in English only.”

**Actual Result / Status:**

**Environment:**
* Web application
* Browser: Any modern browser
* OS: Any OS

---

### 3. Validate Weak Password Rejection

**Summary:**
The system should reject weak passwords.

**Precondition:**
User is on the account registration page.

**Steps to Reproduce:**

1. Fill in all required fields.
2. Enter a weak password (e.g., “123456”).
3. Click Submit/Register.

**Expected Result:**
The system should reject weak passwords and display a warning message.

**Actual Result / Status:**

**Environment:**
* Web application
* Browser: Any modern browser
* OS: Any OS

---

### 4. Validate “Remember Me” Checkbox Behavior

**Summary:**
The system should correctly handle the "Remember Me" option during login.

**Precondition:**
User is on the login page.

**Steps to Reproduce:**
- Scenario A – “Remember Me” not selected:
  1. Login without selecting “Remember Me.”
  2. Close and reopen the application.
- Scenario B – “Remember Me” selected:
  1. Login and select “Remember Me.”
  2. Close and reopen the application.

**Expected Result:**
- Scenario A: User should be logged out.
- Scenario B: User should remain logged in.

**Actual Result / Status:**

**Environment:**
* Web application
* Browser: Any modern browser
* OS: Any OS

---

### 5. Validate Input Field for URLs

**Summary:**
URL fields should only accept valid URLs.

**Precondition:**
User is on a form with social media or website fields.

**Steps to Reproduce:**

1. Enter invalid text (e.g., “abcde”) in URL fields.
2. Click Submit.

**Expected Result:**
The system should display validation errors like: “Please enter a valid URL.”

**Actual Result / Status:**

**Environment:**
* Web application
* Browser: Any modern browser
* OS: Any OS

---
# Bug Reports & Test Cases (Public Version)

### 6. Validate “Remember Me” Checkbox Behavior

**Summary:**  
The system should correctly handle the "Remember Me" option during login.

**Precondition:**  
User is on the login page.

**Steps to Reproduce:**  
- Scenario A – “Remember Me” not selected:  
  1. Login with valid credentials without selecting “Remember Me.”  
  2. Close and reopen the application.  
- Scenario B – “Remember Me” selected:  
  1. Login with valid credentials and select “Remember Me.”  
  2. Close and reopen the application.

**Expected Result:**  
- Scenario A: User should be logged out.  
- Scenario B: User should remain logged in.

---

### 7. Validate Logo Persistence After Registration

**Summary:**  
Uploaded logos should persist after account registration.

**Precondition:**  
User is registering a new account.

**Steps to Reproduce:**  
1. Upload a logo during registration.  
2. Complete registration.  
3. Check the profile page.

**Expected Result:**  
Uploaded logo should appear in the profile and not be replaced by a default image.

---

### 8. Validate Sidebar Icons Visibility and Scroll

**Summary:**  
All sidebar icons should remain visible and scrollable.

**Precondition:**  
User is logged into the admin panel.

**Steps to Reproduce:**  
1. Open the sidebar menu.  
2. Expand options to the last item.  
3. Observe icons and scroll behavior.

**Expected Result:**  
All icons remain visible, and a scrollbar appears if content exceeds view height.

---

### 9. Validate Page Refresh Does Not Cause Errors

**Summary:**  
Refreshing a page while logged in should not cause errors.

**Precondition:**  
User is logged into their account.

**Steps to Reproduce:**  
1. Login successfully.  
2. Refresh the page.

**Expected Result:**  
User remains on the same page without errors.

---

### 10. Validate URL Input Fields Accept Only Valid URLs

**Summary:**  
URL fields should accept only valid URLs.

**Precondition:**  
User is on a form with URL input fields.

**Steps to Reproduce:**  
1. Enter invalid text (e.g., “abcde”) in URL fields.  
2. Submit the form.

**Expected Result:**  
Validation errors should appear for invalid URLs.

---

### 11. Validate Duplicate Names Do Not Conflict

**Summary:**  
The system should prevent creating two entities with the same name.

**Precondition:**  
Two entities exist with the same name.

**Steps to Reproduce:**  
1. Create Entity A with a name.  
2. Create Entity B with the same name.  
3. Try to access both entities.

**Expected Result:**  
The system prevents duplicates or generates unique identifiers.

---

### 12. Validate Name Change Updates Identifier/Slug

**Summary:**  
Changing an entity’s name should update its identifier or slug.

**Precondition:**  
Existing entity with editable name.

**Steps to Reproduce:**  
1. Change the entity name.  
2. Access entity via the updated identifier/slug.  
3. Check if old identifier still works and new identifier is valid.

**Expected Result:**  
Identifier/slug updates automatically or provides a way to update manually.

---

### 13. Validate Numeric Field Rejects Non-Numeric Input (Mobile)

**Summary:**  
Numeric fields should reject non-numeric input.

**Precondition:**  
User is on a mobile device.

**Steps to Reproduce:**  
1. Open numeric input field.  
2. Paste non-numeric text (e.g., “hello”).  
3. Observe the field’s behavior.

**Expected Result:**  
Field accepts digits only and rejects non-numeric input.


## Test Cases Table

| Test ID | Test Case Title                                    | Precondition                  | Test Steps                                                                                   | Expected Result                                                        | Actual Result / Status |
| ------- | -------------------------------------------------- | ----------------------------- | -------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------- |
| TC001   | Validate Arabic Input Restriction                  | User is on the input page     | 1. Open Arabic text field 2. Enter text in another language 3. Click Submit                  | System rejects invalid input                                           |                        |
| TC002   | Validate English Input Restriction                 | User is on the input page     | 1. Open English text field 2. Enter text in another language 3. Click Submit                 | System rejects invalid input                                           |                        |
| TC003   | Validate Weak Password Rejection                   | User on registration page     | 1. Fill fields 2. Enter weak password 3. Submit                                             | System rejects weak password                                           |                        |
| TC004   | Validate Remember Me Checkbox                      | User on login page            | 1. Scenario A: Login without selection, reopen app 2. Scenario B: Login with selection, reopen app | Scenario A: logged out; Scenario B: remains logged in                 |                        |
| TC005   | Validate URL Input Fields                          | User on form page             | 1. Enter invalid URLs 2. Submit                                                             | Validation errors displayed                                            |                        |
| TC006   | Validate Duplicate Names Do Not Conflict          | Two entities exist with same name | 1. Create first entity 2. Create second entity with same name 3. Check for conflicts       | System prevents duplicates or generates unique identifiers             |                        |
| TC007   | Validate Slug/Identifier Update After Name Change | Existing entity editable      | 1. Change entity name 2. Check updated slug or identifier                                   | Slug/identifier should update automatically                            |                        |
| TC008   | Validate Non-Numeric Input Rejection              | User on mobile device         | 1. Paste non-numeric text in numeric field                                                  | Field accepts digits only, rejects non-numeric input                   |                        |
| TC009   | Validate Page Refresh Does Not Cause Errors            | User is logged in                      | 1. Login successfully. 2. Refresh the page.                                                | User should stay on the same page without errors.                   |
| TC010   | Validate URL Input Fields Accept Only Valid URLs      | User is on a form with URL input fields | 1. Enter invalid text (e.g., "abcde") in URL fields. 2. Submit the form.                   | Validation errors should appear for invalid URLs.                    |
| TC011   | Validate Text Visibility in Search Bar (Light Theme)  | User is on a page with light theme     | 1. Set page theme to a light color. 2. Go to the search bar. 3. Observe text visibility.   | Search input and placeholder text should automatically be readable. |
| TC012   | Validate Duplicate Names Do Not Conflict              | Two entities exist with the same name  | 1. Create Entity A with a name. 2. Create Entity B with the same name. 3. Try to access both. | System should prevent duplicates or generate unique identifiers.    |
| TC013   | Validate Identifier/Slug Updates After Name Change   | Existing entity with editable name     | 1. Change the entity name. 2. Access via updated identifier. 3. Check old identifier.     | Identifier/slug updates automatically or provides manual update.    |
| TC014   | Validate Numeric Field Rejects Non-Numeric Input     | User is on a mobile device             | 1. Open numeric input field. 2. Paste non-numeric text (e.g., 'hello'). 3. Observe behavior. | Field accepts digits only and rejects non-numeric input.            |
