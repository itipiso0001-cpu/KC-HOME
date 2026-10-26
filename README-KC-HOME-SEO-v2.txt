KC HOME — SEO + crawlable photos + favicon (v2)

IMPORTANT: Extract this ZIP before uploading. The ZIP itself should NOT be uploaded into the repository.

Upload/replace these items in the ROOT of the GitHub repository:
  index.html
  favicon.ico
  favicon.svg
  favicon-48.png
  favicon-128.png
  apple-touch-icon.png
  logo.png
  robots.txt
  sitemap.xml
  assets/images/   (upload every image inside, preserving the folder path)

The assets/images folder contains the project's own images extracted from the existing HTML, optimized as JPEG files, plus kc-home-social.jpg as the social/share preview image. All image references in index.html now use public image URLs rather than embedded Base64, allowing crawlers and preview systems to request the images directly.

GitHub web upload:
1. Open https://github.com/itipiso0001-cpu/KC-HOME
2. Add file > Upload files, then upload the files above while keeping the assets/images path.
3. If GitHub does not preserve folder paths when uploading from your browser, create/open assets/images in the repository and upload the image files into that folder separately.
4. Commit to branch main. Netlify should publish automatically if its main branch publishing is enabled.
5. Check Netlify Deploys and confirm Production is Published.

Canonical host note:
Google currently shows https://kchome.online/ in its search result. This version aligns canonical, Open Graph URL, structured data, robots.txt and sitemap.xml to https://kchome.online/. In Netlify Domain management, keep kchome.online as the Primary domain so www.kchome.online redirects to it. If you prefer www as primary, all canonical URLs and sitemap URLs should instead be changed consistently to https://www.kchome.online/.

After deployment:
- Check https://kchome.online/favicon.ico and https://kchome.online/assets/images/kc-home-social.jpg open directly.
- In Google Search Console, verify both domain/host variants if applicable, use URL Inspection for https://kchome.online/ and Request indexing, then submit https://kchome.online/sitemap.xml.
- Google favicon and search/AI overview image selections are controlled by Google and are not guaranteed. Recrawling can take days to weeks.
