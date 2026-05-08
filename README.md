# liaoliaojun.com

Static personal landing page for `liaoliaojun.com`, designed for GitHub Pages.

## Files

- `index.html` - single-page profile site
- `style.css` - page styling
- `CNAME` - GitHub Pages custom domain, currently `liaoliaojun.com`
- `.nojekyll` - disables Jekyll processing

## GitHub Pages Setup

1. Create a GitHub repository named `liaoliaojun.github.io`.
2. Push this folder to the repository default branch.
3. Go to `Settings -> Pages`.
4. Set the custom domain to `liaoliaojun.com`.
5. After DNS is ready, enable `Enforce HTTPS`.

## Cloudflare DNS

For apex domain:

```text
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
```

For `www`:

```text
CNAME www   liaoliaojun.github.io
```

Set these records to `DNS only` first. After GitHub Pages HTTPS is issued and stable, Cloudflare proxy can be reconsidered.
