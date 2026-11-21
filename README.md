# StarLookup

StarMaker SID-only profile lookup website.

## Backend
The frontend calls the Supabase Edge Function:
`https://vkpvkobuebfqhzklduvr.supabase.co/functions/v1/swift-processor`

The function proxies the profile lookup provider:
`https://starmaker.id.vn/wp-json/sm-user/v1/lookup`

## Run
Open `index.html` in a browser or publish the repository with GitHub Pages.

Only fields returned by the provider are displayed. Provider availability, rate limits, and its own response fields determine what can be shown.
