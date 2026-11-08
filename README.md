# AI Longevity & International Law Wiki

A curated wiki distilling:

> Truby J, Kantiana ID (2026). "AI's Promise of Healthy Longevity: Exploring the Implications of Extended Lifespans Under International Law." *Journal of Law, Medicine & Ethics* 54(3): 377–383. doi: [10.1017/jme.2026.10262](https://doi.org/10.1017/jme.2026.10262) (Open Access, CC-BY 4.0)

**Public copy:** https://iamflipse.github.io/ai-longevity-law-wiki/ (read-only; static build served from the `gh-pages` branch)

## Layout

- `src/` — wiki pages as markdown (`index.md`, `about.md`, `concepts/`, `sources/`)
- `book/` — mdbook-generated static site (committed for GitHub Pages)
- `tools/mdbook` — mdbook v0.4.21 binary (aarch64 Linux, built from source)

## Rebuild + republish

```sh
./tools/mdbook build -d book
git add -A && git commit -m "update" && git push origin main
# republish gh-pages: check out orphan branch, copy book/* to root, add .nojekyll, force push
```
