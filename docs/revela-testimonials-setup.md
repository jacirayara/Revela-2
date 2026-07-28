# Revela Testimonials Setup

This theme includes a `Revela testimonials` section that can display reviews from Shopify metaobjects, so the client can manage approved testimonials in Shopify Admin without a paid reviews app.

## Shopify Metaobject Definition

Create a metaobject definition in Shopify Admin:

- Name: `Revela testimonial`
- Type: `revela_testimonial`

Recommended fields:

- `name` - Single line text
- `review` - Multi-line text
- `rating` - Integer, 0 to 5
- `image` - File reference, image
- `video` - File reference, video
- `video_url` - Single line text, for YouTube or Vimeo links
- `details` - Single line text, for location, product, or customer detail
- `approved` - True or false
- `featured` - True or false
- `consent_text` - Single line text

## Manual Free Workflow

1. Customer submits feedback through the testimonial form.
2. The client receives and reviews the submission.
3. If approved, the client creates a new `Revela testimonial` metaobject.
4. The client sets `approved` to true.
5. The testimonial appears in the section when the section source is set to `Shopify admin metaobjects`.

## Theme Editor Settings

In the `Revela testimonials` section:

- Set `Show testimonials from` to `Shopify admin metaobjects` once the metaobjects exist.
- Keep `Only show approved metaobjects` enabled.
- Use `Reviews shown before load more` to control how many reviews appear first.
- Use `Maximum metaobject reviews` to stop the page from becoming too long.

Until real reviews are uploaded, keep the section source set to `Theme editor blocks` so the existing placeholders still show.

## Reviews Page

The theme includes a `page.reviews` template for the full review list.

To make it visible in Shopify:

1. Go to Shopify Admin > Online Store > Pages.
2. Create a page named `Reviews`.
3. Set the theme template to `reviews`.
4. Save the page.
5. Add it to the menu if needed.

The homepage should stay curated with three image testimonials and one video. The `Reviews` page can hold the full approved review list and the feedback form.
