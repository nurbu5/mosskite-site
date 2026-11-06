# Mosskite Games website

Static website for Mosskite Games, operated by Mosskite LLC. The site is published by GitHub Pages at `https://nurbu5.github.io/mosskite-site/`; `mosskite.net` is the intended custom domain. There are no build dependencies.

## Before app review

- Confirm **support@mosskite.net** is monitored. Test sending a message and receiving a reply, including score removal requests. The domain currently has Cloudflare email routing MX records; those alone do not confirm the mailbox works.
- Point **mosskite.net** to GitHub Pages in Cloudflare DNS. For the apex, use GitHub's four A records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, and `185.199.111.153`. Use DNS-only records while GitHub provisions HTTPS. Remove conflicting apex A/AAAA records, but preserve the MX and email TXT records. The Pages publishing source is a GitHub Actions workflow, so a repository `CNAME` file is not needed.
- After DNS resolves to GitHub, confirm the custom domain and HTTPS certificate in repository Pages settings, then enable **Enforce HTTPS**. Verify domain ownership under the GitHub Pages repository owner (currently the personal `nurbu5` account) and in the organization's Google Search Console account. If the repository moves to a GitHub organization, verify under that organization after the move.
- Update `privacy.html` against each released game's actual behavior. Name the ad and analytics SDKs, purchase provider, leaderboard provider, other third parties, data collected, purposes, retention, security, and deletion process. Match the app and store disclosures.
- If a game adds accounts, provide external and in-app account deletion before submission. For a nickname-only leaderboard, offer score removal through support.
- After deployment, test home, support, and privacy over HTTPS without signing in, on mobile and desktop. Test keyboard navigation and public links.
- Enter the live URLs in App Store Connect and Play Console only after these steps are complete.

Website publication alone does not guarantee app approval. See the [Apple App Review Guidelines](https://developer.apple.com/app-store/review/guidelines/), [Google Play User Data policy](https://support.google.com/googleplay/android-developer/answer/10144311), and [GitHub Pages custom domain guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages).
