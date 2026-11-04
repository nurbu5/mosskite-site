# Mosskite Games website

Static website for Mosskite Games, operated by Mosskite LLC. Publish the repository root with GitHub Pages. There are no build dependencies.

## Before app review

- Replace the **support email placeholder** on `support.html` and `privacy.html` with a working, monitored mailbox. Test game questions and score removal requests.
- Choose and purchase the **custom domain**. Add it in GitHub Pages, create its DNS records, add a matching `CNAME` file here, and enforce HTTPS after the certificate is ready. Verify ownership in the organization's GitHub Pages settings and Google Search Console account. No domain is configured yet.
- Update `privacy.html` against each released game's actual behavior. Name the ad and analytics SDKs, purchase provider, leaderboard provider, other third parties, data collected, purposes, retention, security, and deletion process. Match the app and store disclosures.
- If a game adds accounts, provide external and in-app account deletion before submission. For a nickname-only leaderboard, offer score removal through support.
- After deployment, test home, support, and privacy over HTTPS without signing in, on mobile and desktop. Test keyboard navigation and public links.
- Enter the live URLs in App Store Connect and Play Console only after these steps are complete.

Website publication alone does not guarantee app approval. See the [Apple App Review Guidelines](https://developer.apple.com/app-store/review/guidelines/), [Google Play User Data policy](https://support.google.com/googleplay/android-developer/answer/10144311), and [GitHub Pages custom domain guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages).
