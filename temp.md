# User Story Flashcards

---

## User Story 1

**Front of the Card**  
    As a visitor, I want to browse property listings so that I can explore available properties without an account.  

**Back of the Card**  

✅ **Success Scenarios**  
- Homepage loads with a grid of featured properties (thumbnail, price, location).  
- Users can click on a property to view details.  

❌ **Failure Scenarios**  
- **Backend database unavailable**  
  *Message:* `We’re experiencing technical difficulties. Please try again later.`  
- **User Browser crashes**  
  *Message:* `Your browser has crashed. Relaunch and try again.`  

---

## User Story 2

**Front of the Card**  
As a registered user, I want to save a property listing so that I can revisit it later.  

**Back of the Card**  
✅ **Success Scenarios**  
- Click “Save” on a property → Saved to user account under **Saved Listings**.  
- Saved listings persist across sessions.  

❌ **Failure Scenarios**  
- **Database error saving data**  
  *Message:* `Failed to save listing. Please try again.`  
- **User not logged in**  
  *Message:* `You must be logged in to save listings. Please log in or register.`  

---

## User Story 3

**Front of the Card**  
As a verified lister, I want to post a new property listing so that buyers/renters can view it.  

**Back of the Card**  
✅ **Success Scenarios**  
- Fill out form (title, description, photos, price) → Listing is submitted for **admin review**.  

❌ **Failure Scenarios**  
- **Missing required fields (e.g., price)**  
  *Message:* `Price is required. Please enter a valid amount.`  
- **Server error during submission**  
  *Message:* `Failed to submit listing. Please try again later.`  
- **Photo upload fails due to corrupt file**  
  *Message:* `Invalid file format. Supported formats: JPG, PNG.`  

---

## User Story 4

**Front of the Card**  
As an administrator, I want to moderate listings so that only verified and compliant listings are published.  

**Back of the Card**  
✅ **Success Scenarios**  
- Approve/reject listings via dashboard → Status updates instantly.  
- Rejected listings notify listers:  
  *Message:* `Your listing was rejected due to [reason].`  

❌ **Failure Scenarios**  
- **Dashboard not loading**  
  *Message:* `Moderation tools are unavailable. Try refreshing the page.`  
- **Unauthorized admin access attempt**  
  *Message:* `Access denied. Your credentials are invalid or expired.`  
