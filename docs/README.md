# GitHub Pages Hosting

This folder contains the files needed to host the Surgical Edits Review UI on GitHub Pages.

## Files

- `index.html` - Landing page that redirects to the review UI
- `review_ui.html` - Main review interface
- `data/surgical_edits_dataset.json` - Default dataset file

## Setup Instructions

### 1. Enable GitHub Pages

1. Go to your GitHub repository
2. Click on **Settings** → **Pages** (in the left sidebar)
3. Under **Source**, select:
   - **Branch**: `main` (or your default branch)
   - **Folder**: `/docs`
4. Click **Save**

### 2. Access Your Hosted UI

After enabling GitHub Pages, your site will be available at:
```
https://[your-username].github.io/[repository-name]/
```

For example:
- `https://username.github.io/ft-idf-challenge-2025/`

The review UI will be accessible at:
```
https://[your-username].github.io/[repository-name]/review_ui.html
```

### 3. Share the Link

Simply share the URL with reviewers. They can:
- Access the UI directly in their browser
- Load the default dataset automatically
- Or upload their own dataset file using the file input

### 4. Updating the Dataset

To update the dataset:
1. Replace `docs/data/surgical_edits_dataset.json` with your new file
2. Commit and push to the repository
3. GitHub Pages will automatically update (may take a few minutes)

## Notes

- The UI automatically tries to load `./data/surgical_edits_dataset.json` on page load
- Users can still upload their own JSON files if needed
- All notes are saved to browser localStorage (per user)
- Notes can be exported as JSON for sharing

