# Video SEO Lab — Cloudflare

## Public video page
https://video.top5reviews.online/videos/horse-gelatin-trick/

## Video Sitemap
https://video.top5reviews.online/video-sitemap.xml

## Robots
https://video.top5reviews.online/robots.txt

## Architecture
GitHub main branch -> Cloudflare static hosting -> custom subdomain.
The root test homepage remains `noindex`. The Horse Gelatin video page is `index, follow` with a self-canonical and one VideoObject. `_headers` does not apply a global noindex. The `video-sitemap.xml` contains the matching single watch-page record.

## Next step
In Google Search Console, verify the property for `https://video.top5reviews.online/`, use URL inspection (Test Live URL) on the video page, check that the live page is indexable, and submit `video-sitemap.xml`. Monitor the Video Indexing report.

## Important duplicate-content warning
The exact same VTurb video also appears on the existing Atomicat page: https://www.top5reviews.online/horse-gelatin-recipe-video-1. Its page and SEO were not changed. Google may treat these as duplicate video pages and select only one URL as canonical. Do not assume both will be indexed.

## Future updates
When adding a new video, publish a dedicated watch page, then add one `<url>` entry to the same `video-sitemap.xml` with true values: watch page, thumbnail, title, description, VTurb embed player, duration, and initial publication date.
