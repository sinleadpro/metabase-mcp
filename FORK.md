# Fork Maintenance

Forked from [jerichosequitin/metabase-mcp](https://github.com/jerichosequitin/metabase-mcp). Published as `@cyberbiz-corp/metabase-mcp`.

## Setup (one-time)

```bash
git remote add upstream https://github.com/jerichosequitin/metabase-mcp.git
npm login  # needs @cyberbiz-corp publish permission
```

## Sync + Publish

```bash
git fetch upstream
git merge upstream/main
npm run build
npm version patch
npm publish --access public
git push origin main --follow-tags
```
