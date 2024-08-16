# Running the Jekyll Server Locally

- MacOS
  - Installer `brew` package manager.
  - `brew install ruby`
  - `gem install --user-install bundler jekyll`
  - `cd` to the repo root.
  - `bundle install`
  - `bundle exec jekyll server`
  - Server will be running at `localhost:4000`

# Contributing

## Adding a new team member or board member

1. Create a new .md file in \_members and fill in the details, use the existing ones as a template.
2. Make sure the photo is square shaped, crop it if it is not, then add the photo to /assets/images/members/
3. Change the weight variable to reorder members, lower weights are displayed first.

### Adding a new sponsor

1. Create a new .md file in \_sponsors and fill in the details, use the existing ones as a template.
2. Crop the logo to roughly the same size as all the other ones before adding it to /assets/images/sponsors or you will break the layout.
3. Change the weight variable to reorder sponsors, lower weights are displayed first.

## Updating the front page events

1. Go to index.md and update the event variables: event-name, event-time, event-desc, event-link etc.
2. Make sure you do this after every event

## Image sizes and files

1. Cover picture and tiles: use the 'large' download settings from flickr
2. Team photos: use a minimum of 200x200 or any squarish shape, it will get resized to 200x200 with CSS
3. MAKE SURE ALL IMAGE EXTENSIONS I.E. JPG ARE lowercase (jpg not JPG)

## Upating the FAQ

Go to \_posts and update "2017-10-04-faq.md"

## Changing the homepage video

1. Go to \_layouts/home.html and replace the iframe code with the new video embed link (grab it from youtube):

```
<iframe width="100%" height="250" src="https://youtu.be/KyDHbgAVYvA" frameborder="0" allowfullscreen></iframe>
```
