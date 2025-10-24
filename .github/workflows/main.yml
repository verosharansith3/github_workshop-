name: Deploy to GitHub Pages

on:
  push:
    branches:
      - main  # Deploy whenever code is pushed to the main branch

permissions:
  contents: read
  pages: write
  id-token: write

jobs:
  deploy:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout repository
        uses: actions/checkout@v4

      - name: Setup Pages
        uses: actions/configure-pages@v5

      - name: Upload files
        uses: actions/upload-pages-artifact@v3
        with:
          path: .  # deploy everything in the root folder

      - name: Deploy to GitHub Pages
        uses: actions/deploy-pages@v4
