# StarLookup

StarMaker SID-only profile lookup website.

## Live website and API

The public website is served by the Supabase Edge Function:

https://vkpvkobuebfqhzklduvr.supabase.co/functions/v1/swift-processor

Enter a SID in the page. The same function returns JSON when called with `?sid=STARMAKER_SID`.

## Lookup provider

The function proxies:

https://starmaker.id.vn/wp-json/sm-user/v1/lookup

Only fields returned by the provider are displayed. Provider availability, rate limits, and returned profile fields determine what can be shown.

## Source

The frontend is in `index.html`. The Supabase Edge Function serves this page and handles SID lookup requests.
