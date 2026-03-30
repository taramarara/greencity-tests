# Test Cases for Registration Page

---

## Test Case 1: Successful registration with valid data

**ID:** TC-REG-001  
**Title:** User can register with valid data  

**Preconditions:**
- Registration form is open

| Step | Action | Data | Expected Result |
|------|--------|------|----------------|
| 1 | Enter valid email | testuser123@gmail.com | Email accepted |
| 2 | Enter valid username | Taras123 | Username accepted |
| 3 | Enter valid password | Qwerty123! | Password meets requirements |
| 4 | Confirm password | Qwerty123! | Passwords match |
| 5 | Click "Register" | - | Registration successful / user logged in or redirected |

**Priority:** High  
**Type:** Positive  

---

## Test Case 2: Validation of empty fields (Negative)

**ID:** TC-REG-002  
**Title:** Form validation for empty required fields  

**Preconditions:**
- Registration form is open

| Step | Action | Data | Expected Result |
|------|--------|------|----------------|
| 1 | Leave all fields empty | - | Fields highlighted in red |
| 2 | Click "Register" | - | Error messages appear (e.g. "Введіть пошту") |

**Priority:** High  
**Type:** Negative  

---

## Test Case 3: Invalid email format

**ID:** TC-REG-003  
**Title:** Email validation rejects invalid format  

**Preconditions:**
- Registration form is open

| Step | Action | Data | Expected Result |
|------|--------|------|----------------|
| 1 | Enter invalid email | testemail.com | Error message shown |
| 2 | Click "Register" | - | Registration blocked |

**Priority:** High  
**Type:** Negative  

---

## Test Case 4: Toggle password visibility

**ID:** TC-REG-004  
**Title:** User can show/hide password  

**Preconditions:**
- Password field contains data

| Step | Action | Data | Expected Result |
|------|--------|------|----------------|
| 1 | Enter password | Qwerty123! | Password hidden |
| 2 | Click "eye" icon | - | Password becomes visible |
| 3 | Click again | - | Password hidden again |

**Priority:** Medium  
**Type:** UI   

---

## Test Case 5: Password mismatch

**ID:** TC-REG-005  
**Title:** System detects password mismatch  

**Preconditions:**
- Registration form is open

| Step | Action | Data | Expected Result |
|------|--------|------|----------------|
| 1 | Enter password | Qwerty123! | Accepted |
| 2 | Enter different confirm password | Qwerty1234! | Error shown |
| 3 | Click "Register" | - | Registration blocked |

**Priority:** High  
**Type:** Negative  

---
