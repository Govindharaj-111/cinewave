# CineWave — Movie Ticket Booking Demo

CineWave is a responsive React + Vite college mini-project demonstration. It includes a movie catalogue, search and genre filters, movie detail dialogs, interactive seat selection, demo checkout, locally saved bookings, booking cancellation, and a demo admin dashboard with CSV export.

## Requirements
- Node.js 20.19+ or 22.12+ recommended
- npm (included with Node.js)
- A modern browser

## Run on Windows
1. Install Node.js LTS from https://nodejs.org/ and restart your terminal.
2. Extract the `cinewave.zip` folder.
3. Open the extracted `cinewave` folder in VS Code, or open Command Prompt in that folder.
4. Run:

   ```bash
   npm install
   npm run dev
   ```
5. Open the local URL shown by Vite, usually http://localhost:5173.
6. To check the production build, run `npm run build`. The output is created in `dist/`.

## Deploy to Vercel
1. Create a GitHub repository named `cinewave` (or use a different available name).
2. Upload/push all files from this folder, including `package.json`, `index.html`, and `src/`.
3. Sign in at https://vercel.com/ with GitHub and choose **Add New → Project**.
4. Import the repository. Vercel should detect Vite automatically. Use build command `npm run build` and output directory `dist`.
5. Click **Deploy**. Vercel provides a public URL such as `your-project.vercel.app`.

Alternative: deploy to https://netlify.com by importing the GitHub repository; use build command `npm run build` and publish directory `dist`.

## Demo walkthrough
1. Browse Home or Movies; search titles and filter by genre.
2. Click a movie poster/title for details or click Book.
3. Pick a date, showtime, seats, and enter a name and valid email.
4. Confirm the booking and note the booking ID.
5. Open My Bookings to see or cancel bookings.
6. Open the CW profile menu → Admin dashboard to view counts and export a CSV.

## Important demo limitations
- This is a front-end demonstration. Bookings are stored in the current browser's localStorage; they are not shared across browsers/devices and can be cleared by the user.
- No real payment is collected. The confirmation screen is a simulated checkout.
- The admin page is not protected by real authentication. Do not use it for real customer data.
- Movie poster and hero images load from TMDB image URLs and need an internet connection. Fallback gradients and titles appear if an image is unavailable.
- Movie data and showtimes are sample data for a college demonstration, not live cinema listings.
