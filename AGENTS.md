# Forestry Demo Instructions

This is a Jekyll 3.6 demo site, not a Rails application. `_config.yml` defines the `people`, `posts`, and `projects` collections, while `.forestry/settings.yml` maps Forestry editor configuration to `_people`, `_posts`, and `_projects`. Keep those paths, front matter, layouts, and includes consistent when changing a collection or editor field.

Use Bundler with the committed `Gemfile.lock`; `bundle exec jekyll build` is the local static-site check when the legacy Jekyll toolchain is available. There is no checked-in application test suite. `auto_deploy` is false in Forestry configuration, so a local build does not establish CMS publication or a hosted-site update.

Keep hosted CMS tokens and editor credentials out of source control. Treat a configured Forestry webhook or CMS write as a separate external action and report remote publication evidence separately from the local Jekyll build.
