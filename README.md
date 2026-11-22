# Bugs’ Burrow

A single-page Bugs Bunny chat that runs SmolLM2-135M-Instruct in the browser with Transformers.js.

## GitHub Pages

In the repository, open **Settings → Pages** and choose **GitHub Actions** as the source. Push the site files to `main` to deploy. The **Deploy to GitHub Pages** workflow also supports manual runs from the **Actions** tab. GitHub shows the deployed URL in the workflow run and in **Settings → Pages**.

The workflow publishes `index.html` as a static page. On first use, visitors need network access to jsDelivr for Transformers.js and to Hugging Face for the model. The model stays in the browser cache while the browser retains it, and chat inference runs on the device.

To preview locally, run `python -m http.server 8000` from the repository and visit `http://localhost:8000`.
