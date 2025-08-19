**Patient User stories**  
_As a patient, I want to view a list of doctors without logging in, so that I can explore options before registering._

**Acceptance Criteria:**  
1. Patient can access doctor list without authentication  
2. Doctors are displayed with name, specialty, and availability  
3. The system should not allow booking unless registered  

**Priority:** High  
**Story Points:** 3  

**Notes:**  
- Consider showing limited doctor details to non-logged-in users


# Admin User Stories

## User Story 1
**Title:**  
_As an admin, I want to log into the portal with my username and password, so that I can manage the platform securely._

**Acceptance Criteria:**  
1. Admin can log in using valid credentials  
2. Invalid login attempts show error messages  
3. Successful login redirects to the admin dashboard  

**Priority:** High  
**Story Points:** 3  

---

## User Story 2
**Title:**  
_As an admin, I want to log out of the portal, so that I can protect system access._

**Acceptance Criteria:**  
1. Admin can log out successfully  
2. Session is cleared after logout  
3. Redirects to the login page  

**Priority:** High  
**Story Points:** 2  

---

## User Story 3
**Title:**  
_As an admin, I want to add doctors to the portal, so that they can be available for patients._

**Acceptance Criteria:**  
1. Admin can add doctor details (name, specialty, availability)  
2. Data is stored in the database  
3. Confirmation message is shown after adding  

**Priority:** High  
**Story Points:** 5  

---

## User Story 4
**Title:**  
_As an admin, I want to delete a doctor’s profile, so that I can remove inactive or invalid accounts._

**Acceptance Criteria:**  
1. Admin can select a doctor and delete their profile  
2. System asks for confirmation before deleting  
3. Deleted doctors are no longer visible in the portal  

**Priority:** Medium  
**Story Points:** 4  

---

## User Story 5
**Title:**  
_As an admin, I want to run a stored procedure in MySQL CLI, so that I can get the number of appointments per month and track usage statistics._

**Acceptance Criteria:**  
1. Admin can access the MySQL CLI  
2. Stored procedure returns total appointments per month  
3. Data is accurate and reflects real usage statistics  

**Priority:** Medium  
**Story Points:** 5  

# Doctor User Stories

As a doctor, you can:

- Log into the portal to manage your appointments  
- Log out of the portal to protect your data  
- View your appointment calendar to stay organized  
- Mark your unavailability to inform patients of only the available slots  
- Update your profile with specialization and contact information so patients have up-to-date information  
- View the patient details for upcoming appointments so that you can be prepared  

