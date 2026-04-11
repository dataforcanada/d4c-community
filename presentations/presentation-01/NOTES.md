pnpm build

rclone copy --progress --transfers 16 --checkers 16 dist/ cloudflare:dataforcanada-static-prod-enam/d4c-community/presentations/2026-04-10-canadian-open-data-society/