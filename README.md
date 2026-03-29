# 🎬 MovieTime - Cinematic Experience Platform

**MovieTime** is a modern movie management and ticket booking application. It provides users with a seamless interface to browse a cinematic catalog, view detailed movie information, and book specific seats in an interactive theater map. The project is specifically engineered to be a **QA Automation Playground**, featuring synchronized validation logic between the frontend and backend.

<img width="908" height="827" alt="image" src="https://github.com/user-attachments/assets/79b97596-a38d-4990-bd7d-9bc4b32a0cc3" />

## 🚀 Key Features
- **Dynamic Catalog:** Sort and filter movies by genre, rating, and status (Now Showing, Coming Soon, Top Rated).
- **Interactive Booking:** A seat selection system with custom pricing logic based on rows (Premium, Standard, Back).
- **User Authentication:** Complete Register/Login flow with strict validation rules.
- **Admin Dashboard:** Full CRUD capabilities for movie inventory, order tracking, and user status management.
- **Modern UI/UX:** Responsive design with support for Dark and Light modes.

## 🧪 Built for Automation (QA Focus)
This project is designed to be easily testable. It follows industry best practices for automation by including unique **`data-testid`** attributes for all critical elements.

### Automation Examples:
- **Search:** Use `data-testid="search-input"` to test filtering logic.
- **Auth Flow:** Target `data-testid="register-form"` for DDT (Data-Driven Testing).
- **Error Handling:** Capture specific validation errors via `data-testid="error-name"` or `data-testid="error-password"`.
- **Seat Selection:** Interact with the grid using IDs like `data-testid="seat-A1"`.

## 📋 Business Rules & Validations
The application implements synchronized validation logic between the React frontend and Node.js (Joi) backend:

| Field | Validation Rule |
| :--- | :--- |
| **Username** | 2-40 characters, English letters and spaces only. |
| **Password** | 6-50 characters. |
| **Email** | Standard RFC email format (Synced with Joi validation). |
| **Booking** | Max 8 tickets per transaction. |

## 🛠 Tech Stack
- **Frontend:** React 18 (via CDN), CSS3 Variables.
- **State Management:** React Context API & LocalStorage.
- **Backend:** Node.js, Express, Joi (for schema validation).
- **Security:** API Key protection for administrative routes.

## 🏃‍♂️ How to Run
1. Clone the repository.
2. **Backend:** Navigate to the server folder, run `npm install` and then `node server.js`.
3. **Frontend:** Open `index.html` in any modern browser.
4. Ensure the server is running on `http://localhost:3001` for API synchronization.
