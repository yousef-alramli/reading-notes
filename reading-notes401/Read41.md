# Dynamic Routs
- Page Path Depends on External Data

- We can pre-render pages with paths that depends on external data

## Implement getStaticPaths

- Create a file called [id].js inside the pages/posts directory.
- Also, remove first-post.js inside the pages/posts directory — we’ll no longer use this.
- paths contains the array of known paths returned by getAllPostIds(), which include the params defined by pages/posts/- [id].js. Learn more in the paths key documentation.
- Ignore fallback: false for now — we’ll explain that later.

## Implement getStaticProps

- We need to fetch necessary data to render the post with the given id.

## Render Markdown

- To render markdown content, we’ll use the remark library.

## Polishing the Post Page
- Adding title to the Post Page

    - In pages/posts/[id].js, let’s add the title tag using the post data. You’ll need to add an import for next/head at the top of the file and add the title tag by updating the Post component.


## Adding CSS

- Finally, let’s add some CSS using the file styles/utils.module.css we added before. Open pages/posts/[id].js, then add an import for the CSS file

## Polishing the Index Page

- let’s update our index page (pages/index.js). We need to add links to each post page using the Link component.

## Dynamic Routes Details
- Fetch External API or Query Database

    - Like getStaticProps, getStaticPaths can fetch data from any data source. In our example, getAllPostIds (which is used by getStaticPaths) may fetch from an external API endpoint

## Development v.s. Production

- In development (npm run dev or yarn dev), getStaticPaths runs on every request.
- In production, getStaticPaths runs at build time.

# Deploying Your Next.js App
## Push to GitHub

- Before we deploy, let’s push our Next.js app to GitHub if you haven’t done so already. This will make deployment easier.

- On your personal GitHub account, create a new repository called nextjs-blog. The repository can be public or private. You do not need to initialize it with a README or other files. If you need help setting up your repo, take a look at this guide on GitHub. Then:

- If you haven’t initialized the git repository locally for your Next.js app, do so now. Push the Next.js app to your GitHub repository.