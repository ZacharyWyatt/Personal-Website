# Personal-Website
My template for a personal website, tailored towards showcasing a short bio, one's projects, and one's resume.
View it live at https://zacharymwyatt.com

Please feel free to use this template for your own personal website! I only ask that you retain the link to this GitHub repo in the site's footer.

If you do choose to use this template, you'll almost certainly want to:
- Replace instances of `https://example.com` throughout the project with your own URL
- Insert your own name, title, bio, project descriptions, etc.
- Replace `resume.pdf` with your own resume.

You'll also likely want to:
- Supply your own favicon and header images
  - And compress/optimize the header images with [this tool](https://tinyjpg.com/) 
- Change the color scheme, or at least the accent color (the template uses green), in `css/styles.css`
- Customize the header icons. They use [FontAwesome](https://fontawesome.com/docs/web/) icons
  - The template uses GitHub, LinkedIn, and Email icons. There are [plenty more](https://fontawesome.com/docs/web/add-icons/how-to#families-styles) available, though. I found the Brand icons especially useful
  - Don't forget to update the URLs that the icons link to, too!
- Adjust the sitemap's `changefreq` tags ([reference](https://www.sitemaps.org/protocol.html)) depending on how often you expect the content to be updated
- Adjust `robots.txt` to suit your needs

Finally, in your hosting environment, consider setting [Expires headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Expires) to control caching.
For example, here's what I have in my site's NGINX configuration:
```
    location ~* \.html$ {
        expires 30d;
    }
    location ~* \.css$ {
        expires 30d;
    }
    location ~* \.woff2$ {
        expires 30d;
    }
    location ~* \.ico$ {
        expires 30d;
    }
    location ~* \.png$ {
        expires 30d;
    }
    location ~* \.jpeg$ {
        expires 30d;
    }
    location ~* \.jpg$ {
        expires 30d;
    }
 ```
