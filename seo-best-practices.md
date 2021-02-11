# SEO Best Practices

## [Google beginner SEO docs][seo-beginner]

- robots.txt
  - block crawling of 404 page
- sitemap.xml
  - creation
  - submission to index
    - submit `www` and `non-www` and `http` versions
- `<title>` and `<meta name="description" content="..."` in `<head>`
  - unique title and description for every page
- use heading tags to emphasize important text
- don't use too many headings
- add structured data to your site
  - [JSON-LD format (recommended)](https://json-ld.org/)
  - <schema.org>
  - [Rich results test][rich-results-test]
  - [Structured data gallery][structured-data-gallery]
- Usefule custom 404 page
- know what your readers want (and give it to them!)
- **Be careful who you link to!**
  - use `nofollow` or `ugc` to keep from endorsing a link
  - to nofollow all links on the page: `<meta name="robots" content="nofollow">`
- Optimize images
  - provide `alt` text
  - use `loading="lazy"` for faster page loads
  - use `img` or `picture` tag
- Make your site mobile-friendly
  - Responsive web design
  - `<meta name="viewport" />` to tell browser how to adjust content
- Promote your website

## [Google advanced SEO docs][seo-advanced]

- understand what [canonical pages][canonical-pages] are

<!-- Links -->

[seo-beginner]: https://developers.google.com/search/docs/beginner/seo-starter-guide "SEO starter guide"
[advanced-beginner]: https://developers.google.com/search/docs/advanced/guidelines/get-started "Advanced SEO"
[canonical-pages]: https://developers.google.com/search/docs/advanced/crawling/consolidate-duplicate-urls#definition "Canonocal pages"
[structured-data-gallery]: https://developers.google.com/search/docs/guides/search-gallery "Structured data gallery"
[rich-results-test]: https://search.google.com/test/rich-results "Test site for rich results"
