# 2026-06-15 Homepage status update

## Facts

- Updated `_pages/about.md` to present Yuqi Peng as a Ph.D. student at the University of Arizona, advised by Prof. Huanrui Yang.
- Removed the old PhD application sentence from the homepage.
- Updated `_config.yml` sidebar metadata from Northeastern/Boston to University of Arizona/Tucson.
- Updated `_pages/cv.md` web CV education section with a University of Arizona Ph.D. entry starting Fall 2026, advisor Prof. Huanrui Yang, and changed the Northeastern M.S. entry from expected to completed.
- Removed the Blogs navigation item from `_data/navigation.yml`.
- Deleted `_pages/blog.html` so the `/blog/` index page is no longer generated from that page.
- Did not modify `files/Yuqi_Peng_CV.pdf`.
- Updated the site contact email in `_config.yml` from `peng.yuq@northeastern.edu` to `yuqipeng@arizona.edu`.

## Verification

- Ran `rg -n "plan to apply|I plan to apply|M\\.S\\. student|CS Master student|Boston, MA|Fall 2026|Northeastern University|Blogs|/blog/" _pages _config.yml _data _includes _layouts _blog`.
- The stale application and current M.S. student phrases no longer appear.
- Remaining `Northeastern University` matches are historical references in the homepage and CV.
- Ran `find . -maxdepth 3 -path './.git' -prune -o -name 'blog.html' -print`; no `blog.html` page remains outside `.git`.
- Attempted `bundle exec jekyll build`, but the environment does not have the required Jekyll executable installed.
- Ran `bundle check`; Bundler reported missing Gemfile dependencies and suggested `bundle install`.

## Next Action

- If a full local render check is required, install the Ruby gems with `bundle install` and rerun `bundle exec jekyll build`.
