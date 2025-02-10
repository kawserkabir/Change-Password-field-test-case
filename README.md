# Change Password Field Test Cases

This document contains test cases for the **Change Password** functionality. Use these test cases to validate the behavior of the change password feature in your application.

## Test Cases

### 1. Verify Field Labels
- **Test Case ID**: TC001
- **Description**: Verify that the field labels ("Current Password", "New Password", "Confirm New Password") are displayed correctly.
- **Steps**: Open the change password page and observe the labels.
- **Expected Result**: Field labels should be displayed as per the design specifications.

### 2. Verify Placeholder Text
- **Test Case ID**: TC002
- **Description**: Verify that placeholder text is present in all password fields.
- **Steps**: Open the change password page and observe the placeholder text.
- **Expected Result**: Placeholder text should guide the user, e.g., "Enter your current password."

### 3. Current Password Field Validation
- **Test Case ID**: TC003
- **Description**: Verify validation for the current password field when left blank.
- **Steps**: Leave the "Current Password" field blank and attempt to submit the form.
- **Expected Result**: An error message like "Current password is required" should appear.

### 4. New Password Field Validation
- **Test Case ID**: TC004
- **Description**: Verify validation for the new password field when left blank.
- **Steps**: Leave the "New Password" field blank and attempt to submit the form.
- **Expected Result**: An error message like "New password is required" should appear.

### 5. Confirm Password Field Validation
- **Test Case ID**: TC005
- **Description**: Verify validation for the confirm password field when left blank.
- **Steps**: Leave the "Confirm New Password" field blank and attempt to submit the form.
- **Expected Result**: An error message like "Confirm password is required" should appear.

### 6. Password Mismatch
- **Test Case ID**: TC006
- **Description**: Verify error message when "New Password" and "Confirm New Password" do not match.
- **Steps**: Enter different values in the "New Password" and "Confirm New Password" fields and submit the form.
- **Expected Result**: An error message like "Passwords do not match" should appear.

### 7. Minimum Password Length
- **Test Case ID**: TC007
- **Description**: Verify that the new password requires a minimum length.
- **Steps**: Enter a password shorter than the required length (e.g., 5 characters) and submit the form.
- **Expected Result**: An error message like "Password must be at least 8 characters" should appear.

### 8. Strong Password Validation
- **Test Case ID**: TC008
- **Description**: Verify that the new password meets strength requirements (e.g., uppercase, lowercase, number, special character).
- **Steps**: Enter a password that does not meet the strength criteria and submit the form.
- **Expected Result**: An error message like "Password must contain an uppercase letter, a number, and a special character" should appear.

### 9. Successful Password Change
- **Test Case ID**: TC009
- **Description**: Verify that the password is successfully changed when all fields are valid.
- **Steps**: Enter the current password, a valid new password, and confirm the new password. Submit the form.
- **Expected Result**: A success message like "Your password has been changed successfully" should appear.

### 10. Invalid Current Password
- **Test Case ID**: TC010
- **Description**: Verify error message when the current password is incorrect.
- **Steps**: Enter an incorrect current password and submit the form.
- **Expected Result**: An error message like "Current password is incorrect" should appear.

### 11. Password Reuse Restriction
- **Test Case ID**: TC011
- **Description**: Verify that the user cannot reuse the last N passwords.
- **Steps**: Enter a previously used password as the new password and submit the form.
- **Expected Result**: An error message like "You cannot reuse your last 5 passwords" should appear.

### 12. Field Masking
- **Test Case ID**: TC012
- **Description**: Verify that all password fields mask the input characters.
- **Steps**: Observe the input while typing in any of the password fields.
- **Expected Result**: Characters should be masked with asterisks or dots.

### 13. Show/Hide Password Toggle
- **Test Case ID**: TC013
- **Description**: Verify the functionality of the "Show/Hide Password" toggle for all fields.
- **Steps**: Click on the toggle button for each password field and observe the input visibility.
- **Expected Result**: Password should be visible when "Show" is selected and masked when "Hide" is selected.

### 14. Session Expiry Handling
- **Test Case ID**: TC014
- **Description**: Verify behavior when the session expires during the password change process.
- **Steps**: Simulate a session timeout and attempt to submit the form.
- **Expected Result**: The user should be redirected to the login page with a message like "Session expired. Please log in again."

