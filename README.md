# QuickTask Frontend

QuickTask is a web and mobile-friendly platform that connects university students with short-term side gigs from approved companies and individuals, with the support of their institutions.

This README covers the **frontend** structure, pages, components, and their core functionalities.

---

## 📄 Pages & Functionalities

### 1. **Home / Dashboard**

**Path:** `/dashboard`  
**Purpose:** Central hub for the user, showing key actions and summaries at a glance.  
**Main Components:**

- **Navbar** (static)
    
- **Job Summary Cards** – total available jobs, applied jobs, posted jobs
    
- **Quick Links** – shortcuts to job posting and applications
    
- **Recent Jobs Feed** – latest gigs from the database
    
- **Notifications Panel** – important updates (optional)
    

**Functionality:**

- Fetches and displays recent job listings.
    
- Shows user-specific statistics.
    
- Responsive layout for mobile and desktop.
    

---

### 2. **Jobs**

**Path:** `/jobs`  
**Purpose:** Displays a list of available jobs for browsing and applying.  
**Main Components:**

- **Search & Filter Bar** – keyword, category, location
    
- **Job Cards** – title, pay rate, company, deadline
    
- **Pagination / Infinite Scroll**
    

**Functionality:**

- Fetch jobs from backend API.
    
- Filter and search dynamically.
    
- Navigate to a job’s **Details Page** for application.
    

---

### 3. **My Applications**

**Path:** `/applications`  
**Purpose:** Lets users track jobs they have applied to.  
**Main Components:**

- **Application List** – job title, company, date applied, status
    
- **Status Badges** – pending, accepted, rejected
    

**Functionality:**

- Pulls application history from backend.
    
- Displays live status updates.
    
- Click on a job to view application details.
    

---

### 4. **My Postings**

**Path:** `/my-postings`  
**Purpose:** For job posters to see and manage gigs they’ve created.  
**Main Components:**

- **Post List** – job title, applicants count, status
    
- **Action Buttons** – edit, close, delete post
    

**Functionality:**

- Fetch posted jobs from backend.
    
- Manage job lifecycle (open/close applications).
    
- View applicant list.
    

---

### 5. **Post a Job**

**Path:** `/post-job`  
**Purpose:** Allows approved users to create a new job listing.  
**Main Components:**

- **Job Form** – title, description, category, pay rate, deadline
    
- **Image/File Upload** (optional)
    
- **Submit Button**
    

**Functionality:**

- Validates input fields.
    
- Sends job data to backend API.
    
- Redirects to **My Postings** after success.
    

---

### 6. **Settings**

**Path:** `/settings`  
**Purpose:** Personalize and control account preferences.  
**Main Components:**

- **Profile Settings** – name, contact info, bio
    
- **Notification Preferences**
    
- **Password Change Form**
    

**Functionality:**

- Update profile details.
    
- Change password securely.
    
- Toggle email/notification preferences.
    

---

### 7. **Profile**

**Path:** `/profile`  
**Purpose:** Displays public or personal profile of a user.  
**Main Components:**

- **Profile Card** – photo, name, bio
    
- **Job History** – jobs applied/posted
    
- **Ratings/Reviews** (optional)
    

**Functionality:**

- Fetch and display user details.
    
- Show activity history.
    
- Option to edit profile (if own account).
    

---

## 📌 Static Navbar

- Appears on all pages.
    
- Contains links to all main sections: Dashboard, Jobs, My Applications, My Postings, Post Job, Settings, Profile.
    
- Responsive: collapses into hamburger menu on mobile.
    
- Displays profile picture and notification icon.
