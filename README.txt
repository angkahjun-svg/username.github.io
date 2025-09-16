# Zhonghua SIL Portal (Static Demo)

This is a static front-end demonstration of the Zhonghua SIL Portal, originally built as a Google Apps Script web application. This version is suitable for hosting on static site platforms like GitHub Pages.

## Key Differences from Original

*   **No Backend:** All server-side Google Apps Script logic has been removed.
*   **Mock Data:** The application uses hardcoded JavaScript objects to simulate student submissions, user roles, and comments. The data does not persist and resets on page reload (except for the Draft Pad).
*   **Mock Authentication:** The login screen allows you to select a user role (Student, Staff, or Admin) to explore the different UI views and permissions.
*   **Browser Storage:** The "Draft Pad" feature now uses the browser's `localStorage` to save and load notes, so drafts are saved on your specific device and browser.

## How to Deploy to GitHub Pages

1.  **Create a New Repository:** Create a new public repository on GitHub (e.g., `sil-portal-demo`).
2.  **Upload the File:** Upload the `index.html` file from this project into your new repository.
3.  **Enable GitHub Pages:**
    *   In your repository, go to **Settings > Pages**.
    *   Under "Branch", select `main` (or `master`) and the `/root` folder.
    *   Click **Save**.
4.  **Access Your Site:** GitHub will provide you with a URL (e.g., `https://<your-username>.github.io/sil-portal-demo/`). It may take a few minutes for the site to become live.

## How to Use the Demo

1.  Open the deployed site URL.
2.  On the login screen, click one of the buttons to sign in as a **Student**, **Staff**, or **Admin**.
3.  Explore the portal's features from the perspective of the chosen role.
4.  To switch roles, click the "Logout" button, which will refresh the page and return you to the mock login screen.