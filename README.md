# Brittney Hughes

A small, responsive personal website for https://brittneyhughes.com. Plain HTML and CSS, with no build step, JavaScript, or external dependencies.

## Preview

From this directory:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000.

## Deploy to GitHub Pages

1. Create a GitHub repository (for example, `brittneyhughes.com`) and push these files to its `main` branch.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then **main** and **/ (root)**. Save.
4. Under **Custom domain**, enter `brittneyhughes.com` and save. The included `CNAME` file also preserves this setting for branch publishing.
5. After setting the custom domain in GitHub, configure the domain’s DNS provider:

   | Type | Name | Value |
   | --- | --- | --- |
   | A | @ | 185.199.108.153 |
   | A | @ | 185.199.109.153 |
   | A | @ | 185.199.110.153 |
   | A | @ | 185.199.111.153 |
   | CNAME | www | brittneyhughes.github.io |

   Replace conflicting web-hosting records for these same names; keep unrelated records such as email MX and TXT records. Configure the `www` record if you want that hostname to work too.
6. Once GitHub’s DNS check and certificate provisioning finish, enable **Enforce HTTPS**. DNS changes can take up to 24 hours.

GitHub recommends verifying domain ownership in account settings before configuring a custom domain. See the [official custom-domain guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) and [domain verification guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/verifying-your-custom-domain-for-github-pages).

## Edit content

- `index.html`: biography, projects, experience, certifications, and contact links.
- `styles.css`: colors, typography, layout, responsive and print styling.
- `assets/favicon.svg`: browser icon.
- `CNAME`: custom domain.

Career details are condensed from the supplied LinkedIn profile export. The projects section features the Bro Code Java learning repository, credits the course, and links to the Mad Libs and Shopping Cart mini projects. The original profile PDF and mobile number are not published. Review details before deployment and update the expected graduation date and footer year as needed.
