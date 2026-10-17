# Dal Lake Dry Fruits store: how to put it live (GitHub Pages)

## 1. Upload the site (one time)
1. Make a free account at github.com and click **New repository**. Name it e.g. `dal-lake`, set it **Public**, and create it.
2. Click **Add file → Upload files**, drag in `index.html`, `admin.html` and `data.json`, then **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment" choose **Deploy from a branch**, branch `main`, folder `/ (root)`, and Save.
4. After about a minute your store is live at `https://YOURNAME.github.io/dal-lake/`.

## 2. Set your admin password (one time)
Open `https://YOURNAME.github.io/dal-lake/admin.html` (bookmark this link; customers never see it or link to it).
Create a password of 10+ characters. Keep it safe.

## 3. Create a GitHub token (one time)
1. GitHub → your profile picture → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. **Repository access:** Only select repositories → choose `dal-lake`.
3. **Permissions → Repository permissions → Contents: Read and write.**
4. Generate, copy the token.

## 4. Connect and publish
In the admin page open the **Publish** tab, enter your GitHub username, repository name (`dal-lake`) and branch (`main`), paste the token, press **Save connection**, then **Publish to live site**.
Do your first publish right after creating your password so the password is saved on the live site.

From now on: add products and photos, change prices, mark items sold out, press **Publish**, and customers see the update in about a minute.

## 5. Payments and orders
- In **Store settings** add your UPI ID (e.g. `name@okaxis`) or upload your own UPI QR image.
- Customers place the order and WhatsApp opens with the full order (name, phone, address, items, total) sent to your number. They must tap Send. Then you reply with payment details, or they can pay straight away using the QR/Pay button and add the transaction ID.
- The site cannot confirm money arrived. Check each payment in your bank/UPI app before dispatching.

## 6. Your own domain (optional)
Settings → Pages → **Custom domain**, enter your domain, then add the DNS records GitHub shows at your domain provider. Tick **Enforce HTTPS**.
If you use a custom domain, enter your GitHub username and repository name in the Publish tab manually.

## Security notes
- The password hides the admin page. The real lock is your GitHub token: nobody can change your store without it. Never share the token.
- The token is saved encrypted (with your password) in your browser only.
- Because the site has no server, the password check happens in the browser. Use a long, unique password.
