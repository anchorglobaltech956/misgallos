# Connect threeroots.anchorglobaltech.com to GitHub Pages

These instructions assume the GitHub account is `anchorglobaltech956`.

## Part 1 — Update GitHub Pages first

1. Open the GitHub repository containing the Three Roots website.
2. Select **Settings**.
3. Select **Pages** from the left menu.
4. Confirm the publishing source is **Deploy from a branch**, branch **main**, folder **/(root)**.
5. In **Custom domain**, enter exactly:

   `threeroots.anchorglobaltech.com`

6. Select **Save**.

The included uppercase `CNAME` file contains the same domain and must remain at the repository root.

## Part 2 — Add the record in Cloudflare

1. Sign in to Cloudflare.
2. Select the `anchorglobaltech.com` domain.
3. Select **DNS → Records**.
4. Select **Add record**.
5. Enter these values:

| Field | Value |
| --- | --- |
| Type | `CNAME` |
| Name | `threeroots` |
| Target | `anchorglobaltech956.github.io` |
| Proxy status | `DNS only` — gray cloud |
| TTL | `Auto` |

6. Select **Save**.

Do not put `/3RootsAnimalNutrition/` or any other repository path in the Target field. The target ends at `.github.io`.

If a DNS record named `threeroots` already exists, edit that record instead of creating a duplicate.

## Part 3 — Finish HTTPS

1. Return to **GitHub repository → Settings → Pages**.
2. Wait until GitHub reports that the DNS check is successful.
3. Select **Enforce HTTPS** when the checkbox becomes available.
4. Open `https://threeroots.anchorglobaltech.com` in a new browser tab.

DNS and the GitHub security certificate may take time to finish. GitHub advises that DNS changes can require up to 24 hours.

Official references:

- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
- https://developers.cloudflare.com/dns/manage-dns-records/how-to/create-subdomain/

