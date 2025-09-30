# LJ Consulting Website

A modern, futuristic website for LJ Consulting built with Jekyll and hosted on GitHub Pages.

## Features

- 🚀 **Futuristic Design**: Modern, engaging UI with animations and effects
- 📱 **Responsive**: Works perfectly on desktop, tablet, and mobile devices
- 🎨 **Custom Theme**: Unique design tailored for IT consulting services
- 📝 **Blog System**: Easy-to-use blog with Jekyll collections
- ⚡ **Fast Loading**: Optimized for performance and SEO
- 🔧 **Easy Maintenance**: Simple Jekyll-based content management

## Services Highlighted

- Microsoft Products & Services
- Azure Cloud Solutions
- Infrastructure & Hardware
- Security Solutions
- Azure Virtual Desktop
- Support & Maintenance

## Technology Stack

- **Jekyll**: Static site generator
- **GitHub Pages**: Hosting platform
- **Custom CSS**: Futuristic design with animations
- **JavaScript**: Interactive features and form handling
- **Font Awesome**: Icons
- **Google Fonts**: Typography (Orbitron, Inter)

## Local Development

1. **Prerequisites**:
   - Ruby 3.1 or higher
   - Bundler gem

2. **Installation**:
   ```bash
   git clone <repository-url>
   cd ljconsulting
   bundle install
   ```

3. **Run locally**:
   ```bash
   bundle exec jekyll serve
   ```
   
   Visit `http://localhost:4000` to view the site.

## Custom Domain Setup

To use a custom domain with GitHub Pages:

1. **Add CNAME file**:
   Create a `CNAME` file in the root directory with your domain:
   ```
   yourdomain.com
   ```

2. **Configure DNS**:
   - Add a CNAME record pointing to `yourusername.github.io`
   - Or add A records pointing to GitHub Pages IP addresses

3. **Enable custom domain in GitHub**:
   - Go to repository Settings > Pages
   - Enter your custom domain
   - Enable "Enforce HTTPS"

## Adding Blog Posts

1. Create a new file in `_posts/` directory
2. Use the following front matter format:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   date: YYYY-MM-DD
   author: "LJ Consulting"
   categories: ["Category1", "Category2"]
   excerpt: "Brief description of your post"
   ---
   ```

3. Write your content in Markdown below the front matter

## Customizing the Site

### Colors and Styling
Edit `assets/css/main.css` to modify:
- Color scheme
- Typography
- Animations
- Layout

### Content
- **Homepage**: Edit `index.html`
- **Services**: Edit `services.md`
- **About**: Edit `about.md`
- **Contact**: Edit `contact.md`

### Navigation
Update the navigation menu in `_config.yml`:
```yaml
navigation:
  - title: "Home"
    url: "/"
  - title: "Services"
    url: "/services/"
```

## Deployment

The site automatically deploys to GitHub Pages when you push to the `main` branch. The GitHub Actions workflow handles the build and deployment process.

## Support

For questions about this website or LJ Consulting services, please contact us at [info@ljconsulting.com](mailto:info@ljconsulting.com).

## License

This website is proprietary to LJ Consulting. All rights reserved.
