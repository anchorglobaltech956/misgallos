# Three Roots Animal Nutrition — GitHub Pages and Custom Subdomain

This package contains the newest bilingual landing page, including the plant map and delivery-route calculator, retailer section, weekly Houston/Dallas/San Antonio deliveries, and the larger English/Español control. Every logo, feed photograph, rooster image, and video is embedded directly inside `index.html`.

## Update the GitHub Pages repository

1. Extract this ZIP file.
2. Open your GitHub repository.
3. Select **Add file → Upload files**.
4. Upload `index.html` and `CNAME` to the top level of the repository. The other files are optional instructions.
5. Select **Commit changes**.
6. Open **Settings → Pages** and confirm the source is the `main` branch and `/(root)` folder.
7. Under **Custom domain**, enter `threeroots.anchorglobaltech.com` and select **Save**.
8. Follow `CLOUDFLARE-SUBDOMAIN-INSTRUCTIONS.md` to add the Cloudflare DNS record.

Only `index.html` is required for the website. There is no separate `assets` folder to lose or place incorrectly.

Do not upload the ZIP itself to the repository. Extract it first and upload the files inside it.
