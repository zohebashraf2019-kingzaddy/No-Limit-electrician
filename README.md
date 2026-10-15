# No Limit Electric LLC Website Demo

A responsive, static website ready for GitHub and Vercel. Includes 14 optimized project images, two converted MP4 walkthroughs, company logo, responsive project gallery with filters, next/previous lightbox navigation, looping video playback in the viewer, services, About placeholder and estimate form.

## Deploy to Vercel
1. Extract ZIP, then upload the contents of `no-limit-electric-site` to a new GitHub repository.
2. In Vercel select **Add New → Project**, import the repository.
3. Select **Other** as framework preset. No build command needed. Set output directory to `.` if requested.
4. Click **Deploy**.

For a local test, open `index.html` in a browser. A local server such as `python3 -m http.server 8000` is recommended for reliable video loading.

## Before going live
- **Estimate form:** The form currently opens a draft email using `mailto:` with the visitor's details. It does **not** send a message to the business because the owner's email address has not been provided. When available, add the email to the mailto link in `script.js`, or connect a server-side form service such as Formspree, Resend, or a Vercel serverless function. Never expose private API keys in client-side JS.
- Add the owner-approved biography, verified license number, business email, business hours and exact service area.
- Confirm rights to publish all supplied images and videos.
- Review the automatically generated project captions and classifications with the owner before launch.
- Add further photos as optimized WebP assets and edit the `items` array in `script.js`.
- Videos are user-click-to-play and loop inside the gallery viewer; no sound autoplay is forced.
