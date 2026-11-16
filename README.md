# Rony Smith | Portfolio

A responsive, single-page portfolio for Rony Smith, a web and AI developer. It introduces his work, highlights selected client projects, and gives visitors a way to get in touch.

## What's on the page

- **Home:** introduction, availability, and featured project.
- **About:** a short profile and photo.
- **Capabilities:** technologies and tools.
- **Selected work:** a keyboard-accessible project carousel with links to live sites.
- **Contact:** a message form and direct email link.

The layout adapts to mobile screens and includes a mobile navigation menu, scroll animations, and a back-to-top button.

## Preview locally

This is a static website: there is no package installation, build step, or framework. You can open `index.html` in a browser, or serve the project root locally:

```bash
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). The page loads fonts, AOS, and Swiper from external CDNs, so an internet connection is needed for those features.

## Project files

| File or folder | Purpose |
| --- | --- |
| `index.html` | Page content, metadata, project cards, contact form, and library setup. |
| `style.css` | Layout, responsive rules, colors, and component styles. |
| `main.js` | Mobile menu, active navigation state, and back-to-top behavior. |
| `src/png/` | Logo and About photos, technology icons, and other PNG assets. |
| `src/webp/` | Featured-project and project-card images. |
| `src/svg/`, `src/ico/`, `src/mp3/` | Supporting icons and media. |

## Updating the portfolio

- Edit the text and links in `index.html`.
- Project cards are inside `#projects`. Keep the Swiper classes (`swiper`, `swiper-wrapper`, and `swiper-slide`) when adding or removing slides.
- Replace the images in `src/webp/` or `src/png/` as needed, and update each image's `src` and descriptive `alt` text in `index.html`.
- The site's colors and visual styles are defined in `style.css`.
- Update the page title, description, social metadata, and favicon in the `<head>` of `index.html` before publishing.
- The contact form currently submits to FormSubmit at `ronysmith@gmail.com`. Change its `action` URL to use a different inbox, and test the form after deployment.

## Libraries and services

- [AOS](https://michalsnik.github.io/aos/) for scroll-triggered animations.
- [Swiper](https://swiperjs.com/) for the selected-work carousel.
- [Google Fonts](https://fonts.google.com/) for DM Sans and Space Grotesk.
- [FormSubmit](https://formsubmit.co/) for contact-form delivery.

These are loaded from their hosted services; the project does not bundle them locally.

## Deployment

Deploy the repository root to any static web host, such as GitHub Pages. No build command is required. Ensure the host serves `index.html` from the root and preserves the `src/` asset paths. If using a custom domain, update `CNAME` to the domain you control or remove it when it is not needed.

## License

This project is released under the MIT License. See [LICENSE](./LICENSE).
