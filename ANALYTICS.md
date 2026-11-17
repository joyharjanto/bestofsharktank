# Website analytics

PostHog tracks the production domains thebestofsharktank.com and www.thebestofsharktank.com. Local previews do not send events.

| Event | Meaning | Useful properties |
| --- | --- | --- |
| `$pageview` | A page opened | PostHog page URL and referrer |
| `$pageleave` | A visitor left | PostHog page/session information |
| `$autocapture` | A standard click or interaction | PostHog element information |
| `amazon_click` | A product, Shark section, or Amazon button was clicked | `product_id`, `product_name`, `category`, `shark`, `deal_status`, `click_location`, `destination` |
| `product_viewed` | At least half a product card entered the viewport, once per page load | `product_id`, `product_name`, `category`, `shark`, `deal_status` |
| `filter_changed` | A category or Shark filter was chosen | `filter_type`, `filter_value` |

In PostHog Product analytics, count `$pageview` for traffic and `amazon_click` for outbound affiliate clicks. Break down `amazon_click` by `product_name` to compare products or `click_location` to compare the three clickable sections. A funnel from `product_viewed` to `amazon_click`, grouped by product, can help compare engagement.

Outbound clicks are not purchases. Amazon does not send order or commission data to this integration.

Session recording is disabled. No identify calls are made. Do Not Track is respected. Standard browser/ad-blocker restrictions can prevent analytics events from being sent.

The public project token is intentionally part of the website. A personal API key must never be included in client-side code.
